# 🕵️‍♂️ Web Hunting Tool 🛠️

This tool helps find website vulnerabilities with features like CloudFlare detection, HTTP method analysis, and security checks. 🧑‍💻

## 🔥 Features

### 1. 🌩️ Check if a Website Uses CloudFlare
This feature identifies whether a website is protected by the CloudFlare content delivery network (CDN). By sending requests and analyzing responses, the tool determines if CloudFlare shields the website from direct access.

### 2. 🌐 Identify Supported HTTP Methods
HTTP methods (verbs like GET, POST, PUT, DELETE) are essential for communication between clients and servers. This feature tests a website's response to various HTTP methods to identify supported ones, which can reveal potential vulnerabilities such as:
- 💥 **Cross-Site Tracing (XST)**: A method that can allow sensitive information leakage if TRACE is enabled.

### 3. 🔒 Check for Insecure HTTP Headers
This feature scans the HTTP headers of a website to detect missing or misconfigured security headers. The following headers are analyzed:
- **X-XSS-Protection**: Protects against Cross-Site Scripting (XSS) attacks.
- **X-Content-Type-Options**: Prevents MIME-type sniffing to reduce exposure to drive-by download attacks.
- **HSTS (Strict-Transport-Security)**: Ensures connections are made over HTTPS.
- **CSP (Content-Security-Policy)**: Mitigates Cross-Site Scripting and other attacks.

### 4. 🗂️ Directory Finder for Common Files and Folders
This feature brute forces common directories and files on a website, helping you discover hidden resources like:
- Admin panels (`/admin/`)
- Login pages (`/login/`)
- Configuration files (`/config.php`)
- Backups (`/backup.zip`)
  
By finding these resources, you can gain insights into the site structure and potential entry points.

### 5. 🔥 Web Application Firewall (WAF) Detection
This feature detects the presence of a Web Application Firewall (WAF) by analyzing server responses and behaviors. WAFs protect websites from a variety of attacks, including:
- SQL injection
- Cross-Site Scripting (XSS)
- File inclusion attacks

### 6. 🔍 URL Parsing
This feature parses a given URL into its components such as protocol, domain, path, and query strings. It helps break down complex URLs, making it easier to analyze and understand what each part does. It is useful for inspecting redirect chains, URL manipulations, and understanding server responses.



## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/darkworld-king/Web-Hunting-Tool.git
2. cd WebHuntingTool
3. pip install -r requirements.txt
4. python3 WebHunter.py 
---

