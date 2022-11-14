# Week 7 Resume

## React Context
- context digunakan untuk menghindari oper props melalui elemen perantara
- pengganti redux 
- Redux digunakan untuk project yang benar-benar membutuhkan manage state dan project tersebut termasuk project besar serta kompleks
- Context digunakan untuk project yang tidak terlalu besar dan kompleks
- Context merupakan library eksternal javascript yang digunakan pada react.js
- Dalam context terdapat dua property, yaitu

## Menggunakan reac context 
- Buat aplikasi react js atau buka folder aplikasi react js jika sudah ada
- Membuat context gunakan createContext
- Fungsi createContext akan mengembalikan provider dan consumer component


## Testing
- Testing pada react untuk memeriksa bahwa code sudah sesuai harapan
- Testing membantu memastikan dan mengetahui celah yang belum teratasi tetapi tidak menyelesaikan bug
- Selain itu, manfaat testing adalah
    - Meningkatkan stabilitas program jika testing terstruktur dengan baik
    - Software engineer dapat menyadari jika terjadi penuruan performa
    - Digunakan sebagai desain (TDD)
- Testing terbagi menjadi dua jenis, yaitu:
  - Manual testing (dilakukan manual dengan analisis manusia)
  - Automated testing (dilakukan dengan code)
  
  ### Automated testing 
  - dibagi menjadi 3 
    - unit tes = membuat komponen dari yang paling kecil seperti functionya bakal di test apakah sesuai ekspetasi kita atau tidak. Setiap buat code lakukan unit test
    - integration = Integration test: satu aplikasi terhubung ke system lain, contoh database
    - end to end =  test yang dilihat dari sisi user (workflow dari awal sampai akhir)

### Menulis testing 
- Import fungsi untuk menguji
- Memberikan masukan ke fungsi
- Menentukan apa yang diharapkan sebagai output
- Memeriksa apakah fungsi menghasilkan output yang diharapkan

### Tes Driven Development
- Circle of life 
  - Red zone (test fails): tahap menulis ekspetasi tanpa code
  - Green zone (test passes): tahap membuat code untuk ekspetasi
  - Blue zone (refactor): tahap memperbaharui code tanpa mengubah ekspetasi

### Unit Testing 
- Unit test merupakan automated test yang paling sering digunakan
- Unit test merupakan test yang paling murah dan yang paling cepat karena sang developer tinggal mengetest function tanpa perlu hire orang lain
- Unit test baiknya digunakan untuk menguji satu unit saja dari program kita (satu fungsi)
- Unit test memiliki tiga istilah, yaitu arrange-act-assert
- arrange-act-assert merupakan pola untuk mengatur dan memformat code dalam unit test
  - Arrange: mengatur semua persyaratan dan input yang dibutuhkan
  - Act: melakukan pengujian pada object yang ingin diuji
  - Assert: memastikan hasil yang diharapkan telah didapat
- Pada unit test, hasil yang didapat dari function yang dites akan dibandingkan dengan nilai ekspektasi
- Test akan gagal bila kedua data tidak sama

### Jest 
- Jest merupakan library javascript untuk melakukan pengetesan pada unit test
- Jest menggunakan matchers untuk membandingkan nilai, seperti:
  - memeriksa kesetaraan
  - membandingkan dua nomor atau string
  - memverifikasi truthiness ekspresi
- Menginstall package jest npm install jest --save-dev

### RTL (React Tesing Library)
- React Testing Library dibangun di atas DOM Testing Library dengan menambahkan API untuk bekerja dengan komponen React
- Di dalam RTL sudah terdapat jest
- RTL merupakan library unit testing semi end-to-end
- Menginstall library testing npm install --save-dev @testing-library/react

### Elemen berdasarkan Accessibility
- Access by everyone
    - getByRole
    - getByLabelText
    - getByPlaceholderText
    - getByText
- Semantic queries
    - getByAllText
    - getByTitle
- Test ID
    - getByTestId

Catatan:

- toBe() untuk mencocokan value yang didapat dengan value yang diharapkan
- jest.fn() untuk membuat function mock jest
- .toEqual() method matcher untuk mencocokkan nilai dari dua object, biasa disebut 'deep equal'
- npm run test perintah untuk menjalankan testing
