# 🦉 CipherBite: Secure Offline Text Encryption

[![Play Store Download](https://img.shields.io/badge/Get_it_on-Google_Play-000000?style=for-the-badge&logo=google-play&logoColor=white)](https://play.google.com/store/apps/details?id=com.purnomosidi.cipherbite)
[![Flutter](https://img.shields.io/badge/Built_with-Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)]()
[![Security](https://img.shields.io/badge/Encryption-AES--256-red?style=for-the-badge)]()

Sharing sensitive credentials—like passwords, PINs, or API keys—via chat or email is a common habit, but it comes with a massive privacy risk if a device is lost or compromised. 

**CipherBite** is designed to solve this exact problem. Instead of sending plain text, CipherBite converts your sensitive information into unique, encrypted cipher text that can only be decoded through the app. We strictly adhere to the golden rule of cybersecurity: "Never roll your own crypto". That is why CipherBite is powered by industry-standard AES-256 encryption. The app operates 100% offline, relying entirely on on-device computation without the need for a backend server.

---

## 🚀 Key Features & Tools

CipherBite offers a robust suite of privacy tools out of the box. We believe in providing military-grade security to everyone, which is why our core encryption tools are available for free.

### 🛡️ Free Tools
* **Military-Grade Security:** Encrypts and decrypts text using the globally trusted AES-256 standard algorithm.
* **100% Offline & On-Device:** Zero internet connection is required for the core encryption process, guaranteeing maximum privacy. 
* **Double-Layer Local Vault:** Automatically saves your encryption and decryption history locally in an encrypted SQLCipher database, protected from unauthorized access.
* **Encrypted Cloud Backup:** Safely backup your vault to a hidden, protected folder (`appDataFolder`) in your personal Google Drive, which cannot be tampered with outside the app.
* **Dark Mode & Multi-Language:** Built with a beautiful, modern UI that supports dynamic themes (Light/Dark) and multiple languages (Default: US English & Indonesian).
* **Wipe Data Option:** Full control to instantly clear all local data, wiping the SQLCipher database and user preferences permanently.
* **Smart Onboarding:** A beautiful, animated onboarding wizard designed to guide new users on their first launch.

### 💎 Pro Features (Subscription)
For power users who need an extra layer of granular security, upgrading to **CipherBite Pro** (`cipherbite_pro`) unlocks the following capabilities:
* **PIN Protection:** Add an extra layer of security by requiring a specific PIN to decode a secret message.
* **Ad-Free Experience:** Remove all non-intrusive AdMob banner ads for a cleaner, distraction-free interface.

---

## 🛠️ The Tech Stack

CipherBite is engineered for maximum performance, security, and maintainability.

| Technology | Purpose in CipherBite |
| :--- | :--- |
| **Flutter** | Builds a high-performance, natively compiled application from a single codebase. |
| **Riverpod** | Acts as the backbone for state management, ensuring the app reacts instantly to database changes without requiring an app restart. |
| **SQLCipher** | Provides a double-layer security architecture by encrypting the `.db` file that saves the AES-256 cipher text. |
| **Google Drive API** | Utilizes the unique `appDataFolder` scope via Google Sign-in v7.2.0 for seamless and tamper-proof cloud backups. |
| **Firebase** | Handles Firebase Analytics to track screen popularity and Firebase Cloud Messaging (FCM) for targeted deep-link notifications. |
| **In-App Purchase** | Communicates with Google Play Billing to manage flexible updates and Pro subscriptions automatically. |

---

## 📥 Installation

CipherBite is currently available for Android devices. 

> **Download Now:** Get it directly from the [Google Play Store](https://play.google.com/store/apps/details?id=com.purnomosidi.cipherbite).

---

## 🔒 Privacy First

Your data belongs to you. CipherBite operates locally on your device. The AES-256 encryption happens within the processor of your phone, and the encrypted SQLite history is locked behind a password known only to the app's internal system. When you back up to Google Drive, the database remains fully encrypted and inaccessible to regular Google Drive apps.
