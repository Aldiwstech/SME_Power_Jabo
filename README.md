# ⚡ Power Management System - SME Operations (JABO Region)

Web dashboard operasional interaktif berbasis real-time untuk pemantauan catu daya (*power & energy*), pelacakan alarm NMS Huawei, eskalasi tiket *maintenance* 2nd-level support, serta penjadwalan *Preventive Maintenance* (PM).

---

## 🚀 Fitur Utama

* **📊 Live KPI & Power Health Status:** Ringkasan visual status site (Normal, Warning, Critical) dengan *doughnut chart* dan estimasi masa cadang baterai (*backup countdown*).
* **☁️ Multi-User Real-time Sync:** Terintegrasi langsung dengan Firebase Realtime Database. Setiap pembaruan atau impor data tersinkronisasi secara otomatis di seluruh perangkat tim.
* **📂 Fuzzy Header Excel/CSV Auto-Mapper:** Engine impor cerdas yang mampu mengenali variasi nama kolom Excel secara otomatis untuk:
  * Master Database Site Power
  * Raw Log Query Alarm Huawei NMS (NCE / U2000)
  * Jadwal & Checklist Preventive Maintenance (PM)
* **🛠️ 2nd Level Maintenance Support:** Manajemen eskalasi gangguan dan koordinasi pemulihan site bersama teknisi CME / FOP lapangan.
* **🔐 Persistent Auth Session:** Akses portal terproteksi dengan sesi login yang tersimpan di browser (`localStorage`).

---

## 🔑 Default Kredensial Akses

| Parameter | Nilai Default |
| :--- | :--- |
| **Username** | `xxxx` |
| **Password** | `xxxx` |

---

## 🛠️ Stack Teknologi

* **Frontend:** HTML5, Tailwind CSS, JavaScript (Vanilla ES6)
* **Icon Set:** Phosphor Icons
* **Charts Engine:** Chart.js 4.4
* **Excel Engine:** SheetJS (`xlsx.full.min.js`)
* **Cloud Database:** Firebase Realtime Database (Google Cloud)
* **Hosting:** GitHub Pages

---

## 📋 Struktur Data Impor (Excel / CSV)

Engine web mendukung pembacaan fleksibel untuk nama kolom berikut:

1. **Master Site:** `Site ID`, `Site Name`, `Cluster`, `PLN`, `Genset`, `Rectifier`, `Battery`, `Health Score`.
2. **NMS Log Feed:** `Site ID` / `NE Name`, `Alarm Name`, `Severity`.
3. **PM Schedule:** `Site ID`, `Tanggal/Jadwal`, `PIC/Teknisi`, `Status`, `Scope/Checklist`.

---

## ⚙️ Cara Menjalankan

1. Unggah file `index.html` ke repositori GitHub Anda.
2. Masuk ke **Settings** > **Pages**.
3. Pilih branch `main` pada menu **Branch** dan klik **Save**.
4. Akses tautan publik yang dihasilkan oleh GitHub Pages.

---

*Private Intranet Portal • Developed for SME Power Operations MKU / Huawei Project.*
