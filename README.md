# GTA SA Open Limit Adjuster Configuration for SAMP

Konfigurasi ini dibuat untuk digunakan dengan **Open Limit Adjuster**, sebuah mod penting yang memungkinkan kita untuk **menghapus batasan teknis internal** dalam game *GTA San Andreas*, terutama saat bermain **SAMP (San Andreas Multiplayer)**.

Saya membagikan file ini ke repository GitHub ini karena dua alasan:
1. Agar dapat membantu orang lain yang juga ingin mengoptimalkan performa SAMP mereka.
2. Sebagai pengingat pribadi jika suatu saat saya perlu mengatur ulang konfigurasi ini di sistem baru.

---

## Apa Itu Open Limit Adjuster?

[Open Limit Adjuster](https://github.com/GTAmodding/III.VC.SA.LimitAdjuster) adalah mod yang memungkinkan kita untuk:
- Meningkatkan jumlah kendaraan, objek, ped, dan model yang bisa dimuat game tanpa crash.
- Mengatasi masalah seperti **ID limit** atau **object streaming flicker**.
- Menyesuaikan penggunaan RAM dan frame limit agar performa lebih stabil.

Mod ini sangat penting untuk kamu yang:
- Bermain di server SAMP dengan **mapping berat atau banyak custom object**.
- Menggunakan banyak **mod kendaraan, skin, atau texture**.
- Ingin mendorong performa maksimal tanpa takut game crash atau lag.

---

## Penjelasan Parameter Penting di `.ini`

Berikut beberapa parameter utama yang telah dioptimalkan:

| Parameter                    | Fungsi                                                                 |
|-----------------------------|------------------------------------------------------------------------|
| `Peds`, `Vehicles`, `Objects`     | Jumlah maksimal entity seperti ped, mobil, dan objek aktif di dunia.       |
| `ColModel`                  | Jumlah maksimal model collision yang bisa dimuat.                     |
| `StreamingObjectInstancesList` | Menambah jumlah objek yang bisa terlihat sekaligus tanpa flickering.     |
| `MemoryAvailable`           | Jumlah RAM (MB atau %) yang boleh digunakan untuk streaming data.     |
| `FrameLimit`                | Mengatur batas maksimal FPS (30 = default, 90 = gameplay mulus asal monitornya support > 60FPS).      |
| `AtomicModels`, `VehicleModels`, `PedModels` | Jumlah definisi model yang bisa dimuat, penting untuk modding.      |
| `EntitiesPerIpl`, `EntityIpl`     | Menghapus batasan jumlah objek yang dimuat dari file `.ipl`.           |

> Semua nilai telah dioptimalkan berdasarkan sistem saya: **RAM 16GB, GTX 1650, i5-12500H**. Jika sistem kamu berbeda, kamu boleh menyesuaikan sesuai kebutuhan.

---

## Rekomendasi Sistem

Konfigurasi ini diuji di sistem berikut:
- **RAM**: 16 GB  
- **GPU**: NVIDIA GTX 1650 Laptop  
- **CPU**: Intel Core i5-12500H  
- **Game**: GTA San Andreas 1.0 US + SAMP 0.3DL 
- **Mod Tambahan**: Colormod, Improved Vehicle Feature Mod (ImVehFT) (base and vehicles), HUD, Vehicle Wheels, Timecyc, etc

---

## Cara Menggunakan

1. Unduh dan pasang [Open Limit Adjuster](https://github.com/GTAmodding/III.VC.SA.LimitAdjuster/releases) (.asi + .ini).
2. Ganti isi file `.ini` dengan konfigurasi ini.
3. Jalankan game seperti biasa. Untuk melihat perubahan efeknya, coba masuk ke daerah padat objek (misalnya base mapping berat).

---
