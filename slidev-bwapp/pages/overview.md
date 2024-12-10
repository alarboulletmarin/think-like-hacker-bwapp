---
layout: section
---

# Technical Overview

<div class="slide-number">
  <SlideCurrentNo />/<SlideTotalNo />
</div>

---
layout: default
---

# 🎨 Architecture Components

<div class="grid grid-cols-3 gap-8 p-6">
  <div class="p-4 bg-blue-50/20 rounded">
    <h3 class="text-blue-600 mb-2">Interface Layer</h3>
    <p>Web interface and admin console with dynamic forms navigation</p>
  </div>

  <div class="p-4 bg-green-50/20 rounded">
    <h3 class="text-green-600 mb-2">Process Layer</h3>
    <p>PHP backend handling authentication and business logic</p>
  </div>

  <div class="p-4 bg-purple-50/20 rounded">
    <h3 class="text-blue-600 mb-2">Data Layer</h3>
    <p>MySQL database with secure file storage system</p>
  </div>
</div>

<div class="slide-number">
  <SlideCurrentNo />/<SlideTotalNo />
</div>

<!--
L'architecture de bWAPP est composée de trois couches distinctes :
L'interface utilisateur, qui gère les interactions avec les formulaires et la console d'administration.
Le backend PHP, responsable du traitement des données et de l'authentification.
La base de données MySQL, qui assure le stockage sécurisé des données.
Cette architecture en couches représente une approche classique des applications web modernes.
-->

---
layout: default
---

# Open Source & Free

<div class="mt-12 grid grid-cols-2 gap-8">
  <div class="p-6 bg-blue-50/20 rounded-lg">
    <h3 class="text-xl mb-4 font-bold">💻 Open Source</h3>
    <div class="space-y-4">
      <p>• Source code publicly available</p>
      <p>• Community contributions welcome</p>
      <p>• Transparent security practices</p>
    </div>
  </div>

  <div class="p-6 bg-green-50/20 rounded-lg">
    <h3 class="text-xl mb-4 font-bold">🆓 Free to Use</h3>
    <div class="space-y-4">
      <p>• No license fees</p>
      <p>• Unlimited usage</p>
      <p>• Free updates</p>
    </div>
  </div>
</div>

<div class="mt-8 p-6 bg-purple-50/20 rounded-lg">
  <h3 class="text-xl mb-4 font-bold">🌐 Community Benefits</h3>
  <div class="space-y-4">
    <p>Accessible cybersecurity education for everyone</p>
    <p>Active community sharing knowledge and experiences</p>
  </div>
</div>

<div class="slide-number">
  <SlideCurrentNo />/<SlideTotalNo />
</div>

---
layout: default
---

# 🐳 Docker Deployment

<div class="grid grid-cols-2 gap-8 p-6">
  <div class="p-4 bg-blue-50/20 rounded">
    <h3 class="text-xl mb-4">Quick Start</h3>
    <div class="font-mono text-sm bg-gray-900 text-gray-100 p-4 rounded">
      docker run -d -p 80:80 raesene/bwapp
    </div>
  </div>

  <div class="p-4 bg-green-50/20 rounded">
    <h3 class="text-xl mb-4">Initial Setup</h3>
    <div class="space-y-2">
      <p>1. Access http://localhost/install.php</p>
      <p>2. Initialize the database</p>
      <p>3. Login with bee:bug</p>
    </div>
  </div>

  <div class="p-4 bg-purple-50/20 rounded">
    <h3 class="text-xl mb-4">Management</h3>
    <div class="space-y-2">
      <p>Container status check:</p>
      <div class="font-mono text-sm bg-gray-900 text-gray-100 p-2 rounded">
        docker ps | grep bwapp
      </div>
    </div>
  </div>

  <div class="p-4 bg-orange-50/20 rounded">
    <h3 class="text-xl mb-4">Persistence</h3>
    <p>Data persists within container, reset by restarting</p>
  </div>
</div>

<div class="slide-number">
  <SlideCurrentNo />/<SlideTotalNo />
</div>

<!--Le déploiement est simplifié grâce à Docker avec une seule commande : 'docker run -d -p 80:80 raesene/bwapp'. 
Une fois déployé, l'initialisation de la base de données s'effectue via l'interface d'installation, suivie d'une connexion avec les identifiants par défaut. 
La gestion du conteneur s'effectue aisément avec les commandes Docker standards. Les données sont conservées entre les sessions, mais peuvent être réinitialisées par un simple redémarrage du conteneur.
-->

---
layout: default
---

# ⚙️ Environment Setup

<div class="grid grid-cols-2 gap-8 p-6">
  <div class="p-4 bg-blue-50/20 rounded">
    <h3 class="text-xl mb-4">💻 Core Stack</h3>
    <p>PHP + MySQL + Apache in containerized environment</p>
  </div>

  <div class="p-4 bg-green-50/20 rounded">
    <h3 class="text-xl mb-4">🌐 Access</h3>
    <p>Web interface on http://localhost:80</p>
  </div>

  <div class="p-4 bg-purple-50/20 rounded">
    <h3 class="text-xl mb-4">🔧 Requirements</h3>
    <p>Docker Engine on Linux, Windows, or macOS</p>
  </div>

  <div class="p-4 bg-orange-50/20 rounded">
    <h3 class="text-xl mb-4">🔒 Isolation</h3>
    <p>Container-based security boundary</p>
  </div>
</div>

<div class="slide-number">
  <SlideCurrentNo />/<SlideTotalNo />
</div>

<!--
L'environnement technique s'appuie sur une stack LAMP conteneurisée. L'application est accessible via localhost sur le port 80. 
Les prérequis techniques sont minimaux — seul Docker doit être installé sur le système d'exploitation. 
L'utilisation des conteneurs apporte une couche d'isolation sécurisée supplémentaire.
-->
