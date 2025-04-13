# Firebase Emulator Suite - Shopping Cart Demo

This project is a local simulation of a shopping cart system using the **Firebase Emulator Suite**. It demonstrates how to develop, test, and secure Firebase apps offline using Firestore, Cloud Functions, and Firebase security rules.

## 🔧 Tech Stack
- Firebase Emulator Suite
- Firestore (Emulator)
- Cloud Functions (Emulator)
- Firebase Authentication (Mocked in tests)
- Mocha (Testing Framework)
- Node.js

---

## 📁 Project Structure
codelab-initial-state/ ├── functions/ # Cloud Functions │ ├── index.js # calculateCart() logic │ ├── test.js # Mocha test suite │ └── package.json ├── firestore.rules # Firestore security rules ├── firebase.json # Emulator config └── seed/ # Seed data for emulators

---

## 🚀 Features

- 🔐 Secure Firestore rules (only owners can read/write their cart)
- 🔄 Real-time Cloud Function that recalculates total cart price
- 🧪 Unit tests using Mocha to verify functionality and security
- 🖥️ Firebase Emulator UI + Web UI simulation (`localhost:5000`)

---

## ✅ Completed Tasks

- [x] Ran Firebase emulators locally
- [x] Configured Firestore security rules for user isolation
- [x] Wrote and deployed a Cloud Function (`calculateCart`)
- [x] Wrote 5 passing unit tests with Mocha
- [x] Connected to frontend and tested "Add to Cart" UI flow
- [x] Recorded demo video walkthrough

---

## 🧪 Running the Project

### 1. Install Dependencies
```bash
cd functions
npm install


2. Start Firebase Emulators
firebase emulators:start --import=./seed

3. Run Tests
cd functions
npm test


🔗 Demo
🖥️ Emulator UI: http://localhost:4000

🛒 Frontend UI: http://localhost:5050
