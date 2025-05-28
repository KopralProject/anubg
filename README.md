# DOR Bot Telegram

Bot Telegram untuk DOR yang sudah siap digunakan di VPS.

## File yang Diperlukan
- `autoftbot` 
- `.env` (file konfigurasi)

## Cara Deploy ke VPS

1. **Upload File ke VPS**
   ```bash
   # Buat folder baru di VPS
   mkdir dor-bot
   cd dor-bot

   # Upload kedua file ke folder tersebut
   # - autoftbot
   # - .env
   ```

2. **Jalankan Bot**
   ```bash
   # Berikan permission execute
   chmod +x autoftbot

   # Jalankan bot
   ./autoftbot
   ```

3. **Menjalankan di Background (Rekomendasi)**
   ```bash
   # Menggunakan screen (direkomendasikan)
   screen -S dor-bot
   ./autoftbot
   # Tekan Ctrl+A+D untuk keluar dari screen
   
   # Untuk melihat screen yang berjalan
   screen -ls
   
   # Untuk kembali ke screen
   screen -r dor-bot
   ```

## Troubleshooting

1. **Error: Permission Denied**
   ```bash
   chmod +x autoftbot
   ```

2. **Error: Cannot find .env**
   - Pastikan file `.env` ada di folder yang sama dengan executable
   - Periksa permission file `.env`

## Catatan Penting
- File `.env` harus disiapkan secara terpisah
- Backup file `.env` di tempat yang aman
- Jangan share file `.env` ke publik

## Support
Jika mengalami masalah, silakan hubungi developer untuk bantuan lebih lanjut. 