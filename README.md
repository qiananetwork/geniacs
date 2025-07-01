# INSTALL GENIEACS OTOMATIS (Versi Qiana Network)

Installer otomatis GenieACS untuk Ubuntu Server 20.04+, cocok untuk deployment cepat dan terstandar.

---

## 📥 Langkah Instalasi

### 1. Install Git dan Curl
```bash
sudo apt install git curl -y
```

### 2. Clone Repository Qiana Network
```bash
git clone https://github.com/qiananetwork/genieacs
cd genieacs
```

### 3. Beri Hak Akses Eksekusi
```bash
chmod +x install.sh
```

### 4. Jalankan Instalasi
```bash
./install.sh
```

---

## ⚠️ CATATAN PENTING SEBELUM UPDATE

Instalasi ini akan **menghapus konfigurasi lama** dan menggantinya dengan konfigurasi baru yang bersih.

Yang akan diperbarui:
- Admin → Preset  
- Admin → Provisions  
- Admin → Virtual Parameters  
- Admin → Config

> **Device, user, permission tidak akan terhapus.**  
> Jika sebelumnya ada konfigurasi error, akan diperbaiki otomatis.

### 🛡️ Backup Sebelum Update
Jika Anda memiliki konfigurasi custom buatan sendiri, **silakan backup terlebih dahulu**, lalu restore manual setelah update.

---

## ♻️ Cara Restore Konfigurasi Lama

```bash
cd
sudo mongorestore --db=genieacs --drop genieacs-backup/genieacs
```

---

## 🤝 Kontribusi

Kontribusi sangat terbuka!  
Silakan pull request atau laporkan masalah melalui:

📞 WhatsApp: [Klik di sini](https://wa.me/6281231300041)
