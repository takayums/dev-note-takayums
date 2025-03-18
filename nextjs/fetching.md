# Fetching

Supaya dalam fetching data, saat response untuk type tidak bertipa any maka kita harus mendeklarisakn dulu typenya atau dibuat assertation. Terkadang untuk meminimalkan fetching data maka kita bisa gunakan caching. sehingga fetching data dengan url yang sama tidak akan dilakukan request langsung ke server. Karena fetching data sebelumnya sudah disimpan. Hal itu disebut dengan request memoization.

Pada client component tidak bisa menggunakan async await dalam fetching data. maka ada cara dengan initiation dengan fetching di server component kemudian dikirimkan ke component client dengan menggonakan use hooks. jadi di server komponent tidak useh mengguankan await dan hanya mengirim props ke client component dan berbentuk promise.

Penggunakan Suspense pada server components dan itu merupakan bagian fitur streaming.
