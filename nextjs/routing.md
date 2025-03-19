# Routing

Routing didalam nextjs ditentukan nama folder yang ada dalam folder app. Tiap folder dalam app harus memiliki file yang bernama page.tsx{js,js,tsx,ts}. Begitu juga untuk nesting route, berarti dalam folder app ada sub folder kedua dalam folder turunan pertama app.

## Layouting

Layouting berguna supaya kita tidak melakukan penulisan koponent setiap page route. Contohnya yaitu Navbar, Footer dan Sidebar. Jika kita tanpa layouting pasti kita menulis komponent navbar dan footer pada setiap page nextjs. dan untuk sidebar hanya berlaku pada page yang memiliki akses admin. Maka dibuat lah layout user dan juga layout admin/dashboard untuk memisahkannya.

## Nesting Layout

Tidak hanya pada routing saja nesting juga berlaku pada layout.

# Dynamic Routing

Dynamic routing digunakan untuk mempermudah kita supaya membuat halaman menjadi dinamis, dengan memberikan segment pada path yang ingin diakses, contonya saja jika kita menampilkan detail blog, halaman product bedasarkan kategory. Jadi sagman tersebut nanti dikirimkan ke api action untuk mengambil data dan juga menampilkan halaman bedasarkan ketentuannya.
