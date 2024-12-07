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

---
layout: default
---

# 🔧 Security Considerations

<div class="grid grid-cols-2 gap-8 p-6">
  <div class="p-4 bg-red-50/20 rounded">
    <h3 class="text-xl mb-4">⚠️ Container Isolation</h3>
    <p>Keep container isolated from production environments</p>
  </div>

  <div class="p-4 bg-yellow-50/20 rounded">
    <h3 class="text-xl mb-4">🔐 Network Security</h3>
    <p>Restrict port exposure to localhost only</p>
  </div>

  <div class="p-4 bg-orange-50/20 rounded">
    <h3 class="text-xl mb-4">🔍 Monitoring</h3>
    <p>Track container resource usage and access</p>
  </div>

  <div class="p-4 bg-purple-50/20 rounded">
    <h3 class="text-xl mb-4">🔄 Reset State</h3>
    <p>Regular container recreation for clean state</p>
  </div>
</div>

<div class="slide-number">
  <SlideCurrentNo />/<SlideTotalNo />
</div>