# Resume Week 6

## React Router

  - Digunakan untuk pindah pindah page
  - Penggunaan router sama seperti a href membuat web menjadi dinamis 

### Cara menggunakan router
1.  Instal depedensi mpn-install react-router-dom 
  
    ![image](https://user-images.githubusercontent.com/85721522/200175922-21c717ee-e490-4f26-b654-f27f414b92b5.png)
    
    di file package json
  
2.  Menambah BrowserRouter dengan import {BrowserRouter} from "react-router-dom" terlebih dahulu di index.js 
3.  Membungkus komponen App dengan BrowserRouter
  
  ![image](https://user-images.githubusercontent.com/85721522/200175960-c20240df-b1ba-4e9e-b7f0-9dffe20ae139.png)

4.  import {Route,Routes,Link} from "react-router-dom"
  - Untuk menggunakan route dan link sebelumnya harus dibungkus dengan Route
  - Route untuk mengarahkan ke halaman tertentu sesuai path url dan element yang dipangil
    <Route path="/url" element={<element/>} />
  - Route terdiri dari single tag dan double tag
  - Route double tag digunakan untuk nested route
  
  ![image](https://user-images.githubusercontent.com/85721522/200175766-df3e651a-23db-4142-8aed-26689ab11aee.png)

  - Link digunakan untuk menuju ke element sesuai dengan url dan element yang sudah di route
  <Link to="/urlhome">Home</Link>
  
  ![image](https://user-images.githubusercontent.com/85721522/200175806-459d55e9-7d45-4f77-9821-3b26904a6196.png)

### Nested Route 
  - Dengan double tag Routes yang membungkus tag Route


    ![image](https://user-images.githubusercontent.com/85721522/200176769-a190e5b5-bf64-40c9-ab21-d771731979ab.png)
    
    ![image](https://user-images.githubusercontent.com/85721522/200176811-abdc3a53-93d2-40ed-bc1f-fdceb774a4b7.png)

###  URL Params
   
   - Mengambil value yang ada di dalam url atau sebagai params
   - Menggunakan hook useParams
   - Dapat digunakan untuk mendapatkan data dari api
   - / = root directory
   - /post/detail/1 = nested route

![image](https://user-images.githubusercontent.com/85721522/200178267-c802faa4-482d-4b3e-89be-b1bb07f95234.png)

![image](https://user-images.githubusercontent.com/85721522/200178340-7a95cfdc-557f-481e-abad-0d242bd74441.png)

![image](https://user-images.githubusercontent.com/85721522/200178360-e8976103-b295-4728-8763-bcfc2706947c.png)

![image](https://user-images.githubusercontent.com/85721522/200178376-9b4dab07-6a18-45d9-93e1-833715af413e.png)


## State Management React Redux

- redux adalah open source library js untuk mengelola dan membuat state terpusat.
- redux digunakan agar child child bisa saling mendapatkan data dengan adanya central data store
- instal depedensi redux (npm i redux react-redux)
- store,reducer,actions
    1. Store
      - tempat untuk menampung data agar data dapat digunakan diberbagai komponen
      
        ![image](https://user-images.githubusercontent.com/85721522/200237574-5111ae12-bf7b-4e3b-918e-675bfa730703.png)
        
        ![image](https://user-images.githubusercontent.com/85721522/200237645-baceb2ea-9d95-49b4-9b1f-7c2b6408a224.png)
    
    2. Reducer
      - reducer adalah function yang mengambil state terbaru dan argumen sebagai argumen dan mengembalikan ke state yang baru
      - (state, action) => newState

        ![image](https://user-images.githubusercontent.com/85721522/200237726-cc57dcd5-0dce-46c4-9e60-13f76bb39dd2.png)

    3. Actions
      - objek yang ada type yang menggambarkan apa yang terjadi 
      - field harus bertipe string ('feature/eventName')
      - action.payload ,yang dimana action memiliki nilai lain 

    ![image](https://user-images.githubusercontent.com/85721522/200237773-59badf30-908a-44bf-8078-7c166c1c1321.png)


- dispatch = penghubung antara component view ke action kemudian ke reducer
- selector berfungsi untuk menerima redux store state sebagai argumen dan return data berdasarkan state 

### Membuat store dengan createstore
- import createStore from redux library 
### file main.js, App dibungkus provider dengan store yang sudah dibuat 


## Async Actions dengan Middleware dan Thunk

- fungsi : Selain fungsi biasa (synchronous, dengan bantuan middleware kita juga bisa melakukan fungsi async seperti memanggil API. Karena itu middleware kita sekarang akan butuh bantuan package redux thunk

- Mengimplementasikan middleware, yang bertugas untuk menangani efek samping karena kita tidak boleh mengganggu action dan reducer yang harusnya pure function

- import thunk from 'redux-thunk'


