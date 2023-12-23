# Redux Toolkit

tujuan dibuatnya redux toolkit untuk membuat konfigurasi yang mudah, meringkas paket yang dibutuhkan dan mengurangi penggunaan boilerplate yang berulang kali dengan digantikan beberapa fungsi baru.

Redux Toolkit juga memberikan penggunaan **data feching dan catching**, yaitu dengan menggunakan **RTK Query**.

Empat keunggulann dari Redux Toolkit adalah:

- Sederhana

Menjadikan satu tempat untuk melakukan konfigurasi, mendefinisikan action dan reducer dalam satu lokasi utama.

- Mengedepankan Opini

Mengedepankan pendekatan dalam pengelolaan state, dan memberikan aturan-aturan yang konsisten dan direkomendadikanan dalam pengelolaan state.

- Powerfull

Kuat dalam hal fleksibel saat penggunaan, prediktif, dan arsitektur yang baik dalam pengelolaan state.

- Effective

Pemberian tools yang mudah digunakan tanpa kita memikirkan boilerplate dalam menyusun dari tools tersebut.

## Pemahaman Redux Sebenarnya

Store tunggal yang berisi state glolbal, Mengirimkan object action ke dalam store ketika terjadi sesuatu, dan Reducer murni yang mengupdate state secara permanen ketika terjadi tindakan.

## Hal yang tidak wajib tapi dianjurkan ada

1. Actions
2. Middleware
3. Thunk
4. Normalisasi state bedasarkan ID state
5. Pengoptimalan data turunan
6. Redux Dev Tools
7. Tipe Typescript untuk action, state, dan function
8. React Redux

## RTK Query

Digunakan untuk melakukan fetching dan caching data, sehingga tidak perlu melakukan secara manual. RTK Query dibangun diatas Redux Toolkit.
