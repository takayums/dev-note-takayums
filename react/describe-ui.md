# Describe UI

## Components

Components dalam react yaitu berbentuk function. Dan sebuah element dalam html seperti button itu bisa dikatakan juga dengan sebuah component.

## Import Export Component

Layaknya sebuah function, component juga bisa digunakan dimana saja file yang ada. Dengan cara yaitu melakukan export import function. Dalam sebuah file bisa saja memiliki lebih dari satu components.

## JSX

React Components diutulis dengan sebuah syntax yang disebut JSX. JSX yaitu syntax markup yang menggabungkan antara Javascript dengan HTML yang dapat juga memiliki informasi dynamic dengan penggunaan Javascript.

Untuk menggunakan dynamic property kita bisa menuliskan dengan kurung kurawal yang diisi property dynamc itu.

## Props

Dalam React Props disebut juga dengan properties. Props ini digunakan untuk mengirimkan sebuah data baik itu berbentuk array, object, variable, dll ke sebuah component dibawahnya. Children component disebuat juga sebagai anak component diaman didalam component ada turunannya component lagi.

## Conditional Rendering

Terkadang sebuah component dapat ditampilkan sesuai keinginkan kita. Biasanya hal ini menggunakan conditional rendering.
Contoh kita ingin menampilkan mark check list ketika todo list itu sudah dikerjakan.

## Rendering List

Rendering list sering digunakan ketika kita ingin menampilkan beberapa list data dalam sebuah component. Dan penggunaan rendring list ini biasanya menggunakan `filter` dan `map`. Setiap list data yang di render pada component harus memiliki seubah `key`.

## Keep Components Pure

Component dikatan murni jika:

- Mengurus urusannya sendiri dan tidak merubah nilai atau variable yang sudah ada didalam comonent itu sendiri.
- Inputan dan Output yang ada pada component akan menghasilkan nilai yang sama ketika rendering.

## UI Tree

Untuk memahami sebuah component maka didefinisiakn lah pohon component. Dimana jika component tidak memiliki child itu disebut daun component, sedangkan komponent yang memiliki anak component itu disebut Disebut Top Level Component. Dan Component paling atas sendiri disebut Root Component / Parent Component.
