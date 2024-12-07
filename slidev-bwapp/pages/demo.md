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

# Stored XSS Attack in Blog

<div class="grid grid-cols-2 gap-8">
  <div>
    <h3 class="text-xl mb-4">Attack Scenario</h3>
    <div class="space-y-4">
      <p>1. Normal blog functionality</p>
      <p>2. Advanced XSS payload injection</p>
      <p>3. Cookie theft simulation</p>
    </div>
  </div>
  <div class="flex flex-col justify-center">
    <h3 class="text-xl mb-4">Security Impact</h3>
    <div class="space-y-4">
      <p>• Persistent malicious code</p>
      <p>• Session hijacking risks</p>
      <p>• Data confidentiality breach</p>
    </div>
  </div>
</div>

<!-- Emplacement pour le GIF de démonstration -->
<!-- <div class="mt-8">
  <img 
    src="/demos/stored-xss.gif" 
    class="rounded-lg shadow-lg w-full"
    alt="Stored XSS Attack demonstration"
  />
</div> -->

<div class="slide-number">
  <SlideCurrentNo />/<SlideTotalNo />
</div>

---
layout: default
---

# Directory Traversal Exploitation

<div class="grid grid-cols-2 gap-8">
  <div>
    <h3 class="text-xl mb-4">Attack Methodology</h3>
    <div class="space-y-4">
      <p>1. Path manipulation techniques</p>
      <p>2. Filter bypass methods</p>
      <p>3. Sensitive file access</p>
    </div>
  </div>
  <div class="flex flex-col justify-center">
    <h3 class="text-xl mb-4">Critical Findings</h3>
    <div class="space-y-4">
      <p>• System file exposure</p>
      <p>• Configuration leakage</p>
      <p>• Security boundary bypass</p>
    </div>
  </div>
</div>

<!-- Emplacement pour le GIF de démonstration -->
<!-- <div class="mt-8">
  <img 
    src="/demos/directory-traversal.gif" 
    class="rounded-lg shadow-lg w-full"
    alt="Directory Traversal demonstration"
  />
</div> -->

<div class="slide-number">
  <SlideCurrentNo />/<SlideTotalNo />
</div>

---
layout: default
---

# Technical Impact Analysis

<div class="grid grid-cols-2 gap-8">
  <div class="bg-red-50/20 p-6 rounded-lg">
    <h3 class="text-xl mb-4">Stored XSS</h3>
    <div class="space-y-4">
      <p>• Affects all visitors</p>
      <p>• Persists in database</p>
      <p>• Cross-user impact</p>
      <p>• Session compromise</p>
    </div>
  </div>
  <div class="bg-blue-50/20 p-6 rounded-lg">
    <h3 class="text-xl mb-4">Directory Traversal</h3>
    <div class="space-y-4">
      <p>• File system access</p>
      <p>• Information disclosure</p>
      <p>• Configuration exposure</p>
      <p>• Privacy violation</p>
    </div>
  </div>
</div>

<div class="slide-number">
  <SlideCurrentNo />/<SlideTotalNo />
</div>