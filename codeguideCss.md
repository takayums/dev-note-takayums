## CSS (Cascading Style Sheets)

### 1. Syntax

- Menggunakan tab atau dua spasi
- Jika terdapat grouping slector harus setiap slector satu baris
- Satu spasi untuk sebelum kurung kurawal
- kurung kurawal terakhir harus berada pada line akhir baru
- Satu sepasi untuk setelah tanda titik dua ": "
- Titik koma untuk akhir setiap declarasi css
- Setiap nilai yang terdapat koma haru ada sepasi satu
- Setiap value color jika terdapat koma maka ganti dengan spasi saja
- Jangan gunakan 0 pada nilai koma, seperti 0.5 tetapi gunakan .5
- Gunakan heksa yang singkat dan gunakan huruf kecil saja
- Gunakan quote untuk atribut value selector
- Gunakan nilai spesifik jika margin: 0; tetapi gunakan margin: 0px;

### 2. Urutan Declarasi Css

- Positioning
- Box Model
- Typography
- Visual
- Misc

### 3. Logical Properties

pada logical properties berpatokan untuk inline yaitu horizontal(left-right) dan untuk block yaitu vertical(bottom-top).

```CSS
// Without logical properties
.element {
  margin-right: auto;
  margin-left: auto;
  border-top: 1px solid #eee;
  border-bottom: 1px solid #eee;
}

// With logical properties
.element {
  margin-inline: auto;
  border-block: 1px solid #eee;
}
```

### 4. Colors

pada colors terdapat singkatan color rgba() dan hsla(), keduanya bisa dirubaha dengan rgb(0 0 0 / .98) dan hsl(0 0 0 / .98)

```CSS
.element {
  color: rgb(255 255 255 / .65);
  background-color: rgb(0 0 0 / .95);
}
```

### 5. Hindari penggunaan @import

### 6. Media Query

Penulisan media query dilakukan dalam satu file saja, dan didekatkan pada selectornya yang ada.

```CSS
.element { ... }
.element-avatar { ... }
.element-selected { ... }

@media (min-width: 480px) {
  .element { ... }
  .element-avatar { ... }
  .element-selected { ... }
}
```

### 7. Deklarsi Tunggal

deklarsi tunggal jika kita hanya menerapkan code css hanya satu properties saja.

```CSS
// Single declarations on one line
.span1 { width: 60px; }
.span2 { width: 140px; }
.span3 { width: 220px; }

// Multiple declarations, one per line
.sprite {
  display: inline-block;
  width: 16px;
  height: 15px;
  background-image: url("../img/sprite.png");
}
.icon           { background-position: 0 0; }
.icon-home      { background-position: 0 -20px; }
.icon-account   { background-position: 0 -40px; }
```

### 8. Notasi Singkat

```CSS
.element {
  margin: 0 0 10px; ## langsugn menggunakan margin-bottom: 0px;
  background: red;
  background: url("image.jpg");
  border-radius: 3px 3px 0 0;
}

// Good example
.element {
  margin-bottom: 10px;
  background-color: red;
  background-image: url("image.jpg");
  border-top-left-radius: 3px;
  border-top-right-radius: 3px;
}
```

### 9. Preprosecor Bersarang

```CSS
// Without nesting
.table > thead > tr > th { … }
.table > thead > tr > td { … }

// With nesting
.table > thead > tr {
  > th { … }
  > td { … }
}
```

### 10. Operator dalam Preproseccor

```CSS
// Bad example
.element {
  margin: 10px 0 @variable*2 10px;
}

// Good example
.element {
  margin: 10px 0 (@variable * 2) 10px;
}
```

### 11. Komment pada CSS

berikan komentar yang jelas untuk apa css tersebut dan juga pada selecot apa yang diterapkan.

```CSS
// Bad example
// Modal header
.modal-header {
  ...
}

// Good example
// Wrapping element for .modal-title and .modal-close
.modal-header {
  ...
}
```

### 12. Class Name

- Penggunaan huruf kecil dalam pemberian class
- Gunakan penghubung "-" daripada menggunakan penulisan CamleCase
- Berikan nama class dengan singkatan yang jelas

### 13. Selector

- Berikan selecot lebih pendik maksimal 3 kata.
- Gunakan selector class dari pada tag, jika tidak berpengaruh pada markup

### 14. Pemilihan anak dan turunan dari Seletor

```CSS
.custom-table > tbody > tr > td,
.custom-table > tbody > tr > th {
  /* ... */
}
```

### 15. Organization

- Mengelompokkan bedasarkan komponent
- Gunakan Komentar Konsisten
- Jika ada beberapa file Css bedakan besarkan bukan halaman tetapi karena komponent
