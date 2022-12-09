![Image Banner!](assets/banner.png "Javascript")

# Tutorial setting Prettier in React

### Apa itu Prettier ?

> Prettier adalah penata format kode. Prettier mendorong gaya penulisan kodemu menjadi konsisten

### Kenapa menggunakan Prettier ?

> Untuk menyamaratakan format penulisan kode ketika bekerja bersama tim karena tak jarang setiap orang memiliki formatnya masing2

### Bagaimana cara menggunakan Prettier ?

1. buka website https://prettier.io/docs/en/install.html
2. install Prettier di local
   ```
   npm install --save-dev --save-exact prettier
   ```
3. buat file yang bernama **.prettierrc.json**, dilokasi yang sejajar dengan **src**
4. tuliskan format yang kamu inginkan didalam file barusan.
   contoh :
   ```
   {
        "tabWidth": 4,
        "singleQuote": true,
        "jsxSingleQuote": true,
        "semi": false
   }
   ```
5. jalankan format Prettier yang barusan kita buat

   ```
   npx prettier --write .
   ```

   noted: tanda "." artinya memilih semua file yang ada

6. jika cara no.5 barusan di anggap terlalu rumit, kamu bisa menggunakan cara ini :

   1. buka file **package.json**
   2. tambahkan `"format": "npx prettier --write ."` pada 'script'
   3. sekarang kamu hanya tinggal menjalankan
      ```
      npm run format
      ```
