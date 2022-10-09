# Week 3 

## Array Js

### Method Array
- push() = menambah element beru di akhir 
![image](https://user-images.githubusercontent.com/85721522/194757069-05200652-5c43-41dc-96ef-631317ccbb86.png)


- unshift() = menambah element di index array pertama
![image](https://user-images.githubusercontent.com/85721522/194756671-1fd2a511-8566-41c9-baaa-fe470e4398a8.png)


- pop() = menghapus element terakhir array
![image](https://user-images.githubusercontent.com/85721522/194757233-1a488162-b72a-42cb-b4a7-058eeac7fbc4.png)


- shift() = menghapus element awal array
![image](https://user-images.githubusercontent.com/85721522/194757265-ae8ea43c-db68-45bf-97c3-98a3c0ba35d8.png)


- splice() = menghapus element tengah sesuai parameter
![image](https://user-images.githubusercontent.com/85721522/194757658-664058e6-4902-424b-8860-fac9b6d34de3.png)


- sort() = mengurutkan element secara ascending atau descending
![image](https://user-images.githubusercontent.com/85721522/194758364-6a371f24-a388-4cd4-aca0-76dad9bddb6b.png)


- length = mengetahui panjang array 
![image](https://user-images.githubusercontent.com/85721522/194758280-399768e5-1e75-4810-baae-551164a826ce.png)


### Array Looping 

for (variable of iterable)

- .forEach() = melakukan looping pada setiap elemen array tanpa membuat array baru
 
             = digunakan untuk menampilkan saja atau menyimpan ke database  
![image](https://user-images.githubusercontent.com/85721522/194759067-f2a5708a-e6c0-411b-97a5-61a46d79ab2b.png)


- .map() = melakukan looping setiap elemen array dengan membuat array baru

         = mengubah nilai array sebelumnya  
![image](https://user-images.githubusercontent.com/85721522/194758829-7eeb80c5-365c-4056-a9a7-d4b8be6a1c2d.png)


## Multidimensional Array Js
  - array of array atau ada array didalam array
  ![image](https://user-images.githubusercontent.com/85721522/194760990-09e5153c-15aa-448f-90ec-783dd5870a19.png)
  - Method dan perulangan sama seperti array 1 dimensi

## Object Js
  - tipe data pada variable yang menyimpan properti dan fungsi(method) 
  ![image](https://user-images.githubusercontent.com/85721522/194761610-ec637949-a3a4-45f8-a5f1-f720edbf9fb1.png)


### Cara mengakses objek

1. Dot notation
 
   syntax = namaobjek.property	
   
   ![image](https://user-images.githubusercontent.com/85721522/194761667-da527ebc-19d3-4268-8ab7-ffa83256a089.png)

	
2. Bracket

    syntax = namaobjek['property']
  
   cocok untuk property yang memiliki spasi
   
   ![image](https://user-images.githubusercontent.com/85721522/194761712-7d2f9a2b-bf91-47d0-a8c2-f7a81bf0f14e.png)


3. memanggil nama objek dengan variable

    syntax = namaobjek[namavariable]

    membuat property baru 
    
### Update Objek
- syntax diakses diluar objek
-  syntax namaobjek.newproperty
- membuat nilai dari property lama diganti
- syntax namaobjek.property = newvalue
- property/isi dari objek dapat diubah walaupun variable objek const

 ![image](https://user-images.githubusercontent.com/85721522/194762466-5939b5d0-e429-49de-9ab7-70d359552095.png)


### Menghapus property

syntax delete namaobjek.propertyyanngingindihapus

![image](https://user-images.githubusercontent.com/85721522/194762779-bf806aee-b954-45ba-873f-e5e4ea5dd428.png)


### Method pada Objek

- didalam objek terdapat function (method)

![image](https://user-images.githubusercontent.com/85721522/194762853-a84e306f-66ac-4fb6-8de7-c966c926b1dc.png)

- Object.keys(namaobjek) = memanggil property objek dalam bentuk array

![image](https://user-images.githubusercontent.com/85721522/194763190-224f8a41-219c-4773-9d86-3619386f90be.png)

- Object.values(namaobjek) = memanggil nilai nilai property

![image](https://user-images.githubusercontent.com/85721522/194763216-deb1a89e-891a-427e-9310-cce090b83687.png)


### Nested Objek 
 Didalam objek ada objek
 
 ![image](https://user-images.githubusercontent.com/85721522/194763611-8cd44248-fd74-444a-955c-acc4bb45e4e9.png)


### Loop objek

Syntax :

for(let namavariable in namaobjek){

 console.log(namaobjek[namavariable]);
 
}

### Array objek 
 - menampung banyak objek di dalam array 
 - API

- [{},{},{}]
- 
![image](https://user-images.githubusercontent.com/85721522/194764000-084dff9f-5a5a-45ee-96f2-1e88a8ee1bab.png)

## Recursive Js
- function yang memanggil dirinya sendiri sampai kondisi tertentu
- 
- digunakan yang berhubungan dengan calculation

![image](https://user-images.githubusercontent.com/85721522/194764343-b0508079-2358-445a-8c52-8b119a0fca9b.png)


## Asynchronous 
  - Intro
    - js single thread = 1 jalur yang menjalakan perintah/task 1 per 1 dan menyelesaikannya 
    
    ![image](https://user-images.githubusercontent.com/85721522/194765191-5c4348b5-c8a8-4c1a-88dd-5daed8ea9657.png)
      
    - blocking = perintah sebelummnya di jalankan terlebih dahulu lalu perintah perintah lain dijalankan
    - 
    ![image](https://user-images.githubusercontent.com/85721522/194765279-aa813869-1d9f-47a6-a69a-a674db1501eb.png)

    - non - blocking = mengizinkan perintah lain untuk dijalankan di suatu perintah yan masih dalam proses eksekusi 
    - 
    ![image](https://user-images.githubusercontent.com/85721522/194765307-742648e1-2feb-4f02-9dd5-ec523cdd648a.png)

    - syncronous = proses berurutan
    ![image](https://user-images.githubusercontent.com/85721522/194765326-ce6def48-e27a-493d-aaba-f8bff2ab6488.png)

    
    - asyncronous = proses yang dilakukan secara tidak berurutan dan bisa menjalakan perintah yang lain selagi suatu perintah di proses
      - single thread (concurrency)
    ![image](https://user-images.githubusercontent.com/85721522/194765363-a95bb5a3-ccde-443a-a31c-e62cbb5c4d97.png)
      - multi thread (paralelism)
      ![image](https://user-images.githubusercontent.com/85721522/194765427-d29173ab-4f8c-4f35-8a38-e5e399112beb.png)


    - ![image](https://user-images.githubusercontent.com/85721522/194765672-41f1d496-3a11-49d4-8d50-fb6f2beaefc2.png)

### js asyncronous
- ### callback = function yang dijadikan sebagai argumen
- callback terjadi karena adanya event loop 
- ![image](https://user-images.githubusercontent.com/85721522/194766487-54810130-ccb2-4db9-ae15-6d7917bc584f.png)

    -   ![image](https://user-images.githubusercontent.com/85721522/194766190-6c58c682-c8e8-40fa-9d96-9edbec3c4871.png)
    -   ![image](https://user-images.githubusercontent.com/85721522/194766207-a60a5bae-a906-439b-96af-cadfff7915e7.png)

- ### promises
  - 3 states promises
    - pending
    - rejected
    - fulfilled
- ### async await


## Web Storage


