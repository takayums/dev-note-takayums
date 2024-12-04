<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->

- [Prisma](#prisma)
  - [Prisma Overview](#prisma-overview)
  - [Why Prisma?](#why-prisma)
  - [Should use Prisma?](#should-use-prisma)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# Prisma

Prisma terdiri dari: 
- Prisma Client
- Prisma Migrate
- Prisma Studio

## Prisma Overview

Ada tiga configurasi dalam prisma: 
- Data Source (Env Tipe Database) 
- Generator (Generat dengan Prisma Client)
- Data Model (Definisikan Model)

Data model adalah representasi collection dari model. Fungsi dari model yaitu untuk representasi relasi dari tabel dan fondasi untuk query Prisma Client

Cara kerja dalam Prisma ada dua: 
- Prisma Migrate 
- SQL migration and interspection (manual)

## Why Prisma?

Prisma berguna untuk menambah produktifitas dari developer, sehingga tidak khawati terhapa maintain query SQL yang terkadang membuat rumit dan susah untuk di maintaince. Selain itu seorang pengembang sangat penting untuk menjaga dan mengembangkan fitur data, bukan hanya berfokus pada query SQL.

## Should use Prisma?

Prisma sangat baik digunakan jika kita: 
- Server yang berkomunikasi dengan Database
- Produktif dalam pengalaman developer
- Bekerja dengna tim
- Tool yang membantu dalam alur kerja
- Tipe data yang aman
- Transparasi proses alur pengembangan
