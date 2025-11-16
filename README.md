# Web-Pentest-Lab v12.4 – **DVWA Killer**  

**Automated Web Vulnerability Scanner**  
- Directory brute-force (custom wordlist)  
- SQLi / XSS / CSRF-bypass detection  
- Full crawling + form testing  
- Screenshots (Playwright)  
- **Web Dashboard** (HTML/CSS/JS) – no server needed  
- Proxy chain support  
- Kali Linux ready  

---

## Features

| Feature | Status |
|--------|--------|
| Turbo brute (25 k paths < 60 s) | Working |
| Auto-login + CSRF token refresh | Working |
| `security=low` cookie injection | Working |
| SQLi → sqlmap auto-run | Working |
| Reflected XSS proof | Working |
| Responsive HTML report | Working |
| Screenshots embedded | Working |

---

---
Example Run :-

Target URL: http://192.168.5.129/dvwa 

Threads: 50

Brute-force? y

Wordlist path: /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt

Login? y → admin / password

---

---

Output :-

[Critical] SQLi → Form: id

[High] XSS → Reflected: message

[+] SCAN COMPLETE!

    Open: file:///home/kali/Web-Pentest-Lab/webpen-output/2025-11-16_15-42-22/display/index.html

---

## Quick Start (Kali Linux)

Note :- create the virtual environment berfor install requirement.txt

```bash
git clone https://github.com/KiranKurbet/Web_pen_Lab.git
cd Web_pen_lab 
pip install -r requirements.txt
playwright install chromium
chmod +x webpen.py
./webpen.py
