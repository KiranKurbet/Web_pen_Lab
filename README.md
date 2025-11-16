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

## Quick Start (Kali Linux)

```bash
git clone https://github.com/yourname/Web-Pentest-Lab.git
cd Web-Pentest-Lab
pip install -r requirements.txt
playwright install chromium
chmod +x webpen.py
./webpen.py
