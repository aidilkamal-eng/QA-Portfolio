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
**Skenario:** Login dengan username melebihi maksimum karakter  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman login  
**Langkah Pengujian:**  
1. Masukkan data invalid username dan data valid password
2. Selesaikan Captcha
3. Klik "Login"

**Data Uji:**  
Username: SelamatMalamPemirsa77   
Password: Chungus12345

**Hasil yang Diharapkan:** Login gagal dan muncul pesan error format username salah  
**Hasil Aktual:** Pesan error muncul "Invalid Username, try again!"  
**Status:** Pass  
**Catatan:**  Format username yang digunakan hanya bisa huruf, angka, dan garis bawah dengan 3-20 karakter. 


## HLTB_LOGIN_010
**Skenario:** Login dengan username mengandung spasi  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman login  
**Langkah Pengujian:**  
1. Masukkan data invalid username dan data valid password
2. Selesaikan Captcha
3. Klik "Login"

**Data Uji:**  
Username: steel charmer   
Password: Chungus12345

**Hasil yang Diharapkan:** Login gagal dan muncul pesan error format username salah  
**Hasil Aktual:** Pesan error muncul "Invalid Username, try again!"  
**Status:** Pass  
**Catatan:**  Format username yang digunakan hanya bisa huruf, angka, dan garis bawah dengan 3-20 karakter.


## HLTB_LOGIN_011
**Skenario:** Login dengan password kurang dari minimum karakter  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman login  
**Langkah Pengujian:**  
1. Masukkan data valid username dan data invalid password
2. Selesaikan Captcha
3. Klik "Login"

**Data Uji:**  
Username: steelcharmer   
Password: Ch4ngus

**Hasil yang Diharapkan:** Login gagal dan muncul pesan error format password salah  
**Hasil Aktual:** Pesan error muncul "Invalid Credentials!"  
**Status:** Pass  
**Catatan:**  Format password akun harus terdiri dari 8-128 karakter dan setidaknya memiliki satu huruf kapital dan satu nomor.


## HLTB_LOGIN_012
**Skenario:** Login dengan password lebih dari maksimum karakter  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman login  
**Langkah Pengujian:**  
1. Masukkan data valid username dan data invalid password
2. Selesaikan Captcha
3. Klik "Login"

**Data Uji:**  
Username: steelcharmer   
Password: Ch4ngusMastinGoodLifeIsAlsoGo0dWhatAboutYou?ImStillHereTryingToTestThePasswordFormSoThatICanFind0utIfItsWorkingAsExpectedOrNotWishMeLuck

**Hasil yang Diharapkan:** Login gagal dan muncul pesan error format password salah  
**Hasil Aktual:** Pesan error muncul "Invalid Credentials!"  
**Status:** Pass  
**Catatan:**  Format password akun harus terdiri dari 8-128 karakter dan setidaknya memiliki satu huruf kapital dan satu nomor.


## HLTB_LOGIN_013
**Skenario:** Login dengan password tanpa memiliki setidaknya satu huruf kapital  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman login  
**Langkah Pengujian:**  
1. Masukkan data valid username dan data invalid password
2. Selesaikan Captcha
3. Klik "Login"

**Data Uji:**  
Username: steelcharmer   
Password: chungus12345

**Hasil yang Diharapkan:** Login gagal dan muncul pesan error format password salah  
**Hasil Aktual:** Pesan error muncul "Invalid Credentials!"  
**Status:** Pass  
**Catatan:**  Format password akun harus terdiri dari 8-128 karakter dan setidaknya memiliki satu huruf kapital dan satu nomor.


## HLTB_LOGIN_014
**Skenario:** Login dengan password tanpa memiliki setidaknya satu nomor  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman login  
**Langkah Pengujian:**  
1. Masukkan data valid username dan data invalid password
2. Selesaikan Captcha
3. Klik "Login"

**Data Uji:**  
Username: steelcharmer   
Password: ChungusIsOkay

**Hasil yang Diharapkan:** Login gagal dan muncul pesan error format password salah  
**Hasil Aktual:** Pesan error muncul "Invalid Credentials!"  
**Status:** Pass  
**Catatan:**  Format password akun harus terdiri dari 8-128 karakter dan setidaknya memiliki satu huruf kapital dan satu nomor.


## HLTB_LOGIN_015
**Skenario:** Klik tombol "Sign Up!"  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman login  
**Langkah Pengujian:**  
1. Klik "Sign Up!"

**Data Uji:**  
**Hasil yang Diharapkan:** Sistem melakukan redirect ke halaman sign up  
**Hasil Aktual:** Halaman redirect ke halaman member sign up  
**Status:** Pass  
**Catatan:**  


## HLTB_LOGIN_016
**Skenario:** Klik tombol "Forgot Password?"  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman login  
**Langkah Pengujian:**  
1. Klik "Forgot Password?"

**Data Uji:**  
**Hasil yang Diharapkan:** Sistem melakukan redirect ke halaman account recovery  
**Hasil Aktual:** Halaman redirect ke halaman forgotten password  
**Status:** Pass  
**Catatan:**  


## HLTB_LOGIN_017
**Skenario:** Klik tombol "Login with IGN"  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman login  
**Langkah Pengujian:**  
1. Klik "Login with IGN"

**Data Uji:**  
**Hasil yang Diharapkan:** Sistem melakukan redirect ke halaman autentikasi resmi IGN dan URL berubah ke domain IGN.  
**Hasil Aktual:** Halaman redirect ke halaman login IGN  
**Status:** Pass  
**Catatan:** Rekomendasi UI/UX: Warna tombol disarankan menggunakan biru agar tidak menimbulkan persepsi negatif atau disalahartikan.  


## HLTB_LOGIN_018
**Skenario:** Klik link "Contact Support"  
**Prioritas:** Menengah  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman login  
**Langkah Pengujian:**  
1. Klik "Contact Support"

**Data Uji:**  
**Hasil yang Diharapkan:** Sistem melakukan redirect ke halaman costumer support  
**Hasil Aktual:** Halaman redirect ke halaman site feedback  
**Status:** Pass  
**Catatan:**  


## HLTB_LOGIN_019
**Skenario:** Klik link "Subscribe to IGN Plus for an Ad-Free Experience!"  
**Prioritas:** Rendah  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman login  
**Langkah Pengujian:**  
1. Klik "Subscribe to IGN Plus for an Ad-Free Experience!"

**Data Uji:**  
**Hasil yang Diharapkan:** Sistem melakukan redirect ke halaman subscription plan IGN  
**Hasil Aktual:** Halaman redirect ke halaman subscription plan IGN  
**Status:** Pass  
**Catatan:**  Rekomendasi UI/UX: Warna teks disarankan menggunakan biru agar tidak menimbulkan persepsi negatif atau disalahartikan.





