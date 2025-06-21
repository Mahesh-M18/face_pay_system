# 💳 Face Pay System – Two-Step Verification

A secure and efficient **Face Recognition-based Payment System** with an integrated **PIN verification** step using a 4x4 keypad. This system verifies a customer’s identity using face recognition and authorizes payment through a secondary PIN check.

---

## 🧠 Overview

This project was developed as a smart payment authentication system with two levels of verification:

1. **Face Recognition** using OpenCV and the `face_recognition` library  
2. **PIN Entry** using a 4x4 keypad interface

Ideal for Raspberry Pi deployment in kiosks, secure access systems, or pay-per-use setups.

---

## 🔧 Tech Stack

- **Programming Language**: Python  
- **Libraries**: OpenCV, face_recognition, NumPy, SQLite3  
- **Hardware Compatibility**: Raspberry Pi, Pi Camera, 4x4 Keypad

---

## 🗂️ Project Structure

| File/Folder                  | Description |
|-----------------------------|-------------|
| `dataset/`                  | Stores captured face images of customers |
| `photo/`                    | Stores live verification snapshots |
| `Create_DB.py`              | Creates the SQLite database schema |
| `Add_Customer.py`           | Adds new customer face data and info to DB |
| `Update_DB.py`              | Updates existing customer details |
| `Delete_DB.py`              | Deletes customer data from DB |
| `Select_customer_DB.py`     | Searches for customer records |
| `train_model.py`            | Encodes faces and generates `encodings.pickle` |
| `encodings.pickle`          | Serialized face encodings for recognition |
| `VERIFICATION_WITH_KEYPAD.py` | Main script: face verification + PIN |
| `TWO_STEP_VERIFICATION.py`  | Combined logic for both steps |
| `headshots_picam.py`        | Captures image using Pi Camera |
| `CUSTOMERS`                 | SQLite database file (`.db` format) |

---

