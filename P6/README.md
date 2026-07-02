# 📊 DATABASE KOPERASI (MySQL / MariaDB - XAMPP)

Project ini merupakan latihan pembuatan database koperasi menggunakan MySQL/MariaDB di XAMPP melalui CMD.

---

# ⚙️ INFORMASI PROJECT
- Nama Database : koperasi  
- DBMS : MariaDB (XAMPP)  
- Tools : CMD / MySQL Terminal  
- Bahasa : SQL  

---

# 🗂️ STRUKTUR DATABASE

Database ini terdiri dari **4 tabel (entitas utama)**:

---

## 1. Tabel ANGGOTA
Menyimpan data anggota koperasi.

| Kolom | Tipe | Keterangan |
|------|------|------------|
| id_anggota | INT | Primary Key |
| nama | VARCHAR(50) | Nama anggota |
| alamat | VARCHAR(100) | Alamat anggota |
| no_hp | VARCHAR(15) | Nomor HP |

---

## 2. Tabel SIMPANAN
Menyimpan data tabungan anggota.

| Kolom | Tipe |
|------|------|
| id_simpanan | INT (PK) |
| id_anggota | INT |
| jenis | VARCHAR(30) |
| jumlah | INT |

---

## 3. Tabel PINJAMAN
Menyimpan data pinjaman anggota.

| Kolom | Tipe |
|------|------|
| id_pinjaman | INT (PK) |
| id_anggota | INT |
| jumlah | INT |
| bunga | INT |

---

## 4. Tabel ANGSURAN
Menyimpan data pembayaran cicilan.

| Kolom | Tipe |
|------|------|
| id_angsuran | INT (PK) |
| id_pinjaman | INT |
| cicilan_ke | INT |
| bayar | INT |

---

# 🧾 PERINTAH PEMBUATAN DATABASE

```sql id="sql1"
CREATE DATABASE koperasi;
USE koperasi;
