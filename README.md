# 🔐 Browser PGP Tool

A modern, client-side OpenPGP encryption tool built with **OpenPGP.js** that runs entirely inside your web browser.

Generate PGP key pairs, encrypt and decrypt messages or files, digitally sign data, verify signatures, and manage your key ring—all without sending your information to a server.

---

## ✨ Features

### 🔑 Key Generation

* Generate modern **Curve25519 (ECC)** key pairs *(recommended)*
* Generate **RSA 2048** or **RSA 4096** key pairs
* Optional passphrase protection for private keys
* Export public and private keys as `.asc` files

---

### 📋 Built-in Key Ring

* Store public and private keys locally
* Import existing PGP public or private keys
* View fingerprints
* Export stored keys
* Delete individual keys or clear the entire key ring

---

### 🔒 Encryption

Encrypt:

* Plain text messages
* Files of virtually any type

Supports:

* ASCII-armored output (`.asc`)
* Binary encrypted output (`.gpg`)
* Optional digital signing during encryption

---

### 🔓 Decryption

Decrypt:

* PGP encrypted messages
* ASCII armored encrypted files
* Binary encrypted files

Supports automatic detection of armored and binary PGP formats.

---

### ✍️ Digital Signatures

Create OpenPGP clear-text signatures using your private key.

Useful for:

* Authenticating messages
* Proving authorship
* Detecting tampering

---

### ✅ Signature Verification

Verify signed messages using the sender's public key.

Confirms:

* Message integrity
* Message authenticity
* Whether the signature is valid

---

### 📁 File Encryption

Supports drag-and-drop encryption and decryption for files directly inside the browser.

No upload process is required.

---

## 🔒 Security

This application is designed with a **privacy-first architecture**.

### Everything runs locally

All cryptographic operations are performed inside your browser using OpenPGP.js.

The application **does not transmit**:

* Keys
* Messages
* Files
* Passphrases

to any remote server.

Your data remains on your own device unless **you choose to share it**.

---

### Modern cryptography

Supports:

* Curve25519 ECC
* RSA 2048 / RSA 4096
* OpenPGP standard encryption
* Digital signatures
* Fingerprint verification

Cryptographic operations are provided by the trusted **OpenPGP.js** library.

---

### Private key protection

When generating a key pair, you can protect your private key with a passphrase.

If a passphrase is used:

* the private key remains encrypted while stored.

If **no passphrase is used**:

* the private key is stored unencrypted in the browser's local storage.

For this reason:

* Always use a strong passphrase.
* Do not use the tool on shared or public computers.
* Lock your browser profile and operating system.

The application also displays warnings whenever unprotected private keys are detected.

---

### Local Storage

The built-in key ring uses your browser's **localStorage**.

Nothing is uploaded automatically.

Stored keys remain only on that browser until you remove them or clear browser storage.

---

## ⚠️ Security Considerations

Although all encryption happens locally, your overall security still depends on your environment.

For maximum protection:

* Use a strong passphrase for private keys.
* Keep your operating system secure.
* Avoid installing untrusted browser extensions.
* Verify public key fingerprints before encrypting sensitive information.
* Back up important private keys securely.

---

## 🚀 Getting Started

1. Download the project.
2. Open `pgp.html` in a modern browser.
3. Generate or import a key pair.
4. Encrypt, decrypt, sign, or verify messages.

No installation or backend server is required.

---

## 📦 Technologies Used

* HTML5
* CSS3
* JavaScript
* OpenPGP.js v5

---

## 🎯 Use Cases

* Secure communication
* Email encryption
* File encryption
* Digital signatures
* Identity verification
* Secure document exchange
* Learning how OpenPGP works

---

## 📜 License

Feel free to modify and use this project according to the license you choose.

---

## Disclaimer

This tool is intended for educational and practical use. While it uses well-established OpenPGP cryptography, no software can guarantee complete security. Users are responsible for protecting their devices, safeguarding private keys, verifying public keys, and following good operational security practices.
