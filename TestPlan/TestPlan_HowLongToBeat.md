# Test Plan – Fitur Login dan Signup

## 1. Informasi Dokumen
Versi dokumen: 1.0  
Disusun oleh: M. Aidil Kamal Adlim  
Tanggal: 23 Februari 2026  
Direview oleh: -  
Status Persetujuan: draft  

## 2. Pendahuluan
Dokumen ini menjelaskan strategi, pendekatan, ruang lingkup, dan kriteria keberhasilan untuk pengujian fitur Login dan Signup pada website HowLongToBeat.  

## 3. Tujuan
- Memastikan user dapat melakukan login dengan kredensial valid.
- Memastikan user dapat melakukan pendaftaran akun baru dengan data valid.
- Memastikan validasi input berjalan sesuai aturan.
- Memastikan pesan error ditampilkan dengan benar.
- Mengidentifikasi defect sebelum fitur digunakan oleh end-user.

## 4. Ruang Lingkup
### In Scope
- UI Login functionality
- UI Signup functionality
- Field validation
- Error message validation
- Basic session behavior (redirect setelah login)
- Boundary value testing untuk input field

### Out of Scope
- API & backend logic
- Database validation
- Forgot password functionality
- Performance testing
- Security penetration testing (advanced)

## 5. Strategi Pengujian
Testing akan dilakukan dengan manual testing menggunakan teknik black-box testing.  
Skenario positif dan negatif akan dilakukan.  
Boundary value analysis juga akan dilakukan untuk validasi input.  

## 6. Lingkungan Pengujian
- OS: Windows 11
- Browser: Chrome 145
- Environment: Production

## 7. Kriteria Keberhasilan
- 100% test case Prioritas High telah dieksekusi.
- Tidak ada defect severity Critical atau High yang masih open.
- Minimal 95% total test case berstatus Pass.
- Test summary report telah dibuat.
