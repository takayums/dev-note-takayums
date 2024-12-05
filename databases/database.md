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
