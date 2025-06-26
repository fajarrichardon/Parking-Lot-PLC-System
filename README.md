# 🚗 Parking Lot PLC System

> *This repository documents the project-based learning journey of building an automated parking lot system using PLC.*

## 📘 Introduction

This project is part of my personal journey in understanding **Programmable Logic Controllers (PLC)** through hands-on, project-based learning. The focus is on designing a smart parking lot system that can:

- Automatically detect cars entering and exiting
- Open/close the gate accordingly
- Provide real-time status of parking availability via indicator lamps

The system logic is implemented using **Ladder Diagram**, commonly used in industrial automation.

---

## 📊 System Overview

### 🔌 **Input Components**

| Input          | Function                                |
|----------------|-----------------------------------------|
| Sensor Masuk   | Mendeteksi mobil masuk ke area parkir   |
| Sensor Keluar  | Mendeteksi mobil keluar dari parkiran   |

### 💡 **Output Components**

| Output          | Function                                                  |
|-----------------|-----------------------------------------------------------|
| Gate            | Membuka/Tutup secara otomatis sesuai kondisi sensor       |
| Lampu Hijau     | Menyala saat masih tersedia slot parkir                   |
| Lampu Merah     | Menyala saat slot parkir penuh                            |

---

## 🧠 Block Diagram

```plaintext
+------------------+         +--------------+         +----------------+
|  Sensor Masuk    | ----->  |              |         |                |
|  Sensor Keluar   | ----->  |     PLC      | ----->  |     Output     |
|                  |         |  (Ladder     |         |  Devices:      |
|                  |         |  Program)    |         |  - Gate        |
|                  |         |              |         |  - Lampu Hijau |
|                  |         |              |         |  - Lampu Merah |
+------------------+         +--------------+         +----------------+
