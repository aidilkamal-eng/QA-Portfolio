# Test Case untuk fitur Sign Up

## HLTB_SIGNUP_001
**Skenario:** Verifikasi pendaftaran dengan kredensial valid  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna belum pernah mendaftarkan akun sebelumnya  
**Langkah Pengujian:**
1. Buka Website
2. Klik "Join"
3. Masukkan data valid Email, Username, Password, dan Verify Password
4. Selesaikan Captcha
5. Klik "Create Account"

**Data Uji:** (Menggunakan data pribadi)  
**Hasil yang Diharapkan:** Akun berhasil didaftarkan  
**Hasil Aktual:** Akun berhasil dibuat dan diarahkan ke halaman profil  
**Status:** Pass  
**Catatan:** Data pribadi digunakan karena akan dipakai terus  


## HLTB_SIGNUP_002
**Skenario:** Verifikasi pendaftaran dengan email tidak valid  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman pendaftaran  
**Langkah Pengujian:**
1. Masukkan data invalid Email, Username, Password, dan Verify Password
2. Selesaikan Captcha
3. Klik "Create Account"

**Data Uji:**  
Email: chungus@google.com7  
Username:Chungus156  
Password: chungus12345  
verify Password: chungus 12345

**Hasil yang Diharapkan:** Akun tidak dibuat dan muncul pesan kesalahan format email  
**Hasil Aktual:** Muncul peringatan bar merah: “Email address is not valid”  
**Status:** Pass  
**Catatan:** 


## HLTB_SIGNUP_003
**Skenario:** Verifikasi pendaftaran dengan konfirmasi password tidak cocok  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman pendaftaran  
**Langkah Pengujian:**
1. Masukkan data invalid Email, Username, Password, dan Verify Password
2. Selesaikan Captcha
3. Klik "Create Account"

**Data Uji:**  
Email: chungus@gmail.com  
Username:Chungus156  
Password: chungus12345  
verify Password: chungus 122345

**Hasil yang Diharapkan:** Akun tidak dibuat dan muncul pesan error ketidaksesuaian password  
**Hasil Aktual:** Muncul peringatan: “Your passwords do not match”  
**Status:** Pass  
**Catatan:**


## HLTB_SIGNUP_004
**Skenario:** Verifikasi pendaftaran tanpa mencentang CAPTCHA  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman pendaftaran  
**Langkah Pengujian:**
1. Masukkan data Email, Username, Password, dan Verify Password
2. Klik "Create Account"

**Data Uji:**  
Email: chungus@gmail.com  
Username:Chungus156  
Password: chungus12345  
verify Password: chungus 12345  

**Hasil yang Diharapkan:** Akun tidak dibuat dan muncul error CAPTCHA  
**Hasil Aktual:** Muncul pesan “Invalid CAPTCHA”  
**Status:** Pass  
**Catatan:**

