# Ven (វេន) ⏱️💈

<div align="center">
  <img src="./assets/logo.png" alt="Ven Logo" width="480"/>

  <h3>Smart Queue & Appointment Booking via Telegram</h3>
  <p><strong>Eliminate crowded waiting areas. Give customers live queue updates.</strong></p>

  <p align="center">
    <img src="https://img.shields.io/badge/pricing-%245--%248%2Fmonth-brightgreen?style=flat-square" alt="Pricing" />
    <img src="https://img.shields.io/badge/target-Barbers%2C%20Salons%2C%20Clinics-blue?style=flat-square" alt="Target" />
    <img src="https://img.shields.io/badge/notifications-Live%20Telegram%20Alerts-orange?style=flat-square" alt="Notifications" />
  </p>
</div>

---

## 💡 About the Name
**Ven (វេន)** means **"turn / shift / queue slot"** in Khmer. It is a sleek, 1-syllable modern name that represents organizing customers by their rightful turn smoothly.

---

## 🛑 The Problem
1. **Lost Walk-In Customers:** Customers leave if they see a crowded barbershop or salon with an unknown wait time.
2. **Messy Booking:** Booking appointments through chat messages leads to double-bookings and no-shows.

---

## ⚡ How It Works (Queue Flow)

```mermaid
sequenceDiagram
    autonumber
    actor Customer as 👤 Customer
    participant Bot as 🤖 Ven Telegram Bot
    actor Barber as 💈 Barber / Specialist

    Customer->>Bot: Scans QR / Taps "Join Queue"
    Bot-->>Customer: Issues Digital Ticket #14 ("3 people ahead of you")
    Note over Customer: Waits comfortably at a nearby cafe
    Barber->>Bot: Finishes client & taps "Call Next"
    Bot->>Customer: 🔔 "Your turn in 5 mins! Please head to Chair #2."
    Customer->>Barber: Arrives right on time with zero waiting
```

---

## 🔑 Key Features
* Virtual Queue ticketing without app installation.
* Staff dashboard to call the next customer in 1 tap.
* Telegram reminder notifications to minimize no-shows.
