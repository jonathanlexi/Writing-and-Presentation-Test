# Week 5 Resume


## Fundamental React
- React adalah library javascript untuk membuat tampilan(user interface) pada website
- React digunakan sebagai pengganti DOM(lambat dan tidak efisien)
- Berbasis komponen
- SPA (Single Page Application) = menggunkan satu halaman web saja sebagai tampilan aplikasinya web dibuat menjadi ringan dan cepat
 
## Cara Menjalankan React 
- install node js latest 
- npm -v (cek apakah sudah di insatall)
- npx create-react app nama_folder (membuat folder react yang berisi library dan file khusus react)
- npm start(melihat tampilan di browser)
  - ### Isi folder 
  - node-modules = isi library 
  - public = didalam terdapat index.html yang menjadi sgp/tumpuan
  - src = halman,component,fokus untuk resource yang diproses
  - file package = file yang mencatat library yang telah diiinstal dalam project,menyimpan library yang digunakan 
  - file package-lock=optional
  
  ![image](https://user-images.githubusercontent.com/85721522/198880135-7c808fb7-3b6a-46fd-a8af-35742e52353b.png)



## Jsx
- jsx adalah javascript xml 
- gabungan penggunaan syntax js dan element html  
- biasanya didalam kurung kurawal adalah syntax js
- format penamaan file .js / .jsx

## Class Component dan Functional Component

Components bersifat reuseable(bisa dipakai berkali kali)

- Class Component

  ![image](https://user-images.githubusercontent.com/85721522/198880638-c6eaef41-4605-4fcc-8fee-d517601c8487.png)

- Function Component

  ![image](https://user-images.githubusercontent.com/85721522/198880686-9d1f47e1-aec7-44d0-9f88-6dbbbff17052.png)


Penggunaan function 
- nama function diawali huruf kapital
- export default nama function
- function hanya return 1 parent
(div,fragment kosong)
  
  ![image](https://user-images.githubusercontent.com/85721522/198880833-11ae948b-8774-4ed8-af95-8e2af7958088.png)

## State & Props
- Membuat suatu komponen mennjadi dinamis 
- State => objek untuk menyimpan data dan di render ketika melakukan perubahan data di dalam component
        => Tempat penampungan data yang dapat diubah
  - Ciri ciri function state 
    import {useState} from 'react'
    syntax => const[count,setCount] = useState(0)
	                 (value) (function)	(inisiasi nilai awal)
    count(value) = yang akan ditampilkan di page
    setCount(function) = yang mengubah data
  - Stateful (komponen yang memiliki state)
  
    ![image](https://user-images.githubusercontent.com/85721522/198881154-a28c94dc-d10e-45d4-8a35-37057695e174.png)

  - Stateless (komponen yang tidak memiliki state)
  
    ![image](https://user-images.githubusercontent.com/85721522/198881178-0c6f38b6-1ef3-42c9-a9b8-9dbd99b2dbe4.png)

    
- Props (properties) => komunikasi/data yang dikirim dari komponen parent ke child / parameter function
		
    ![image](https://user-images.githubusercontent.com/85721522/198881178-0c6f38b6-1ef3-42c9-a9b8-9dbd99b2dbe4.png)


## React event handler
    
   - onClick()

   ![image](https://user-images.githubusercontent.com/85721522/198881267-638cfaba-4cd8-4219-ad5b-271febaf29c3.png)
   
  ## lifecycle method react js 
  
   ![image](https://user-images.githubusercontent.com/85721522/198883909-8398e8c2-bb89-4fab-88e0-ebc3e596d3ff.png)
    
- mount 
- unmount
- update  

![image](https://user-images.githubusercontent.com/85721522/198883974-10044e7c-c409-4491-98ce-977fb5bd19e1.png)

## Hooks
  - hooks adalah fitur yang dapat memudahkan penggunaan functional components agar bisa menggunakan state dan lifecycles lainnya 
  - ### UseState
  
    ![image](https://user-images.githubusercontent.com/85721522/198884279-5763fc9e-956e-4db9-ad45-e753e6b133d2.png)
    
  - ### UseEffect
    - hooks yang bisa digunakan untuk menggunakan lifecycle pada functional component dengan mudah 
    - penggunaan useEfect bisa dimasukkan sebelum melakukan render,biasanya terletak di bawah useState
    - ![image](https://user-images.githubusercontent.com/85721522/198884562-be841764-648b-4237-a8ee-71462a0b131e.png)
    - ![image](https://user-images.githubusercontent.com/85721522/198884581-78ba8080-f6be-4e73-a220-e9d8f4ae6d43.png)
    - ![image](https://user-images.githubusercontent.com/85721522/198884611-40728dcc-b205-47c4-bc5d-cdf11309e1a7.png)

## PropTypes
- Pengecekan tipe data props dapat menggunakan PropTypes
- PropTypes.element, menentukan bahwa hanya dapat menerima satu komponen anak yang dapat dikirimkan ke komponen lain
- install proptypes di terminal dengan command npm install prop-types
- import PropTypes 'prop-types';
- defaultProps,mendefinisikan nilai default props 

![image](https://user-images.githubusercontent.com/85721522/198936941-948c70d8-7af0-4951-b86a-4b5fba3dfc7a.png)

### Mengecek props termasuk kedua type data tersebut

![image](https://user-images.githubusercontent.com/85721522/198939415-f26a5a82-26e3-49b3-ba4b-1563ef667a10.png)

### Mengecek type data apa yang ada didalam prop array 

![image](https://user-images.githubusercontent.com/85721522/198939826-19161a09-8fb0-4c39-a868-1da6e05d09ad.png)

## styling pada react js 
- styling inline menggunakan property style
  - style={{backgroundColor : ''}}
  - style={{props.color}}

- styling external
  -  ![image](https://user-images.githubusercontent.com/85721522/198884120-afe1872c-49c0-4edf-a045-4227636bdb81.png)
 
  -   ![image](https://user-images.githubusercontent.com/85721522/198884155-da52d160-b304-4b75-a6bf-97c1c0baca81.png)









