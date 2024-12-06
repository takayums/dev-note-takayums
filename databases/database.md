<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->

- [Belajar Basis Data](#belajar-basis-data)
  - [Basis Data](#basis-data)
  - [Sistem Basis Data](#sistem-basis-data)
  - [DDL (Data Definiton Language)](#ddl-data-definiton-language)
  - [DML (Data Manipulation Language)](#dml-data-manipulation-language)
  - [Model Data](#model-data)
  - [ERD (Entity Relationship Diagram)](#erd-entity-relationship-diagram)
  - [Entity](#entity)
  - [Atribute](#atribute)
  - [Relationship](#relationship)
  - [Tahapan Membuat ERD](#tahapan-membuat-erd)
  - [Tipe Data](#tipe-data)
  - [Kardinalitas / Derajat relasi](#kardinalitas--derajat-relasi)
  - [One to One](#one-to-one)
  - [One to Many](#one-to-many)
  - [Many to One](#many-to-one)
  - [Many to Many](#many-to-many)
  - [Weak Entity](#weak-entity)
  - [Sub Entity](#sub-entity)
  - [Unary Relationship](#unary-relationship)
  - [Mutli Entity Relationship](#mutli-entity-relationship)
  - [Redundent Relationship](#redundent-relationship)
  - [Tools Pembuatan Entity](#tools-pembuatan-entity)
  - [Normalisasi Data](#normalisasi-data)
  - [Jenis Jenis Atribute](#jenis-jenis-atribute)
    - [1. Atribute Key](#1-atribute-key)
    - [2. Simple Attribute dan Composite atribute](#2-simple-attribute-dan-composite-atribute)
    - [3. Single Value Atribute dan Muliti Value Atribute](#3-single-value-atribute-dan-muliti-value-atribute)
    - [4. Mandatory Atribute](#4-mandatory-atribute)
    - [5. Derived Atribute](#5-derived-atribute)
  - [Atribute Key](#atribute-key)
    - [Super Key](#super-key)
    - [Candidate Atribute](#candidate-atribute)
    - [Primary Key](#primary-key)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# Belajar Basis Data

## Basis Data

Basis data (database) diibaratkan sebagai lemari arsip data. Tujuan dari basis data adalah untuk mengatur, mengelompokkan, dan mengorganisasi data dengan baik. 

Operasi yang dapat digunakan dalam basis data yaitu: Membuat, Membaca, Mengupdate, dan Mendelete data.

## Sistem Basis Data

 Sistem Basis Data adalah software atau perangkat lunak yang mengelola data. Atau disebut juga dengan Database Management Sistem. Perintah yang dilakukan dalam Basis data ada dua yaitu: DDL (Data Definition Language) dan DML (Data Manipulation Language).

## DDL (Data Definiton Language)

DDL adalah perintah untuk membuat struktur data. Seperti membuat table, menyimpan, menghapus basis data arsip, dll.

## DML (Data Manipulation Language)

DML adalah perintah untuk memanipulasi data pada table, seperti menghapus, membuat, dan mencari data pada table.

## Model Data

Model data adalah konseptual untuk menggambarkan suatu data dan juga hubungan antar Data. Tujuannya yaitu supaya kita mengetahui makna dari data itu dan juga relasi antar data. ERD (Entity Relationship Diagram) adalah salah satu cara untuk membuat Model Data.

## ERD (Entity Relationship Diagram)

Terdapat tiga komponent dalam ERD yaitu Entitas, Atribute, dan Relation.

## Entity 

Entity adalah individu yang memiliki fakta data. Contoh dalam lingkup E-Commerce yaitu Pembeli, Penjual, Product, dll.

## Atribute

Atribute adalah karakteristik atau ciri-ciri yang dimiliki oleh Entity. Contoh Pembeli (nama, umur, alamat, dll.). Dalam Entity terdapat Atribute Kunci (Premery Key). Contaoh Pembeli (Nomor Pembeli bisa ID).

## Relationship

Relationship adalah relasi atau hubungan antar Entity. Contoh Penjual dan Product yaitu setiap Penjual memiliki banyak Product.

## Tahapan Membuat ERD

- Menentukan Entity
- Menentukan Atribute Key
- Menentukan Atribute
- Menentukan Relationship
- Implementasi Model Data
- Menentukan Tipe Data
- Menentukan Kardinalitas

## Tipe Data

Ada beberapa jenis tipe data yaitu: Text, Number, Boolean, Datetime, dll.

## Kardinalitas / Derajat relasi

Kardinalitas adalah menentukan jumlah hubungan antar entity. Contohnya setiap penjual data memiliki banyak product yang dijual (relationship one to many). 

## One to One

Contoh hubungan one to one yaitu setiap penjual hanya memiliki satu tempat tinggal. 

## One to Many

Contoh hubungan one to many yaitu setiap penjual memiliki banyak product. 

## Many to One

Kebalikan dari one to many. jadi pasti keduanya memiliki hubungan sama.

## Many to Many

Contoh hubungan dari many to many yaitu beberapa penjual memiliki beberapa kategori penjualan. Pada Kardinalitas many-to-many harus dihubungkan dengan entity tambahan yaitu dengan Kardinalitas one-to-many.

## Weak Entity

Weak Entity adalah entitas lemah, jadi entity tersebut tidak dapat berdiri tanpa adanya entitiy lain. Contoh entitas Dopmet itu tidak bisa berdiri sendiri tanpa adanya entitas pemberli.

## Sub Entity 

Sub Entity adalah entitas yang memiliki beberapa atribut yang sama, tetapi juga jika secara detail memiliki atribute yang berbeda juga. Contoh entitas barang memiliki nama, sku, jenis. Tetapi secara detail jika ada barang jenis laptop dan juga pakaian pasti memiliki atribute yang lebih detail, seperti halnya laptop memiliki jenis ram, cpu, dll. Sedangkan pakaian memiliki jenis ukuran, merek, dll.

## Unary Relationship

Unary Relationship adalah hubungan atau relasi terhadap entitas diri sendiri. Seperti halnya Entitas Member Refeal (Member get Member). Setiap orang atau member bisa meberikan rekomendasi member lain.

## Mutli Entity Relationship

Multi Entity Relationship adalah entitas yang memiliki hubungan atau relasi lebih dari dua entitas. Contoh entitas Pembeli membeli entitas Barang, dengan menggunakan entitas pembayaran dengan Bank.

## Redundent Relationship

Redundent Relationship adalah relasi antar satu entitas itu memiliki lebih dari satu relasi. Contoh Pembeli bisa membeli barang, dan juga pembeli bisa menyukai barang tersebut.

## Tools Pembuatan Entity

- drawio (manual)
- plantuml (otomatis)

## Normalisasi Data

Tujuan dari normalisasi data yaitu redudancy atau penumpukkan data yang tidak konsisten. Dalam tahapn normalisasi data ada 6 tahapan, tetapi yang sering digunakan adalah sampai 3 tahapn saja.

## Jenis Jenis Atribute

### 1. Atribute Key

Bisanya disebute dengan Primary Key. Atribute Key yang disimpan di dalam entitas lain disebut dengan Foreign Key.

### 2. Simple Attribute dan Composite atribute

Simple Atribute adalah atribute yang tidak bisa diturunkan, Sedangkan Composite Atribute adalah atribute yang dapat diturunkan. Contoh Composite Atribute yaitu alaman. Alamat bisa diturunkan lagi dengan nama jln, desa, kec, kab, dan provinsi.

### 3. Single Value Atribute dan Muliti Value Atribute

Single value adalah atribute yang memiliki satu nilai. Sedangkan Multi Value adalah atribute yang memiliki lebih dari satu atribute.

### 4. Mandatory Atribute

Mandatory Atribute adalah atribut yang wajib diisi dan tidak boleh kosong (NULL).

### 5. Derived Atribute

Derived Atribute adalah atribut yang dihasilkan dari pengolahan atribute lain. Contohnya yaitu total belanja, yang berasal dari penjumlahan banyak barang dan harga barang.

## Atribute Key

Atribute Key adalah sebagai identitas dari baris pada entitas tertentu dan bersifat unik. Atribute Key terdiri dari 3 jenis:
- Super Key
- Candidate Key
- Primary Key

### Super Key 

Atribute yang dapat membedakan dari atribute lain dan sifatnya unik.

### Candidate Atribute

Atribute yang berasal dari gabungan dari beberapa atribute yang dapat membedakan atribute lain.

### Primary Key

Key utama yang merepresentasikan dari baris secara unik.
