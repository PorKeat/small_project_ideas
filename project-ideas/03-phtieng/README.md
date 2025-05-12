# Phtieng (ផ្ទៀង) ⚡📦

<div align="center">
  <img src="./assets/logo.png" alt="Phtieng Logo" width="480"/>

  <h3>Social Commerce Payment Slip Verifier & Auto-Order Bot</h3>
  <p><strong>Stop fake payment slips. Automate order address collection for Live sellers.</strong></p>

  <p align="center">
    <img src="https://img.shields.io/badge/pricing-%247--%2412%2Fmonth-brightgreen?style=flat-square" alt="Pricing" />
    <img src="https://img.shields.io/badge/verification-Instant%20OCR%20%2B%20QR-blue?style=flat-square" alt="OCR Verification" />
    <img src="https://img.shields.io/badge/platforms-Telegram%20%2B%20Messenger-orange?style=flat-square" alt="Platforms" />
  </p>
</div>

---

## 💡 About the Name
**Phtieng (ផ្ទៀង)** means **"to verify, match, or double-check"** in Khmer. It accurately describes what the automated bot does: verifying payment slips against real transaction records to protect live sellers from scams.

---

## 🛑 The Problem
1. **Fake Slip Scams:** Fraudulent buyers Photoshop bank transfer screenshots (Bakong/ABA/Wing) to steal merchandise.
2. **Hours of Manual Checking:** Live sellers waste 3–4 hours every night matching bank notifications with chat screenshots.
3. **Lost Customer Addresses:** Shipping info gets buried in long chat threads, causing delivery errors.

---

## ⚡ How It Works (Verification Flow)

```mermaid
flowchart TD
    A[Buyer sends bank transfer screenshot in Chat] --> B[Phtieng OCR Engine]
    B --> C[Extract Amount, TxID, Timestamp, Bank]
    C --> D{Is Slip Valid & Unique?}
    D -->|❌ No / Duplicate / Edited| E[🚨 Flag as Fake/Used & Alert Seller]
    D -->|✅ Yes| F[Mark Order as Paid]
    F --> G[Bot auto-sends 1-Click Delivery Address Form]
    G --> H[Auto-export shipping labels to Virak Buntham / J&T Express]
```

---

## 🔑 Key Features
* **Automated Slip Verification:** Validates amount, transaction ID, and timestamp instantly to block duplicates and fakes.
* **Smart Customer Form:** One-tap form to get precise phone number & delivery address.
* **1-Click Courier Export:** Exports clean shipping labels and spreadsheets directly formatted for delivery companies (J&T Express, Virak Buntham, Grab).

---

## 🛠️ Recommended Tech Stack
* **Bot Framework:** Telegraf (Node.js) / Grammy (TypeScript)
* **OCR & Image Parsing:** Google Cloud Vision / Tesseract / DeepSeek Vision
* **Database:** Supabase (PostgreSQL)
* **Hosting:** Cloudflare Workers / Fly.io
