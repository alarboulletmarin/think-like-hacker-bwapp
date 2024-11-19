---
layout: section
---

# Live Demonstration

---
layout: default
---

# SQL Injection Demo

<div class="grid grid-cols-2 gap-4">
<div>

## Vulnerability
```php
$query = "SELECT * FROM users 
          WHERE username='$username' 
          AND password='$password'";
```

## Attack Vector
```sql
username: admin' --
password: anything
```

</div>
<div v-click>

## Impact
- Authentication bypass
- Data exposure
- Database control

## Prevention
```php
$stmt = $pdo->prepare("SELECT * FROM users 
       WHERE username = ? AND password = ?");
$stmt->execute([$username, $password]);
```

</div>
</div>

---
layout: default
---

# XSS Attack Demo

<div class="grid grid-cols-2 gap-4">
<div>

## Vulnerable Code
```html
<input type="text" value="<?php echo $_GET['name']; ?>">
```

## Attack Payload
```javascript
"><script>alert('XSS')</script>
```

</div>
<div v-click>

## Impact
- Cookie theft
- Session hijacking
- Defacement

## Secure Code
```php
<input type="text" value="<?php echo htmlspecialchars($_GET['name']); ?>">
```

</div>
</div>

---
layout: center
class: text-center
---

# File Upload Vulnerability

<div class="grid grid-cols-2 gap-4 mt-4">
<div v-click>

## Vulnerable Setup
- No file type validation
- No size restrictions
- Unsafe file handling
- Predictable locations

</div>
<div v-click>

## Security Measures
- File type checking
- Size limitations
- Random naming
- Secure storage

</div>
</div>

---
layout: default
---

# Security Tools Used

<div class="grid grid-cols-3 gap-4">
<div v-click class="border p-4 rounded">
  <h3 class="text-lg font-bold">Burp Suite</h3>
  <ul>
    <li>Request interception</li>
    <li>Parameter testing</li>
    <li>Vulnerability scanning</li>
  </ul>
</div>
<div v-click class="border p-4 rounded">
  <h3 class="text-lg font-bold">OWASP ZAP</h3>
  <ul>
    <li>Automated scanning</li>
    <li>Attack simulation</li>
    <li>Security testing</li>
  </ul>
</div>
<div v-click class="border p-4 rounded">
  <h3 class="text-lg font-bold">Browser Tools</h3>
  <ul>
    <li>Developer console</li>
    <li>Network monitoring</li>
    <li>Cookie inspection</li>
  </ul>
</div>
</div>