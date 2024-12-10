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
Les injections : Avec plus de 25 vulnérabilités, ce domaine inclut les injections SQL, HTML, de commandes, XML/XPath, et LDAP. Ces vulnérabilités permettent d'apprendre à manipuler les systèmes en contournant leur logique de traitement des données. 

Les problèmes d’authentification : Avec 15 vulnérabilités, on y retrouve le contournement de l’authentification, les gestions de sessions faibles, les attaques par force brute, et même des problèmes liés aux cookies. Enfin, il y a d’autres vulnérabilités majeures, comme le Cross-Site Request Forgery (CSRF), l’upload de fichiers malveillants, ou les fuites d’informations sensibles.

Les failles XSS (Cross-Site Scripting) : Plus de 20 vulnérabilités y sont dédiées. Ces failles, telles que les XSS réfléchis, stockés ou basés sur le DOM, visent à manipuler l'exécution du code côté client.
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
Pour faciliter l’apprentissage, ces vulnérabilités sont également organisées en plusieurs catégories :

Par leur impact sur la sécurité : Cela inclut la confidentialité, l’intégrité, ou encore la disponibilité des données.
Par type d’attaque : Certaines vulnérabilités ciblent les clients, d’autres les serveurs, la logique métier, ou encore la configuration.
Par leur alignement avec l’OWASP Top 10 : bWAPP met un point d’honneur à suivre les bonnes pratiques et les principaux risques de sécurité identifiés dans le domaine.
Par contexte d’exploitation : On peut s’exercer sur des scénarios locaux ou distants, avec ou sans interaction utilisateur, et même en tenant compte du niveau d’authentification.
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
Enfin, bWAPP offre un parcours pédagogique adapté grâce à trois niveaux de difficulté :

Niveau débutant : Les vulnérabilités sont ici simples à exploiter, sans mécanismes de protection. C’est parfait pour les débutants afin de comprendre les bases.
Niveau intermédiaire : Les protections sont un peu plus robustes et nécessitent des techniques plus avancées pour être contournées.
Niveau expert : On atteint ici un niveau avancé, avec des protections complexes. C’est un véritable défi pour ceux qui maîtrisent déjà bien les concepts.

Ces niveaux permettent une progression pédagogique adaptée, avec des documentations et solutions détaillées pour accompagner l'apprentissage. 
Grâce à cette structuration, bWAPP est un outil idéal pour acquérir des compétences solides en sécurité web.
-->
