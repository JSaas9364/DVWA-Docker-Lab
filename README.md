<h1>🛡️ DVWA Docker Lab</h1>

<p>
This project sets up <a href="https://github.com/digininja/DVWA">Damn Vulnerable Web Application (DVWA)</a> in Docker using <code>docker-compose</code>. It’s built for local web app security testing and pentest practice using tools like Burp Suite, sqlmap, or your Kali VM.
</p>

---

<h2>🚀 Quick Start</h2>

<ol>
  <li>Clone the repo:
    <pre><code>git clone https://github.com/&lt;your-username&gt;/DVWA-Docker-Lab.git
cd DVWA-Docker-Lab</code></pre>
  </li>
  <li>Start the containers:
    <pre><code>docker compose up -d</code></pre>
  </li>
  <li>Open in browser:
    <pre><code>http://localhost/</code></pre>
  </li>
  <li>Click on <strong>Create / Reset Database</strong> on first load</li>
</ol>

---

<h2>📁 Project Structure</h2>

<pre>
DVWA-Docker-Lab/<br/>
├── docker-compose.yml<br/>
├── README.md<br/>
</pre>

---

<h2>📦 Containers Used</h2>

<table>
  <thead>
    <tr>
      <th>Service</th>
      <th>Description</th>
      <th>Docker Image</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>dvwa</td>
      <td>Web front-end (PHP)</td>
      <td><code>vulnerables/web-dvwa</code></td>
    </tr>
    <tr>
      <td>mysql</td>
      <td>MySQL 5.7 backend</td>
      <td><code>mysql:5.7</code></td>
    </tr>
  </tbody>
</table>

---

<h2>🔐 Default Credentials</h2>

<pre>
Username: admin
Password: password
</pre>

---

<h2>🧪 Pentest from Kali (Optional)</h2>

<pre>
nmap -p 80 &lt;host-ip&gt;<br/>
firefox http://&lt;host-ip&gt;<br/>
</pre>

<small>⚠️ Make sure your VM is in <strong>Bridged</strong> or <strong>Host-only</strong> mode and Docker is exposing port 80.</small>

---

<h2>📌 Notes</h2>

<ul>
  <li>Built with Docker + Docker Compose</li>
  <li>Tested on Windows 11 (WSL2 backend)</li>
  <li>Great for testing:
    <ul>
      <li>SQLi, XSS, CSRF</li>
      <li>Burp Suite/ZAP scans</li>
      <li>Low/Medium/High DVWA modes</li>
    </ul>
  </li>
</ul>

---

<h2>🛠️ TODO</h2>

<ul>
  <li>[ ] Add custom Docker network</li>
  <li>[ ] Automate ZAP/Burp scan via script</li>
  <li>[ ] Log attacks to ELK or Splunk</li>
</ul>
