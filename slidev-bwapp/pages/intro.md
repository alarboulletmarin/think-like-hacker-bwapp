---
layout: default
---

# Overview

<div class="mt-12 mb-12 ml-12">
  <div class="space-y-6 text-xl">
    <div class="flex items-center gap-4">
      <span class="text-blue-500">1.</span>
      <p>Introduction to bWAPP</p>
    </div>
    <div class="flex items-center gap-4">
      <span class="text-blue-500">2.</span>
      <p>Technical Overview</p>
    </div>
    <div class="flex items-center gap-4">
      <span class="text-blue-500">3.</span>
      <p>Vulnerability Exploration</p>
    </div>
    <div class="flex items-center gap-4">
      <span class="text-blue-500">4.</span>
      <p>Live Demonstrations</p>
    </div>
    <div class="flex items-center gap-4">
      <span class="text-blue-500">5.</span>
      <p>Analysis & Conclusion</p>
    </div>
  </div>
</div>

<div class="slide-number">
  <SlideCurrentNo />/<SlideTotalNo />
</div>

<!--
Cette présentation se structure en cinq parties principales :
1. Une introduction pour comprendre bWAPP et ses objectifs
2. Un aperçu technique détaillant l'architecture et le déploiement
3. Une exploration des différentes vulnérabilités
4. Des démonstrations pratiques d'attaques
5. Une analyse et conclusion sur l'outil
-->

---
layout: center
---


# What is bWAPP?

Buggy Web Application (bWAPP) is an open-source deliberately vulnerable web application designed for cybersecurity education.

<v-clicks>

- 🎯 **Purpose**: Educational platform for security testing
- 🔓 **Features**: 100+ vulnerabilities and security flaws
- 🛠 **Usage**: Hands-on security training and testing
- 🎓 **Target**: Security professionals, developers, students

</v-clicks>

<div class="slide-number">
  <SlideCurrentNo />/<SlideTotalNo />
</div>

<!--
Pour commencer cette présentation, bWAPP est une application web volontairement vulnérable. Elle a été conçue spécifiquement pour l'apprentissage de la sécurité informatique. Avec plus de 100 vulnérabilités intégrées, elle offre un environnement idéal pour la formation pratique aux tests de sécurité. Elle s'adresse aussi bien aux professionnels de la sécurité qu'aux développeurs et étudiants.
-->

---
layout: default
---

# Why bWAPP Matters?

<div class="grid grid-cols-2 gap-4 p-4">
  <div class="bg-blue-50/20 p-4 rounded">
    <h3 class="font-bold mb-4 text-blue-600">Learning Environment</h3>
    <div class="space-y-2">
      Practice in real-world scenarios
      Safe testing environment
      Complete vulnerability coverage
    </div>
  </div>

  <div class="bg-green-50/20 p-4 rounded">
    <h3 class="font-bold mb-4 text-green-600">Professional Benefits</h3>
    <div class="space-y-2">
      Practical hands-on experience
      Progressive difficulty levels
      Active community expertise
    </div>
  </div>
</div>

<div class="grid grid-cols-2 gap-4 p-4 mt-2">
  <div class="bg-purple-50/20 p-4 rounded">
    <h3 class="font-bold mb-4 text-purple-600">Security Training</h3>
    <div class="space-y-2">
      Comprehensive documentation
      Structured learning path
      Professional certification prep
    </div>
  </div>

  <div class="bg-orange-50/20 p-4 rounded">
    <h3 class="font-bold mb-4 text-orange-600">Development Impact</h3>
    <div class="space-y-2">
      Code security awareness
      Best practice implementation
      Vulnerability prevention
    </div>
  </div>
</div>

<div class="slide-number">
  <SlideCurrentNo />/<SlideTotalNo />
</div>

<!--
L'importance de bWAPP se manifeste à travers quatre aspects clés. C'est un environnement d'apprentissage qui permet de pratiquer sur des scénarios réels en toute sécurité. Professionnellement, elle offre une expérience pratique progressive avec le soutien d'une communauté active. Pour la formation, elle fournit une documentation complète et un parcours structuré. Enfin, côté développement, elle sensibilise aux bonnes pratiques de sécurité et à la prévention des vulnérabilités.
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

# Security Training Impact

<div class="grid grid-cols-2 gap-x-16 gap-y-20 p-12 relative">
  <!-- Éducation -->
  <div class="flex items-start space-x-6">
    <div class="text-purple-600">
      <carbon:education class="text-3xl" />
    </div>
    <div>
      <h3 class="text-gray-400 uppercase tracking-wider text-sm mb-2">Practical Learning</h3>
      <p class="text-xl">From theory to real-world application</p>
    </div>
  </div>

  <!-- Certification -->
  <div class="flex items-start space-x-6">
    <div class="text-orange-600">
      <carbon:certificate class="text-3xl" />
    </div>
    <div>
      <h3 class="text-gray-400 uppercase tracking-wider text-sm mb-2">Professional Growth</h3>
      <p class="text-xl">Certification preparation</p>
    </div>
  </div>

  <!-- Développement -->
  <div class="flex items-start space-x-6">
    <div class="text-green-600">
      <carbon:development class="text-3xl" />
    </div>
    <div>
      <h3 class="text-gray-400 uppercase tracking-wider text-sm mb-2">Development Skills</h3>
      <p class="text-xl">Secure coding in practice</p>
    </div>
  </div>

  <!-- Analyse -->
  <div class="flex items-start space-x-6">
    <div class="text-red-600">
      <carbon:analytics class="text-3xl" />
    </div>
    <div>
      <h3 class="text-gray-400 uppercase tracking-wider text-sm mb-2">Security Analysis</h3>
      <p class="text-xl">Threat assessment expertise</p>
    </div>
  </div>
</div>

<div class="slide-number">
  <SlideCurrentNo />/<SlideTotalNo />
</div>

<!--
L'impact sur la formation en sécurité se décline en quatre axes. L'apprentissage pratique permet de passer de la théorie à l'application réelle. La croissance professionnelle est soutenue par la préparation aux certifications. Les compétences en développement sont renforcées par la pratique du code sécurisé. L'expertise en analyse de sécurité s'acquiert à travers l'évaluation des menaces. Cette approche globale assure une formation complète en sécurité web.
-->