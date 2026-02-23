# HLTB_BUG_LOGIN_001

## Judul
Akun sebelumnya terlogin sendiri dan session aktif jika mengklik tombol "Subscribe to IGN Plus for an Ad-Free Experience!"

## Environment
- Browser: Chrome 140
- OS: Windows 11

## Prasyarat
- Session aktif
- User berada pada halaman profil

## Langkah-langkah untuk Mereproduksi Bug
1. Klik logo profil
2. Klik "Logout"
3. Klik "Login"
4. Klik "Subscribe to IGN Plus for an Ad-Free Experience!"
5. Klik tombol back pada browser

## Hasil yang Diharapkan
1. Sistem redirect ke halaman login
2. Session kosong dalam keadaan tidak ada akun yang ter-login

## Hasil Aktual
1. Sistem redirect ke halaman login
2. Session dari akun yang sudah ter-logout sebelumnya menjadi aktif

## Tingkat Dampak Bug
Tinggi

## Prioritas
Tinggi

## Lampiran
<img width="1918" height="968" alt="image" src="https://github.com/user-attachments/assets/2ec2eae7-ca9b-4cc8-842f-2f1b9d81529e" />

