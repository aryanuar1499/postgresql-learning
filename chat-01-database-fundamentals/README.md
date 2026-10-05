# Chat 01 — PostgreSQL Database Fundamentals

## 🎯 Learning Objectives

Pada learning session ini, saya mempelajari fundamental PostgreSQL dan konsep dasar relational database sebagai fondasi untuk memahami SQL, database design, dan data querying.

Target pembelajaran:

* Memahami apa itu PostgreSQL
* Memahami konsep Database Management System (DBMS)
* Memahami konsep Relational Database Management System (RDBMS)
* Memahami struktur dasar relational database
* Memahami hubungan antara Database, Schema, Table, Row, dan Column
* Memahami konsep Primary Key
* Mengenal SQL sebagai bahasa untuk berinteraksi dengan relational database
* Mulai menggunakan PostgreSQL melalui pgAdmin 4

---

## 📚 Learning Materials

Dokumentasi pembelajaran akan dikembangkan secara bertahap berdasarkan materi, praktik, dan eksperimen yang dilakukan selama learning session.

### Topics

1. PostgreSQL & RDBMS
2. Relational Database Concepts
3. Database Structure
4. SQL Fundamentals
5. PostgreSQL Environment
6. Hands-on Practice
7. Key Insights
8. Reflection

## 1. What is PostgreSQL?

PostgreSQL adalah **Relational Database Management System (RDBMS)** open-source yang digunakan untuk menyimpan, mengelola, dan mengambil data menggunakan **SQL (Structured Query Language)**.

PostgreSQL menerapkan relational database model, sehingga data dapat disimpan dalam bentuk table dan dihubungkan dengan table lainnya melalui relationship.

Secara sederhana:

```text
PostgreSQL
     ↓
RDBMS
     ↓
Relational Database
     ↓
SQL
```

> PostgreSQL adalah sistem yang mengelola database, sedangkan SQL merupakan bahasa yang digunakan untuk berinteraksi dengan database tersebut.

---

## 2. PostgreSQL as a DBMS and RDBMS

PostgreSQL termasuk ke dalam **Database Management System (DBMS)**, lebih spesifik lagi merupakan **Relational Database Management System (RDBMS)**.

RDBMS merupakan jenis DBMS yang menggunakan relational model untuk mengorganisasi dan mengelola data.

Struktur sederhananya:

```text
DBMS
 │
 └── RDBMS
      │
      ├── PostgreSQL
      ├── MySQL
      └── ...
```

PostgreSQL sendiri bukan sebuah database, melainkan sistem yang digunakan untuk mengelola database.

Contohnya:

```text
PostgreSQL
    │
    └── Database
         │
         ├── pelanggan
         ├── produk
         └── transaksi
```

---

## 3. Why PostgreSQL?

PostgreSQL dibutuhkan ketika data mulai memiliki jumlah, struktur, dan relationship yang lebih kompleks sehingga membutuhkan sistem pengelolaan data yang lebih terstruktur dibandingkan spreadsheet sederhana.

Beberapa kemampuan PostgreSQL yang mendukung pengelolaan data antara lain:

* **Primary Key** untuk mengidentifikasi data secara unik
* **Foreign Key** untuk menjaga relationship antar-table
* **Constraints** untuk menjaga data integrity
* **Transactions** untuk menjaga konsistensi proses perubahan data
* **Indexes** untuk membantu meningkatkan query performance
* **SQL** untuk melakukan data querying dan analysis

Sebagai contoh, sistem penjualan dapat memiliki beberapa entity:

```text
Pelanggan
    │
    ↓
Transaksi
    │
    ↓
Detail Transaksi
    │
    ↓
Produk
```

Dengan relational database, hubungan antar-data tersebut dapat dikelola secara terstruktur sehingga perubahan dan pengolahan data dapat dilakukan dengan lebih konsisten dan efisien.

### Key Insight

> PostgreSQL bukan sekadar tempat menyimpan data. PostgreSQL adalah **RDBMS yang menyediakan berbagai mekanisme untuk menyimpan, mengelola, menjaga konsistensi, menghubungkan, dan menganalisis data secara terstruktur.**
