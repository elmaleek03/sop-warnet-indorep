# Jobdesk OP Warnet - INDOREP NET

## 1. Pelayanan Transaksi
- Menerima pembayaran billing warnet (Cash & QRIS)
- Menerima pembayaran produk (minuman dingin) (Cash & QRIS)

## 2. Kebersihan & Kerapian
Dilakukan segera setelah customer selesai menggunakan PC:
- Merapikan monitor, PC, keyboard, mousepad, mouse, headset
- Mengelap meja
- Menata kembali tisu ke tempat asal
- Antarkan alat makan ke lt 1 jika luang

## 3. Pemeliharaan Sistem
- Menjalankan update game setiap hari pukul 05:00 WIB (lihat SOP Update Game)

# SOP OP Warnet - Update Game INDOREP NET


## Priority List

### 🔴 [High Priority] — Check Daily (1x/day)
- Valorant (Riot)
- League of Legends (Riot)
- Point Blank
- DOTA 2 (Steam)
- Counter-Strike 2 (Steam)
- PUBG (Steam)

### 🟠 [Medium Priority] — Check Weekly (1x/week)
- Genshin Impact (HoYoLauncher)
- Honkai Star Rail (HoYoLauncher)
- Honkai Impact (HoYoLauncher)
- ZZZ (Hoyo Launcher)
- Wuthering Waves
- The Finals (Steam)
- Apex Legends (Steam)
- Delta Force (Steam)
- AyoDance

### 🟢 [Low Priority] — Check Biweekly or Less (1x/2 weeks or more)
- Roblox
- FiveM
- GTA V Legacy (Steam)
- Growtopia (Steam)
- Among Us (Steam)
- Buckshot Roulette (Steam)
- Fall Guys (Steam)
- Phasmophobia (Steam)

---

## 1. PC Operator Side

### 🔴 High Priority
- Buka Riot Client, update semua game high priority
- Buka PBLauncher, update Point Blank
- Buka Steam, update semua game high priority
- Cek Syncthing PC di [http://localhost:8384/](http://localhost:8384/), pastikan sudah up-to-date semua
- Cek progress ke PC client (link internal / progress monitoring tools)

### 🟠 Medium Priority
- Buka Steam, update semua game medium priority
- Navigasi ke `D:\Apps\AyoDance`, update AyoDance
- Navigasi ke `D:\Apps\HoyoLauncher` update ke-4
- Buka Steam, update semua game medium priority

### 🟢 Low Priority
- Navigasi ke `D:\Apps`, buka seluruh launcher
- Update launcher & game
- Buka Steam, update semua game low priority

> ⚠️ **SEMUA GAME DI PC OPERATOR HARUS SELESAI DIUPDATE SEBELUM LANJUT KE TAHAP 2**

---

## 2. PC Client Side (Update pada PC yang tidak digunakan)

- Pause Syncthing NAS (RAJA-GAME) dari [http://192.168.5.61:8384/](http://192.168.5.61:8384/) menuju PC Client tujuan
![Pause Syncthing menuju PC Client](iamges/pause.png)
- Buka billing, klik kanan pada PC Client > Manage > Enter Maintenance Mode / Exit billing PC Client yang mau diupdate
- Restart PC Client lewat **Reboot Restore RX**
- **Turn Off Protection** di PC Client
- Pastikan PC client sudah selesai turn off protection dengan tidak menampilkan loading progress bar!
- Restore Baseline menjadi berwarna abu setelah disabled"
- ![RX Protection Off!](images/rx-off.png)
- ![RX Protection ON!](images/rx-on.png)
- Buka Kembali Syncthing NAS di [http://192.168.5.61:8384/](http://192.168.5.61:8384/), resume update dan pantau progress update client
- Pastikan folder `apps`, `Riot`, dan `steamapps` sudah up-to-date semua atau 99% dengan sisa file size kecil
  
> ⚠️ **JANGAN PAKAI PC SAAT KONDISI PROTECTION TURN OFF!**  
> ⚠️ **JANGAN PAKAI PC SAAT KONDISI PROTECTION TURN OFF!**

- Setelah update selesai, di Syncthing NAS tekan pause pada PC Client 
- Buka Reboot Restore RX, Turn On Protection pada PC Client (PC akan restart otomatis)
- ✅ Done!

---

## 3. Virtual Disk Side (Game non-steam)

- Buka `INDOREP-GAME (P:)`, jalankan `disk2vhd.exe`
- Jangan ubah apapun
- Centang hanya volume `D:` lalu tekan **Create**
- Tunggu hingga proses selesai
- Rename DESKTOP-xxxx.vhdx menjadi OLD-DESKTOP-xxxx.vhdx
- Rename GAME.vhdx menjadi DESKTOP-xxxx.vhdx
- ✅ Done!
