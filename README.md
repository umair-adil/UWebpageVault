# UWebpageVault  

View demo here:
https://www.youtube.com/watch?v=usWqJOVyS10

## Umair's Webpage Vault  

Encrypt and host private HTML pages with password-based access without requiring a back-end server.

---

## How it works

- encrypter.js encrypts HTML files into secure.json  
- index.html decrypts and loads pages in the browser  
- Uses AES-256-GCM encryption with PBKDF2 key derivation  
- Supports multiple passwords per page  
- Supports JavaScript/CSS inside the encrypted HTML pages  

---

## Setup

1. Place your HTML files beside encrypter.js  
2. Run:
node encrypter.js
3. Follow the console instructions  

---

## Publish

Only publish these files:

- index.html  
- secure.json  

Do NOT publish:

- passwords_file_PRIVATE.json  
- Original HTML files  

---

## Accessing Pages

Pages can be opened in index.html either:

- By entering a password manually  
- Or by using a URL hash, such as:  

index.html#yourpassword


---

## Notes

- The security of the pages is entirely dependent on the strength of the passwords  
- Password recovery is impossible without the original files or passwords  
- Increasing PBKDF2 iterations improves security but slows encryption/decryption, and vice versa  
- This project was initially created and iterated on my website repo before being moved to its own repository