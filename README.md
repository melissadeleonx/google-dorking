# Google Dorking Cheat Sheet

## 🚀 About
Google Dorking (also known as Google Hacking) is a technique used to uncover sensitive information exposed on the internet by leveraging advanced Google search operators.

⚠️ **Disclaimer:** This cheat sheet is for educational and ethical purposes only. Unauthorized access or data retrieval without permission may violate laws and policies.

---

## 🔍 Common Google Dorks

### 1️⃣ Finding Sensitive Files
```bash
filetype:log intext:"password"
filetype:txt intext:"username"
filetype:pdf intext:"confidential"
```

### 2️⃣ Exposed Login Pages
```bash
inurl:admin/login
inurl:dashboard
intitle:"index of" "admin"
```

### 3️⃣ Discovering Publicly Indexed Directories
```bash
intitle:"index of /" "parent directory"
intitle:"index of" site:example.com
```

### 4️⃣ Finding Cameras & IoT Devices
```bash
inurl:/view/view.shtml
inurl:axis-cgi/jpg
inurl:top.htm inurl:currenttime
```

### 5️⃣ Searching for Configuration Files
```bash
inurl:"config" filetype:xml
inurl:"wp-config.php"
inurl:config intitle:index.of
```

### 6️⃣ Exposing Databases
```bash
inurl:"phpmyadmin" intext:"Welcome to phpMyAdmin"
inurl:"/phpinfo.php"
filetype:sql "phpMyAdmin"
```

### 7️⃣ Finding Vulnerable Websites
```bash
inurl:"/wp-content/plugins/"
inurl:".git" "index of"
inurl:"/cgi-bin/" ext:sh
```

### 8️⃣ Open FTP Servers
```bash
intitle:"index of" inurl:ftp
inurl:"ftp://" site:example.com
```

---

## 🛡️ How to Protect Your Website
- **Use `robots.txt`** to prevent Google from indexing sensitive pages.
- **Disable directory listing** in the web server configuration.
- **Use proper authentication** to restrict access to sensitive files.
- **Monitor logs** to detect unauthorized access.
- **Regularly update and patch software** to avoid known exploits.

---

## 📚 Resources
- [Google Hacking Database (GHDB)](https://www.exploit-db.com/google-hacking-database)
- [Google Search Operators Guide](https://ahrefs.com/blog/google-advanced-search-operators/)
- [OWASP Google Dorking Cheatsheet](https://owasp.org/www-pdf-archive/Google_Dorks.pdf)

---

🚀 **Contribute:** If you have more useful Google Dorks, feel free to submit a pull request!

📧 **Contact:** If you have any questions, open an issue in the repo.

🔗 **Follow for more updates:** 

