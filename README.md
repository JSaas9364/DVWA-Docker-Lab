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
      <td>Web
