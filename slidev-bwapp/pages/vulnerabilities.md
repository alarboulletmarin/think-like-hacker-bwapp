---
layout: section
---

# Vulnerability Exploration

<div class="slide-number">
  <SlideCurrentNo />/<SlideTotalNo />
</div>

<!--
Cette section explore les différentes vulnérabilités présentes dans bWAPP, permettant de comprendre leur diversité et leur impact sur la sécurité des applications web.
-->

---
layout: default
---

# Types of Vulnerabilities

<div class="mt-8 space-y-12">
  <div class="border-l-4 border-blue-500 pl-4">
    <h3 class="text-xl mb-2">💉 Injection Attacks</h3>
    <p>SQL, Command, LDAP, XML and HTML injections target data processing systems</p>
  </div>
  <div class="border-l-4 border-red-500 pl-4">
    <h3 class="text-xl mb-2">🔓 Authentication</h3>
    <p>Bypass techniques, weak sessions, brute force attacks compromise user accounts</p>
  </div>
  <div class="border-l-4 border-green-500 pl-4">
    <h3 class="text-xl mb-2">🌐 Cross-Site Scripting</h3>
    <p>Reflected, Stored and DOM-based XSS manipulate client-side execution</p>
  </div>
</div>

<div class="slide-number">
  <SlideCurrentNo />/<SlideTotalNo />
</div>

<!--
Les attaques par injection constituent la base de nombreuses vulnérabilités web. Les injections SQL, commandes et LDAP permettent de manipuler les systèmes. L'authentification et ses faiblesses représentent un vecteur d'attaque critique, tandis que le XSS expose les risques côté client. Ces trois catégories forment le socle des vulnérabilités web les plus courantes.
-->

---
layout: default
---

# Vulnerability Categories

<div class="grid gap-y-16 mt-12">
  <div class="grid grid-cols-2 gap-x-24">
    <div>
      <h3 class="text-blue-400 text-xl uppercase tracking-wider mb-6">Security Impact</h3>
      <div class="text-xl space-x-8">
        <span>Confidentiality</span>
        <span>Integrity</span>
        <span>Availability</span>
      </div>
    </div>
    <div>
      <h3 class="text-green-400 text-xl uppercase tracking-wider mb-6">Attack Surface</h3>
      <div class="text-xl space-x-8">
        <span>Client-side</span>
        <span>Server-side</span>
        <span>Logic</span>
      </div>
    </div>
  </div>
  <div class="grid grid-cols-2 gap-x-24">
    <div>
      <h3 class="text-purple-400 text-xl uppercase tracking-wider mb-6">Context</h3>
      <div class="text-xl space-x-8">
        <span>Authentication</span>
        <span>Authorization</span>
        <span>Data</span>
      </div>
    </div>
    <div>
      <h3 class="text-orange-400 text-xl uppercase tracking-wider mb-6">OWASP Alignment</h3>
      <div class="text-xl space-x-8">
        <span>Injection</span>
        <span>Auth</span>
        <span>Data</span>
      </div>
    </div>
  </div>
</div>

<div class="slide-number">
  <SlideCurrentNo />/<SlideTotalNo />
</div>

<!--
La catégorisation suit quatre axes essentiels :

- L'impact permet d'évaluer les conséquences (confidentialité, intégrité, disponibilité)
- La surface d'attaque identifie les points d'entrée (client, serveur, logique)
- Le contexte définit le cadre d'exploitation (authentification, autorisation, données)
- L'alignement OWASP assure la pertinence avec les standards actuels
-->

---
layout: default
---

# Learning Journey

<div class="grid grid-cols-2 gap-12 mt-12">
  <div class="space-y-8">
    <h3 class="text-xl mb-6">Difficulty Levels</h3>
    <div class="space-y-6">
      <div class="flex items-center gap-4">
        <span class="text-3xl">🎯</span>
        <div>
          <h4 class="font-bold">Beginner</h4>
          <p>Clear paths and basic concepts</p>
        </div>
      </div>
      <div class="flex items-center gap-4">
        <span class="text-3xl">🎯🎯</span>
        <div>
          <h4 class="font-bold">Intermediate</h4>
          <p>Multiple approaches required</p>
        </div>
      </div>
      <div class="flex items-center gap-4">
        <span class="text-3xl">🎯🎯🎯</span>
        <div>
          <h4 class="font-bold">Advanced</h4>
          <p>Complex protection bypass</p>
        </div>
      </div>
    </div>
  </div>

  <div class="space-y-8">
    <h3 class="text-xl mb-6">Learning Process</h3>
    <div class="space-y-6">
      <div class="flex items-center gap-4">
        <span class="text-3xl">📚</span>
        <div>
          <h4 class="font-bold">Foundation</h4>
          <p>Understanding core security concepts</p>
        </div>
      </div>
      <div class="flex items-center gap-4">
        <span class="text-3xl">🛠️</span>
        <div>
          <h4 class="font-bold">Practice</h4>
          <p>Hands-on vulnerability testing</p>
        </div>
      </div>
      <div class="flex items-center gap-4">
        <span class="text-3xl">🎓</span>
        <div>
          <h4 class="font-bold">Mastery</h4>
          <p>Advanced exploitation skills</p>
        </div>
      </div>
    </div>
  </div>
</div>

<div class="slide-number">
  <SlideCurrentNo />/<SlideTotalNo />
</div>

<!--
Le parcours pédagogique est progressif :

- Niveau débutant : vulnérabilités évidentes pour comprendre les concepts
- Niveau intermédiaire : protections basiques nécessitant des techniques avancées
- Niveau expert : défis complexes pour maîtriser les contre-mesures sophistiquées
-->