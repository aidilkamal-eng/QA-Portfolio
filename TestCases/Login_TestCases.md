# Test Case untuk fitur Login

## HLTB_LOGIN_001
**Skenario:** Login dengan kredensial valid  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Akun user terdaftar dan berstatus aktif  
**Langkah Pengujian:**
1. Buka Website
2. Klik "Login"
3. Masukkan data valid Username dan password
4. Selesaikan Captcha
5. Klik "Login"

**Data Uji:** (Menggunakan data pribadi)  
**Hasil yang Diharapkan:** Login berhasil, dialihkan ke halaman profil, dan session aktif  
**Hasil Aktual:** Berhasil login dan diarahkan ke halaman profil  
**Status:** Pass  
**Catatan:** Data pribadi digunakan karena akan dipakai terus  


## HLTB_LOGIN_002
**Skenario:** Login dengan akun yang belum terdaftar  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:**  
- Pengguna berada di halaman login
- Akun belum terdaftar di sistem sebelumnya

**Langkah Pengujian:**  
1. Masukkan data invalid Username dan password
2. Selesaikan Captcha
3. Klik "Login"

**Data Uji:**  
Username: 67Warrior123  
Password: Chungus12345  

**Hasil yang Diharapkan:** Login gagal dan muncul pesan error bahwa akun tidak ditemukan  
**Hasil Aktual:** Pesan error muncul "Invalid Credentials!"  
**Status:** Pass  
**Catatan:** Pesan error masih bersifat umum dan tidak menjelaskan apakah kesalahan pada username atau password. Direkomendasikan evaluasi dari sisi UX dan keamanan.  


## HLTB_LOGIN_003
**Skenario:** Login dengan password salah  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:**  
- Pengguna berada di halaman login
- Username terdaftar di sistem sebelumnya

**Langkah Pengujian:**  
1. Masukkan data valid Username dan invalid password
2. Selesaikan Captcha
3. Klik "Login"

**Data Uji:**  
Username: steelcharmer (valid)  
Password: Chungus12345 (invalid)  

**Hasil yang Diharapkan:** Login gagal dan muncul pesan error bahwa password salah  
**Hasil Aktual:** Pesan error muncul "Invalid Credentials!"  
**Status:** Pass  
**Catatan:** Pesan error masih bersifat umum dan tidak menjelaskan apakah kesalahan pada username atau password. Direkomendasikan evaluasi dari sisi UX dan keamanan.


## HLTB_LOGIN_004
**Skenario:** Login tanpa mencentang captcha  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:**  
- Pengguna berada di halaman login
- Akun terdaftar di sistem sebelumnya

**Langkah Pengujian:**  
1. Masukkan data valid Username password
2. Klik "Login"

**Data Uji:** (Menggunakan data pribadi)  
**Hasil yang Diharapkan:** Login gagal dan muncul pesan error untuk melakukan verifikasi captcha terlebih dahulu  
**Hasil Aktual:** Pesan error muncul "Invalid CAPTCHA."  
**Status:** Pass  
**Catatan:** 


## HLTB_LOGIN_005
**Skenario:** Login dengan kolom username kosong  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman login  
**Langkah Pengujian:**  
1. Masukkan data valid password
2. Selesaikan Captcha
3. Klik "Login"

**Data Uji:**  
Password: Chungus12345  

**Hasil yang Diharapkan:** Login gagal dan muncul pesan error untuk mengisi username  
**Hasil Aktual:** Pesan error muncul "Invalid Username, try again!"  
**Status:** Pass  
**Catatan:**  


## HLTB_LOGIN_006
**Skenario:** Login dengan kolom password kosong  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman login  
**Langkah Pengujian:**  
1. Masukkan data valid username
2. Selesaikan Captcha
3. Klik "Login"

**Data Uji:**  
Username: steelcharmer    

**Hasil yang Diharapkan:** Login gagal dan muncul pesan error untuk mengisi password  
**Hasil Aktual:** Pesan error muncul "You forgot your secret password!"  
**Status:** Pass  
**Catatan:**  


## HLTB_LOGIN_006
**Skenario:** Login dengan kolom password kosong  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman login  
**Langkah Pengujian:**  
1. Masukkan data valid username
2. Selesaikan Captcha
3. Klik "Login"

**Data Uji:**  
Username: steelcharmer    

**Hasil yang Diharapkan:** Login gagal dan muncul pesan error untuk mengisi password  
**Hasil Aktual:** Pesan error muncul "You forgot your secret password!"  
**Status:** Pass  
**Catatan:**  


## HLTB_LOGIN_007
**Skenario:** Login dengan username mengandung karakter khusus (@,#,$, dll)  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman login  
**Langkah Pengujian:**  
1. Masukkan data invalid username dan data valid password
2. Selesaikan Captcha
3. Klik "Login"

**Data Uji:**  
Username: steel#charmer   
Password: Chungus12345

**Hasil yang Diharapkan:** Login gagal dan muncul pesan error format username salah  
**Hasil Aktual:** Pesan error muncul "Invalid Username, try again!"  
**Status:** Pass  
**Catatan:**  Format username yang digunakan hanya bisa huruf, angka, dan garis bawah dengan 3-20 karakter.  


## HLTB_LOGIN_008
**Skenario:** Login dengan username kurang dari minimum karakter  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman login  
**Langkah Pengujian:**  
1. Masukkan data invalid username dan data valid password
2. Selesaikan Captcha
3. Klik "Login"

**Data Uji:**  
Username: LA   
Password: Chungus12345

**Hasil yang Diharapkan:** Login gagal dan muncul pesan error format username salah  
**Hasil Aktual:** Pesan error muncul "Invalid Username, try again!"  
**Status:** Pass  
**Catatan:**  Format username yang digunakan hanya bisa huruf, angka, dan garis bawah dengan 3-20 karakter. 


## HLTB_LOGIN_009
**Skenario:** Login dengan username kurang dari minimum karakter  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman login  
**Langkah Pengujian:**  
1. Masukkan data invalid username dan data valid password
2. Selesaikan Captcha
3. Klik "Login"

**Data Uji:**  
Username: LA   
Password: Chungus12345

**Hasil yang Diharapkan:** Login gagal dan muncul pesan error format username salah  
**Hasil Aktual:** Pesan error muncul "Invalid Username, try again!"  
**Status:** Pass  
**Catatan:**  Format username yang digunakan hanya bisa huruf, angka, dan garis bawah dengan 3-20 karakter. 
