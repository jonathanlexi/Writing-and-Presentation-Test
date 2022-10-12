# Week 4 

## JS Fetch
 - API menjadi perantara antara web aplikasi dan server dan database

 - API mengambil data dari server ke web 

 - API ditanggkap dengan promises dan async await
 
  ![image](https://user-images.githubusercontent.com/85721522/194855461-2d2c082e-b8ce-4842-9eb7-4c680c2e4fdc.png)

  ### Akses fetch 
  
  - promise (than catch)
  
    ![image](https://user-images.githubusercontent.com/85721522/194902741-9adab2ed-0e45-47ae-9d80-dd5e99a531a1.png)


  - async await
  
    ![image](https://user-images.githubusercontent.com/85721522/194904711-10e9b70b-f1d8-4e1f-ba01-f78c77abe380.png)

  
  
## JS Async await
 - cara untuk menangkap objek promise

#### Menjalankan kode promise dengan 2 cara 
- promise (than catch)
- async await 

## Git & Github Lanjutan

- git adalah software yang version control system yang berfungsi untuk mencatat perubahan file atau repository 
- github adalah layanan cloud untuk menyimpan dan mengelola project (repository)
- git & github digunakan agar bisa bekerja sama/berkolaborasi dengan tim 

### git hub organization 
 - membuat fitur didalam branch tertentu seperti membuat fitur login harus di dalam branch khusus untuk menyimpan file login
 - menghindari banyak bug 
 - client dan developer dapat berkolaborasi.

### Command git 

- git branch
  - fitur fitur dikelola oleh branch masing masing 
  - command line : 
  - git branch nama_branch (membuat branch baru)
   - git branch (cek nama nama branch yang ada)
   ![image](https://user-images.githubusercontent.com/85721522/195302532-9791a71e-2108-45dc-94fe-ff7afb4f7412.png)
   - git branch --merged (mengecek apakah branch sudah di merge)
   - git branch -d nama_branch_delete (menghapus branch yang tidak diperlukan)
  
       ![image](https://user-images.githubusercontent.com/85721522/195312027-1cfa3b37-a0ef-4b2d-98fc-a30c6667cd21.png)


- git switch = git checkout
  - berfungsi pindah branch
  
  ![image](https://user-images.githubusercontent.com/85721522/195304378-e43ef09c-4de5-4c3b-a858-da94425f5c97.png)


- git merge (menggabungkan branch)
  - command : git merge nama_branch 

  - ### git merge conflict
  - terjadi karena 2 branch mengerjakan baris yang sama dalam 1 repo
  - ![image](https://user-images.githubusercontent.com/85721522/195316727-ca08a0c5-07cf-4dec-a257-8f367eb59f2e.png)
  - Demo conflict yang terjadi ketika melakukan merge
  - ![image](https://user-images.githubusercontent.com/85721522/195320038-0b1e719e-48b4-4216-a573-830fa15d37be.png)
  - Untuk mengatasinya pilih data mana yang ingin diubah lalu lakukan commit seperti biasa


- git pull
  - mengambil file baru repository
  
- git clone
  - berfungsi untuk download atau mengambil file di repository github dan di simpan ke penyimpanan local
  - tidak perlu lagi menggunakan git remote
  - command line : git clone url

- git log => menampilkan commit yang sudah dilakukan

![image](https://user-images.githubusercontent.com/85721522/195302963-919474e6-5ab3-4323-8699-02ce0071646e.png)


## Responsive Web Design & Bootstrap

- Responsive adalah layout yang tetap menarik walaupun diakses di berbagai device
- Responsive Web Design (RWD) bertujuan membuat desain website dapat diakses dalam device apapun 


### viewport (bagian dari responsive web)
- viewport adalah area website yang dapat diakses oleh user
- viewport diakses di html dengan tag <meta name="viewport" content="width=device-width, initial-scale=1.0">
- tujuan tag viewport meta agar tampilan lebih jelas dilihat

### Ada beberapa cara untuk membuat tampilan menjadi responsive
 - max-width : 100% (membuat ukuran objek sesuai dengan ukuran layar )
 - ### CSS relative units (satuan ukur yang relative terhadap sesuatu)
 - css unit digunakan sesuai dengan kreasi masing masing 
       - px (absolute)
       - em 
       - rem 
       - vw/viewport widht (mengikuti lebar dari viewport)
       - vh/viewport height (mengikuti tinggi dari viewport)
       - % (relative terhadap parent elementnya)
 - #### em vs rem
        - em (ukuran sesuai dengan element)
        - 2em=40px
        - rem (ukuran relative dengan root html)
        - ukuran root html = 16px
        - 2rem = 32px
 - ![image](https://user-images.githubusercontent.com/85721522/195342397-f0856400-4b60-4517-9448-aadf898e7e53.png)
 - ### Media query (digunakan untuk membuat beberapa styles tergantung pada jenis device)
 
 ![image](https://user-images.githubusercontent.com/85721522/195390809-b719c1fb-cb88-4a5e-9f17-9084dc422bd8.png)

 - Flex (secara 1 arah vertical atau horizontal)
 - Grid (secara vertical dan horizontal)
 - ### Bootstrap
       -  Dapat membuat website lebih cepat dan responsive
       -  layout (breakpoints,containers,grid,column)
       -  grid system menggunakan container,rows,columns untuk mengatur posisi konten
       -  grid system dibagi menjadi 12 kolom
       -  components
       -  https://getbootstrap.com/docs/5.2/getting-started/introduction/
  
