# A. Server Components

Server Components adalah components yang dirender dibagain sisi server. Gampangnya rendering dilakukan ketika browser meminta ke server terhadap components yang berada pada path tertentu. Kemudian dari server memberikan sebuah response berbentuk RSC payload. Dari hasil response tersebut oleh browser di representasikan menjadi sebuah tampilan. Server Components bersifat non-iteractive. Jadi tidak bisa melakukan click, atau lainnya.

Server Components tidak memiliki rerendering (render ulang). Proses Haydaration.

**Keuntungan Menggunakan Server Components**

- Data Fetching

Data Langsung diambil dan di render tanpa melakukan rendering dua kali karena pemanggilan data yang biasa digunakan di sisi client dengan useEffect atau dengan getServerSideProps. Sehingga render menjadi lebih cepat dan mengurangi jumlah permintaan request data, karena setiap perpindahan halaman data akan di fetching ulang karena menggunakan client components. Contoh Implementasinya yaitu fetching data product dll.

- Keamanan

Jika fetching dengan sisi client maka dipastikan ada kebocoran data seperti token atau kunci api yang dapat dilihat disi network / jaringan browser. Berbeda dengan Server Components fetching data dilakukan disisi client sehingga data tidak bocor atau diketahui oleh hacker dan tidak ada data yang dikirimkan disisi client. Contoh Implementasinya yaitu pada Authentikasi di Login.

- Caching

Caching bermanfaat untuk mengurangi biaya operasional pada server karena caching berguna untuk menggunakan kembali data yang sudah di fetching khususnya data data yang tidak berubah seperti blog atau product.

- Performa

- Pemuatan Halaman Awal dan FCP

- SEO dan Kemampuan Berbagi Jaringan

- Streaming
