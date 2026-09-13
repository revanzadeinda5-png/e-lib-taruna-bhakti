# E-Lib TB (Sistem Informasi Perpustakaan SMK Taruna Bhakti)

Aplikasi manajemen perpustakaan digital berbasis web yang dirancang untuk mempermudah transaksi peminjaman, pengembalian, dan pencatatan buku.

## 📌 Dokumen Pendukung
Dokumen resmi Software Requirements Specification (SRS) dapat diunduh pada repositori ini:
* [SRS-Document.pdf](./SRS-Document.pdf)

## 📊 Design System (UML Diagram)

### 1. Use Case Diagram
```mermaid
graph TD
    Siswa((Siswa))
    Admin((Admin / Pustakawan))

    subgraph "Sistem Informasi Perpustakaan (E-Lib TB)"
        UC1[Login Sistem]
        UC2[Lihat Katalog Buku]
        UC3[Kelola Data Buku]
        UC4[Kelola Data Pengguna]
        UC5[Proses Transaksi Peminjaman]
        UC6[Proses Pengembalian & Hitung Denda]
        UC7[Lihat Riwayat Peminjaman]
        UC8[Cetak Laporan Sirkulasi]
    end

    Siswa --> UC11
    Siswa --> UC2
    Siswa --> UC7

    Admin --> UC1
    Admin --> UC2
    Admin --> UC3
    Admin --> UC4
    Admin --> UC5
    Admin --> UC6
    Admin --> UC7
    Admin --> UC8