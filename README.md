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

## 🪜 Ladder Diagram Preview

![Ladder Diagram](Ladder_Diagramm.png)

---

Logika umum:
- Jika jumlah mobil < kapasitas ➝ Lampu Hijau ON, Gate bisa terbuka
- Jika jumlah mobil == kapasitas ➝ Lampu Merah ON, Gate tidak bisa terbuka
- Jika sensor masuk atau keluar on dan terdapat slot parkir ➝ Gate terbuka 3 detik  

---

## 🚀 Features

- Otomatisasi sistem parkir berbasis PLC
- Indikator kondisi parkir secara real-time
- Simulasi Ladder Diagram menggunakan software PLC
- Bisa dikembangkan menjadi sistem parkir skala besar

---

## 🔧 Tools Used

- PLC Software: *CX-Programmer / TIA Portal / Zelio Soft / lainnya*
- PLC Hardware: *(Opsional: isi jika menggunakan model tertentu)*
- Sensor Infrared / Proximity (simulasi atau real)
- GitHub untuk dokumentasi versi

---

## 💬 Personal Note

Project ini menjadi langkah awal saya mendalami dunia **otomasi industri dan logika kontrol**. Saya sangat menikmati proses memecahkan masalah dunia nyata dengan pendekatan teknik.  
Melalui project ini, saya belajar tentang pemrograman PLC, bagaimana menyusun logika ladder diagram, serta pentingnya pemikiran sistematis dalam merancang solusi berbasis sensor dan aktuator.

Saya berharap repo ini bisa jadi referensi atau inspirasi bagi siapa pun yang ingin memulai belajar PLC dengan cara yang praktis dan menyenangkan.

---

## 📫 Contact

> **Fajar Richardo Nainggolan**  
📧 Email: [your-email@example.com]  
🔗 LinkedIn: [linkedin.com/in/yourprofile](#)
