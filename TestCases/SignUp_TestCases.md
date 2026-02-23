# Test Case untuk fitur Sign Up

## HLTB_TC_SIGNUP_001
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


## HLTB_TC_SIGNUP_002
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


## HLTB_TC_SIGNUP_003
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


## HLTB_TC_SIGNUP_004
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


## HLTB_TC_SIGNUP_005
**Skenario:** Verifikasi pendaftaran dengan password tanpa huruf kapital  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman pendaftaran  
**Langkah Pengujian:**
1. Masukkan data email, username, dan password dengan format tidak valid
2. Selesaikan Captcha
3. Klik "Create Account"

**Data Uji:**  
Email: chungus@gmail.com  
Username: Chungus156  
Password: chungus12345  
Verify Password: chungus12345  

**Hasil yang Diharapkan:** Akun tidak dibuat dan sistem menampilkan pesan error bahwa password harus terdiri dari 8–128 karakter serta mengandung minimal satu huruf kapital dan satu angka.  
**Hasil Aktual:** Muncul pesan error "Password must be 8-128 characters and include at least one uppercase letter and one number."  
**Status:** Pass  
**Catatan:** Format password akun harus terdiri dari 8-128 karakter dan setidaknya memiliki satu huruf kapital dan satu nomor


## HLTB_TC_SIGNUP_006
**Skenario:** Verifikasi pendaftaran dengan email yang sudah digunakan  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:**  
- Pengguna berada di halaman pendaftaran
- Email "aidilkamal91@gmail.com" sudah terdaftar pada sistem sebelumnya

**Langkah Pengujian:**
1. Masukkan data email, username, dan password
2. Selesaikan Captcha
3. Klik "Create Account"

**Data Uji:**  
Email: aidilkamal91@gmail.com  
Username: Chungus153  
Password: Chungus12345  
Verify Password: Chungus12345  

**Hasil yang Diharapkan:** Akun tidak dibuat dan sistem menampilkan pesan error bahwa email sudah digunakan sebelumnya.  
**Hasil Aktual:** Akun baru terbuat  
**Status:** Fail  
**Catatan:** 


## HLTB_TC_SIGNUP_007
**Skenario:** Verifikasi pendaftaran dengan username yang sudah digunakan  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:**  
- Pengguna berada di halaman pendaftaran
- Username "steelcharmer" sudah terdaftar pada sistem sebelumnya

**Langkah Pengujian:**
1. Masukkan data email, username, dan password
2. Selesaikan Captcha
3. Klik "Create Account"

**Data Uji:**  
Email: aidilkamal91@gmail.com  
Username: steelcharmer  
Password: Chungus12345  
Verify Password: Chungus12345  

**Hasil yang Diharapkan:** Akun tidak dibuat dan sistem menampilkan pesan error bahwa username sudah terdaftar di sistem.  
**Hasil Aktual:** Muncul pesan error "Sorry that username already exists."  
**Status:** Pass  
**Catatan:** 


## HLTB_TC_SIGNUP_008
**Skenario:** Verifikasi pendaftaran dengan username menggunakan spasi
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman pendaftaran  
**Langkah Pengujian:**
1. Masukkan data email, username, dan password dengan format invalid
2. Selesaikan Captcha
3. Klik "Create Account"

**Data Uji:**  
Email: aidilkamal91@gmail.com  
Username: steel charmer  
Password: Chungus12345  
Verify Password: Chungus12345  

**Hasil yang Diharapkan:** Akun tidak dibuat dan sistem menampilkan pesan error bahwa format username tidak valid.  
**Hasil Aktual:** Muncul pesan error "Username may only have Numbers, Letters and _ allowed. 3-20 Characters."  
**Status:** Pass  
**Catatan:** Format username yang digunakan hanya bisa huruf, angka, dan garis bawah dengan 3-20 karakter.


## HLTB_TC_SIGNUP_009
**Skenario:** Verifikasi pendaftaran dengan karakter username tidak cukup
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman pendaftaran  
**Langkah Pengujian:**
1. Masukkan data email, username, dan password dengan format invalid
2. Selesaikan Captcha
3. Klik "Create Account"

**Data Uji:**  
Email: aidilkamal91@gmail.com  
Username: LA  
Password: Chungus12345  
Verify Password: Chungus12345  

**Hasil yang Diharapkan:** Akun tidak dibuat dan sistem menampilkan pesan error bahwa format username tidak valid.  
**Hasil Aktual:** Muncul pesan error "Username may only have Numbers, Letters and _ allowed. 3-20 Characters."  
**Status:** Pass  
**Catatan:** Format username yang digunakan hanya bisa huruf, angka, dan garis bawah dengan 3-20 karakter.


## HLTB_TC_SIGNUP_010
**Skenario:** Verifikasi pendaftaran dengan karakter password tidak cukup  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman pendaftaran  
**Langkah Pengujian:**
1. Masukkan data email, username, dan password dengan format tidak valid
2. Selesaikan Captcha
3. Klik "Create Account"

**Data Uji:**  
Email: aidilkamal91@gmail.com  
Username: Chungus156  
Password: Chung4s  
Verify Password: Chung4s  

**Hasil yang Diharapkan:** Akun tidak dibuat dan sistem menampilkan pesan error bahwa password harus terdiri dari 8–128 karakter serta mengandung minimal satu huruf kapital dan satu angka.  
**Hasil Aktual:** Muncul pesan error "Password must be 8-128 characters and include at least one uppercase letter and one number."  
**Status:** Pass  
**Catatan:** Format password akun harus terdiri dari 8-128 karakter dan setidaknya memiliki satu huruf kapital dan satu nomor


## HLTB_TC_SIGNUP_011
**Skenario:** Verifikasi pendaftaran dengan kolom email kosong  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman pendaftaran  
**Langkah Pengujian:**
1. Masukkan data username dan password
2. Selesaikan Captcha
3. Klik "Create Account"

**Data Uji:**   
Email: (kosong)  
Username: Chungus156  
Password: Chungus12345  
Verify Password: Chungus12345  

**Hasil yang Diharapkan:** Akun tidak dibuat dan sistem menampilkan pesan error bahwa kolom email perlu di isi  
**Hasil Aktual:** Muncul pesan error "Email Address cannot be empty."  
**Status:** Pass  
**Catatan:**  


## HLTB_TC_SIGNUP_012
**Skenario:** Verifikasi pendaftaran dengan kolom username kosong  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman pendaftaran  
**Langkah Pengujian:**
1. Masukkan data email dan password
2. Selesaikan Captcha
3. Klik "Create Account"

**Data Uji:**   
Email: aidilkamal91@gmail.com  
Username: (kosong)  
Password: Chungus12345  
Verify Password: Chungus12345  

**Hasil yang Diharapkan:** Akun tidak dibuat dan sistem menampilkan pesan error bahwa kolom username perlu di isi  
**Hasil Aktual:** Muncul pesan error "Username cannot be empty."  
**Status:** Pass  
**Catatan:**  


## HLTB_TC_SIGNUP_013
**Skenario:** Verifikasi pendaftaran dengan kolom password kosong  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman pendaftaran  
**Langkah Pengujian:**
1. Masukkan data email dan username
2. Selesaikan Captcha
3. Klik "Create Account"

**Data Uji:**   
Email: aidilkamal91@gmail.com  
Username: Chungus156  
Password: (kosong)  
Verify Password: Chungus12345  

**Hasil yang Diharapkan:** Akun tidak dibuat dan sistem menampilkan pesan error bahwa kolom password perlu di isi  
**Hasil Aktual:** Muncul pesan error "Password cannot be empty."  
**Status:** Pass  
**Catatan:**  


## HLTB_TC_SIGNUP_014
**Skenario:** Verifikasi pendaftaran dengan kolom verify password kosong  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman pendaftaran  
**Langkah Pengujian:**
1. Masukkan data email, username, dan password tanpa verify password
2. Selesaikan Captcha
3. Klik "Create Account"

**Data Uji:**   
Email: aidilkamal91@gmail.com  
Username: Chungus156  
Password: Chungus12345  
Verify Password: (kosong)  

**Hasil yang Diharapkan:** Akun tidak dibuat dan sistem menampilkan pesan error bahwa kolom verify password perlu di isi  
**Hasil Aktual:** Muncul pesan error "Your passwords do not match."  
**Status:** Pass  
**Catatan:**  Rekomendasi: pesan error yang ditampilkan adalah "Verify password cannot be empty"


## HLTB_TC_SIGNUP_015
**Skenario:** Verifikasi pendaftaran dengan karakter username lebih dari batas maksimal  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman pendaftaran  
**Langkah Pengujian:**
1. Masukkan data email, username, dan password dengan format invalid
2. Selesaikan Captcha
3. Klik "Create Account"

**Data Uji:**  
Email: aidilkamal91@gmail.com  
Username: SelamatMalamPemirsa77  
Password: Chungus12345  
Verify Password: Chungus12345  

**Hasil yang Diharapkan:** Akun tidak dibuat dan sistem menampilkan pesan error bahwa format username tidak valid.  
**Hasil Aktual:** Muncul pesan error "Username may only have Numbers, Letters and _ allowed. 3-20 Characters."  
**Status:** Pass  
**Catatan:** Format username yang digunakan hanya bisa huruf, angka, dan garis bawah dengan 3-20 karakter.


## HLTB_TC_SIGNUP_016
**Skenario:** Verifikasi pendaftaran dengan username mengandung karakter khusus (@,#,$, dll)  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman pendaftaran  
**Langkah Pengujian:**
1. Masukkan data email, username, dan password dengan format invalid
2. Selesaikan Captcha
3. Klik "Create Account"

**Data Uji:**  
Email: aidilkamal91@gmail.com  
Username: steel#charmer  
Password: Chungus12345  
Verify Password: Chungus12345  

**Hasil yang Diharapkan:** Akun tidak dibuat dan sistem menampilkan pesan error bahwa format username tidak valid.  
**Hasil Aktual:** Muncul pesan error "Username may only have Numbers, Letters and _ allowed. 3-20 Characters."  
**Status:** Pass  
**Catatan:** Format username yang digunakan hanya bisa huruf, angka, dan garis bawah dengan 3-20 karakter.


## HLTB_TC_SIGNUP_017
**Skenario:** Verifikasi pendaftaran dengan jumlah karakter password melebihi batas maksimum  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman pendaftaran  
**Langkah Pengujian:**
1. Masukkan data email, username, dan password dengan format invalid
2. Selesaikan Captcha
3. Klik "Create Account"

**Data Uji:**  
Email: aidilkamal91@gmail.com  
Username: steelcharmer  
Password: Ch4ngusMastinGoodLifeIsAlsoGo0dWhatAboutYou?ImStillHereTryingToTestThePasswordFormSoThatICanFind0utIfItsWorkingAsExpectedOrNotWishMeLuck  
Verify Password: Ch4ngusMastinGoodLifeIsAlsoGo0dWhatAboutYou?ImStillHereTryingToTestThePasswordFormSoThatICanFind0utIfItsWorkingAsExpectedOrNotWishMeLuck  

**Hasil yang Diharapkan:** Akun tidak dibuat dan sistem menampilkan pesan error bahwa password harus terdiri dari 8–128 karakter serta mengandung minimal satu huruf kapital dan satu angka.  
**Hasil Aktual:** Muncul pesan error "Password must be 8-128 characters and include at least one uppercase letter and one number."  
**Status:** Pass  
**Catatan:** Format password akun harus terdiri dari 8-128 karakter dan setidaknya memiliki satu huruf kapital dan satu nomor


## HLTB_TC_SIGNUP_018
**Skenario:** Verifikasi pendaftaran dengan password tanpa memiliki setidaknya satu nomor  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman pendaftaran  
**Langkah Pengujian:**
1. Masukkan data email, username, dan password dengan format invalid
2. Selesaikan Captcha
3. Klik "Create Account"

**Data Uji:**  
Email: aidilkamal91@gmail.com  
Username: steelcharmer  
Password: ChungusIsOkay  
Verify Password: ChungusIsOkay  

**Hasil yang Diharapkan:** Akun tidak dibuat dan sistem menampilkan pesan error bahwa password harus terdiri dari 8–128 karakter serta mengandung minimal satu huruf kapital dan satu angka.  
**Hasil Aktual:** Muncul pesan error "Password must be 8-128 characters and include at least one uppercase letter and one number."  
**Status:** Pass  
**Catatan:** Format password akun harus terdiri dari 8-128 karakter dan setidaknya memiliki satu huruf kapital dan satu nomor


## HLTB_TC_SIGNUP_019
**Skenario:** Klik link "Terms of Use"  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman pendaftaran  
**Langkah Pengujian:**
1. Klik "Terms of Use"

**Data Uji:**  
**Hasil yang Diharapkan:** Sistem redirect ke halaman Terms of Use  
**Hasil Aktual:** Sistem redirect ke halaman Terms of Use Ziff Davis  
**Status:** Pass  
**Catatan:** 


## HLTB_TC_SIGNUP_020
**Skenario:** Klik link "Privacy Policy"  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman pendaftaran  
**Langkah Pengujian:**
1. Klik "Privacy Policy"

**Data Uji:**  
**Hasil yang Diharapkan:** Sistem redirect ke halaman Privacy policy  
**Hasil Aktual:** Sistem redirect ke halaman Privacy Policy domain IGN  
**Status:** Pass  
**Catatan:** 


## HLTB_TC_SIGNUP_021
**Skenario:** Klik link "Login"  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman pendaftaran  
**Langkah Pengujian:**
1. Klik "Login"

**Data Uji:**  
**Hasil yang Diharapkan:** Sistem redirect ke halaman login  
**Hasil Aktual:** Sistem redirect ke halaman login  
**Status:** Pass  
**Catatan:** 


## HLTB_TC_SIGNUP_021
**Skenario:** Klik link "Contact Support"  
**Prioritas:** Menengah  
**Jenis Tes:** Functional  
**Prasyarat:** Pengguna berada di halaman pendaftaran  
**Langkah Pengujian:**
1. Klik "Contact Support"

**Data Uji:**  
**Hasil yang Diharapkan:** Sistem redirect ke halaman Costumer support  
**Hasil Aktual:** Sistem redirect ke halaman Site Feedback  
**Status:** Pass  
**Catatan:** 


## HLTB_TC_SIGNUP_022
**Skenario:** Navigasi kembali setelah akun berhasil dibuat  
**Prioritas:** Tinggi  
**Jenis Tes:** Functional & Session Management Test  
**Prasyarat:**  
- Akun berhasil dan baru saja dibuat
- Pengguna sudah masuk ke halaman profil

**Langkah Pengujian:**
1. Klik tombol back pada browser

**Data Uji:**  
**Hasil yang Diharapkan:**  
- Sistem mengarahkan pengguna ke halaman Home
- Session tetap aktif

**Hasil Aktual:**  
- Sistem kembali ke halaman Sign Up
- Session tetap aktif

**Status:** Fail  
**Catatan:** Rekomendasi: Sistem sebaiknya mengarahkan pengguna ke halaman Home atau menampilkan peringatan form resubmission untuk menghindari kebingungan pengguna.
