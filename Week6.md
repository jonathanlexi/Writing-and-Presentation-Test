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

![image](https://user-images.githubusercontent.com/85721522/200178267-c802faa4-482d-4b3e-89be-b1bb07f95234.png)

![image](https://user-images.githubusercontent.com/85721522/200178340-7a95cfdc-557f-481e-abad-0d242bd74441.png)

![image](https://user-images.githubusercontent.com/85721522/200178360-e8976103-b295-4728-8763-bcfc2706947c.png)

![image](https://user-images.githubusercontent.com/85721522/200178376-9b4dab07-6a18-45d9-93e1-833715af413e.png)


## State Management React Redux



## Async Actions with Middleware dan Thunk
