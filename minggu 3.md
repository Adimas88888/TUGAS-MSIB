### ADI MAS SETIAWAN(BACK END)


 ### **Javascript - Array<br>**
### Pengertian Array
> Array adalah tipe data list order yang dapat menyimpan tipe data apapun di dalamnya. Array dapat menyimpan tipe data String, Number, Boolean, dan lainnya.
### Contoh Array
```Javascript
let premiereLeague = ['Manchester United','Liverpool'.'Arsenal','Manchester City', 'Chelsea','Tottenham Hotspur']
console.log(premiereLeague)
```
### Membuat Array
> Array didefinisikan menggunakan square bracket [].
### Mengakses Array
- Array pada javascript dihitung dari index data ke-0.
- Data pertama adalah index ke-0.
- Contoh:
  ```Javascript
  let laukIni = ['Ayam Goreng','Ikan Goreng','Babi Guling']
  ```
  Penjelasan :
  - 'Ayam Goreng' adalah index ke-0
  - 'Ikan Goreng' adalah index ke-1
  - 'Babi Guling' adalah index ke-2
  - Kita bisa memanggi Ayam Goreng dengan
    ```Javascript
    console.log(laukIni[0])
    ```
### Update Array
```Javascript
let laukIni = ['Ayam Goreng','Ikan Goreng','Babi Guling']
laukIni[0] = 'Ayam Panggang'
console.log(laukIni) //Output : ['Ayam Panggang','Ikan Goreng','Babi Guling']
```
### Const in Array
- Jika menggunakan let, kita dapat mengubah array  dengan array baru dan konten nilai yang ada di dalam array dengan nilai lain
- Const tidak bisa melakukan update data. Namun pada Array kita dapat melakukan update konten nilai di dalam array (mutable).
- Yang tidak bisa adalah mengubah array dengan array yang baru jika menggunakan const
- Contoh :
  ```Javascript
  const merekMotor = ['Yamaha','Honda','Kawasaki']
  merekMotor = ['Suzuki'] //Output : Error
  ```
### Array Properties
- Properties adalah fitur yang sudah disediakan oleh Javascript untuk memudahkan developer.
- .length Properties
  - length akan mengembalikan nilai dari jumlah panjang data suatu array.
  - Contoh :
    ```Javascript
    const merekMotor = ['Yamaha','Honda','Kawasaki']
    console.log(merekMotor.length) //Output : 3
    ```
### Array Method
- Array memiliki method atau biasa disebut built-in methods.
- Artinya Javascript sudah memudahkan kita dengan menyediakan function/method umum yang bisa kita gunakan.
- Kita tidak perlu membuat function lagi jika method yang kita butuhkan sudah tersedia.
- Contoh Array Built-in Methods :
  - .push()
  > Method untuk menambahkan item  array pada urutan yang paling akhir.
  - .pop()
  > Method yang menghapus item array index terakhir.
  - .shift()
  > Method untuk menghapus item Array pada index pertama
  - .unshift()
  > Method untuk menambahkan item Array pada index pertama
  - .sort()
  > Method untuk mengurutkan secara Ascending atau Descending Alphanumeric
### Array - Looping
- Array memiliki built in methods untuk melakukan looping yaitu .map() dan .forEach()
1. .map()
> Melakukan perulangan/looping dengan membuat array baru.
Contoh :
```Javascript
let angka = [1,2,3,4]
let kaliDua = angka.map(num => {
return num * 2
})
//Output : [2,4,6,8]
```
2. forEach()
> method untuk melakukan looping pada setiap elemen array.
Contoh :
```Javascript
const merekMotor = ['Yamaha','Honda','Kawasaki']
const forEach(element =>{
  console.log(element)
})
//Output : 'Yamaha','Honda','Kawasaki'
```
### Javascript - Multidimensional Array
- Multidimensional Array bisa dianalogikan dengan array of array. Ada array di dalam array.
  <br>Contoh :
  ```Javascript
  let inventory = [
  ['Celana',5],
  ['Baju', 10]
  ]
  
  console.log(inventory)
  ```
- Akses index multidimensional array
  <br>Contoh :
    ```Javascript
    let inventory = [
    ['Celana',5],
    ['Baju', 10]
    ]
  
    console.log(inventory[1][0]) //Output : Celana
    ```
- Operation using map in multidimensional array
  <br>Contoh :
  ```Javascript
  let inventory = [
  ['Celana',5],
  ['Baju', 10]
  ]
  
  inventory.map(dataInventory => {
    terjual = 100 - dataInventory[1]
    dataInventory[2] = terjual
  })
  
  console.table(inventory)
  ```
  Result :
  <br>![image](https://user-images.githubusercontent.com/100120189/194701355-20c2fb76-7a8d-46df-ac96-060f2d3c88fd.png)
- Looping For Multidimensional Array
  <br>Contoh :
  ```Javascript
  let inventory = [
  ['Celana',5],
  ['Baju', 10]
  ]
  
  inventory.forEach(baris) => {
    baris.forEach(column) => {
    console.log(column)
    }
  }
  //Output :
  //Celana
  //5
  //Baju
  //10
  ```
  ### **JavaScript Intermediate - Object & Array of Object**
### **Object**

<br>Pada programming, object adalah sebuah tipe data pada variabel yang menyimpan properti dan fungsi (method)

- **Properti** adalah data lengkap dari sebuah object.
- **Method** adalah action dari sebuah object. Apa saja yang dapat dilakukan dari suatu object.
- Contoh Object Mobil beserta properti dan methodnya
  - Properti :
  1. name = 'Fiat'
  2. weight = "850kg"
  3. color = "white"
  - Method :
  1. start()
  2. drive()
  3. stop()
- Membuat sebuah object
  <br> object dapat diassign kedalam sebuah variable
  ```
  let person = {}; //object person
  ```
  <br> didalam object dapat menyimpan properti dengan tipe data apapun
  ```
  let person = {
    name: 'Naruto',
    age: 20,
    isVerified; true,
  };
  ```
- Mengakses Object dan Properti Object
  ```
  console.log(person); //mengakses seluruh object
  console.log(person.name); //mengakses properti object
  ```
  <br> bisa menggunakan bracket notation saat memanggil properti sebuah object
  ```
  console.log(person['name']);
  ```
- Update Object
  <br> dapat mengupdate value dari key yang sudah ada serta dapat menambahkan key dan value baru
  ```
  let person = {
  name: 'Naruto',
  age: 20,
  isVerified: true,
  };
  ```
  - update current key
    ```
    person.age = 23;
    ```
  - menambahkan key dan value baru
    ```
    person.address = 'Tokyo, Jepang'
    ```
  - memanggil object
    ```
    console.log(person);
    ```
- menghapus properti object

  ```
  delete person.age;
  ```

- **Method**
  <br>contoh:
  ```
  const greeting = {
    welcome: function() {
        return 'halo selamat datang'
    },
    afterPay: function() {
        return 'Thank You'
    },
   };
   console.log(greeting.welcome()); //Output : 'halo selamat datang'
   console.log(greeting.afterPay()); //Output : 'Thank You'
  ```
- **Nested Object**
  <br> Object yang berasal dari turunan obect lainnya
  <br> contoh :

  ```
  let buku = {
      judul: "jago ngoding",
      tahun: 2015,
      penulis: {
        penulis1: {
            nama: "reyhan",
            kota: "jakarta",
        },
        penulis2: {
            nama: "reza",
            kota: "bandung",
        },
      },
  };
  console.log(buku); //menampilkan semua object buku
  console.log(buku.penulis.penulis1.nama); //Output: reyhan
  console.log(buku.penulis.penulis2.kota); //Output: Bandung
  ```

- **Looping Object**

  ```
    for(let key in object){
    };
  ```

  <br>contoh, coding lanjutan dari nested

  ```
  for(let key in buku.penulis.penulis1){
    console.log(buku.penulis.penulis1[key]);
  } //Output:
  reyhan
  jakarta
  ```

- **Array of Object**
  <br> contoh

  ```
  let buku = {
    judul: "jago ngoding",
    tahun: 2015,
    penulis: {
        penulis1: {
            nama: "reyhan",
            kota: "jakarta",
        },
        penulis2: {
            nama: "reza",
            kota: "bandung",
        },
    },
  };
  //Array of Object
  let data = buku.map((el)) => {
    console.log(el.nama);
  }); // Output :
  reyhan
  reza
  ```
### **Rekrusif dan Modules**
- **Rekrusif** adalah function atau algoritma yang memanggil dirinya sendiri sampai kondisi tertentu. Rekrusif ini mirip seperti looping. Misalnya pada gambar ada gambar di dalam gambar. Terdapat 2 kunci pada rekrusif,yaitu base case atau titik berhenti dan recrusion case atau titik memanggil function. Contoh script :
  ```
  Menampilkan bilangan 1 2 3 4 5
  
  function deretAngka(n){
   if (n == 1) {
     console.log(n)
   } else {
     deretAngka(n-1)
     console.log(n);
    }
  }
  deretAngka(3)
  
  Atau contoh lain :
  Mencari angka faktorial
  Misalnya 5!
  Solusinya jika dijabarkan 5 x 4 x 3 x 2 x 1

  function faktorial(n) {
    if (n == 1) {
      return 1
    } else {
      return n * faktorial(n - 1)
    }
  }
  console.log(faktorial(3))
  //Output = 6
  ```
- **Modules** adalah cara untuk memisahkan kode ke file yang berbeda. Keuntungan dari modules yaitu mudah untuk mengelola kode serta kode tidak menumpuk di dalam satu file. Terdapat 2 kata kunci pada modules yaitu export dan import. Contoh script :
  ```
  // File Jepang.js
  export let motor = ["suzuki", "yamaha", "honda", "kawasaki"]
  
  let entertainment = ["anime", "manga", "wibu", "dorama"]
  export default entertainment
  
  export function sayHello() {
   console.log("hallooo")
  }
  
  import {apple} from './amerika.js';
   console.log(apple);
  
  // File Indonesia.js
  import {motor} from "./Jepang.js"
   console.log(motor);
   
  import Entertainment, { motor as motorJepang, sayHello  } from "./jepang.js"
  console.log(Entertainment);
  
  // File Amerika.js
  let apple = ["iphone", "macbook", "imac"]
    export {apple}
  
  Berdasarkan script diatas,
  - Indonesia hanya bisa import, karena dia file utama.
  - Jepang bisa melakukan import dan export.
  - Amerika hanya melakukan export.
  ```
- Hal hal yang harus dilakukan saat membuat modules adalah menambahkan type="module" pada script utama, lalu siapkan script ke-2 dan sebagainya untuk melakukan export, serta lakukan import pada file atau script utama.

### **Asynchronous**

Asynchronus 
Proses yang dilakukan secara tidak berurutan. Jika proses terlalu panjang, akan diselat oleh proses yang lebih singkat 
Synchronous : proses yg berurutam (proses keseluruhan) 
Blocking : proses yg gabisa diselat
Proses concurrent yg tidak sama dengan multitask/multithread
Secara umum, bahasa pemrograman berjalan secara synchronous. JS memiliki kelebihan dapat menjalankan sebuah proses tanpa harus berurutan.
Tiap engine JS terdiri dari 2 bagian, heap dan stack. Bersifat first in last out.

JS asynchronous memiliki 3 kunci utama 
1.	Callback 
Callback : function yg dijadikan sebagai argumen
Ketika sesuatu memerlukan waktu yang lama, maka dia akan masuk kedalam callback queue lalu menjalankan proses yang berada di belakangnya. Jika proses yg belakang sudah selesai, maka engine akan memeriksa yang ada didalam callback queue untuk dijalankan.
 <br>![image](https://github.com/Adimas88888/TUGAS-MSIB/blob/3ff0bf2d039472fff5a083066df0d43bd0834345/Screenshot_58.png)

	
Contoh 
```javascript
Console.log(???A???)
setTimeout( () => {
Console.log(???B???) 
}, 1000)
Console.log(???C???)
```
Output : 
 
 yang dikerjakan console.log(???C???) terlebih dahulu karena console.log(???B???) memerlukan waktu sebelum diproses
2.	Promises 
Kejadian yang telah selesai atau gagal dalam operasi asynchronous yang menghasilkan nilai
Saat on progress progress dalam fase pending. Jika gagal maka status asynchronous menjadi rejected. Jika kejadian dari event asynchronous telah berhasil, maka status fulfilled.
```javascript
Let nontonPromise = new Promise ((resolve, reject) => {
resolve(???nonton terpenuhi???)
reject(???gagal???)
})
Console.log(???A???)
nontonPromise
.then(result =>{
console.log(result)
})
.catch((err) => {
Console.log(err)
})
Console.log(???C???)
```
 
Jika ingin memberi parameter, harus pake function 
```javascript
Let nonton = () => {
Return new Promise((resolve, reject) => {
If (kondisi == ???jalan???) {
Resolve (???nonton terpenuhi???)
}
Reject (???batal nonton???)
})
}
Nonton(???jalan???)
.then(result => {
Console.log(result)
})
.catch(err => {
Console.log(err)
})
```


3.	Async await
Async/await adalah fitur yang hadir sejak ES2017. Fitur ini mempermudah kita dalam menangani proses asynchronous.Async/Await merupakan sebuah syntax khusus yang digunakan untuk menangani Promise agar penulisan code lebih efisien dan rapih.Async/Await terbagi menjadi Async dan Await, mari kita lihat contohnya.

```
const getAllUser = async ()=> {
	const data = await getUser()
	console.log(data)
}
```

Pada contoh diatas, pertama kita memiliki function dengan menambahkan async didepan function yang mana berfungsi untuk menjadikan function tersebut asynchronous, dan await berfungsi menunda eksekusi hingga proses asynchronous selesai, dari kode di atas berarti console.log(data) tidak akan di eksekusi sebelum proses getUser() selesai. await juga bisa digunakan berkali-kali di dalam function.

Penjelasan penggunaan Async Await
1.	Async/Await adalah salah satu cara untuk mengatasai masalah asynchronous pada Javascript selain menggunakan callback dan promise.
2.	Pada implementasi Async/Await, kita menggunakan kata kunci async sebelum fungsi. Await sendiri hanya bisa digunakan pada fungsi yang menggunakan async.
3.	Untuk menggunakan Async/Await, kembalian dari suatu fungsi harus merupakan suatu Promise. Async/Await tidak dapat berdiri tanpa adanya Promise.
4.	Tidak seperti Promise, dengan Async/Await maka suatu baris kode dapat tersusun rapi mirip dengan kode yang sifatnya synchronous.
5.	Setiap baris yang menggunakan await, akan ditunggu sampai Asynchronous Promise tersebut di resolve.

Error Handling Async/Await
Untuk menghandle error  Async/Await kita dapat menggunakan try catch di dalam function yang kita buat, sehingga jika terjadi error kita dapat menangkap errornya dalam block catch, berikut contoh penggunaannya.

```
const getAllUser = async ()=> {
	try {
		const result = await getUser()
		console.log(result)
	} catch (error) {
		console.log(error)
	}
}
```
## JavaScript Intermediate Web Storage
- Ada beberapa cara untuk menyimpan data pengguna seperti pencarian, artikel berita, dan lain-lain ke lokal (browser) menggunakan web storage seperti cookies, local storage, dan session storage. Data ini dimanfaatkan oleh situs web tersebut untuk merekam kebiasaan pengguna agar dapat memberikan rekomendasi sesuai preferensi si pengguna tersebut.
#### Cookies
- Cookies adalah data kecil yang dikirim dari situs web dan disimpan di komputer kita oleh web browser saat kita menjelajah. Disebut data kecil karena maksimum data yang dapat disimpan dalam cookies adalah 4096 bytes (4 KB).
- Biasanya data yang disimpan di cookies adalah access token pengguna saat login atau data pencarian saat melakukan pencarian pada situs web tertentu. Hal ini yang biasanya dilakukan oleh situs pencarian untuk melacak pencarian kita dan menampilkan iklan yang berhubungan dengan pencarian kita sebelumnnya.
- Namun ada beberapa kekurangan yang perlu kita perhatikan mengenai cookies di antaranya:
  1. Setiap kita mengakses situs web, cookies juga kembali dikirim sehingga memperlambat aplikasi web kamu dengan mengirimkan data yang sama.
  2. Cookies disertakan pada setiap HTTP request, sehingga mengirimkan data yang tidak dienkripsi melalui internet, maka saat kita ingin menyimpan data dalam cookies kita harus mengenkripsinya terlebih dahulu.
  3. Cookies hanya dapat menyimpan data sebanyak 4KB.
  4. Lalu cookies juga memiliki tanggal kadaluarsa. Tanggal ini telah ditentukan sehingga web browser bisa menghapus cookies jika tanggal sudah kadaluarsa atau tidak dibutuhkan.
- Kita dapat memanfaatkan jenis web storage yang lain untuk mengatasi kekurangan yang dimiliki cookies.
#### Local Storage & Session Storage
- Pernahkah kita saat melakukan pencarian pada sebuah situs lalu situs tersebut menampilkan riwayat pencarian kita? Iya, data pencarian tersebut disimpan ke dalam local storage untuk diolah menjadi riwayat pencarian. Itulah salah satu contoh penerapan dari local storage pada aplikasi web.
- Berbeda dengan local storage, walaupun masuk ke dalam web storage, data yang tersimpan pada session storage akan hilang ketika session dari sebuah laman berakhir.
- Karakteristik Local Storage:
  1. Menyimpan data tanpa tanggal kadaluarsa.
  2. Data tidak akan dihapus ketika web browser ditutup dan akan tersedia seterusnya selama kita tidak menghapus data local storage pada web browser.
  3. Dapat menyimpan data hingga 5MB.
  4. Hanya dapat menyimpan data string.
- Sedangkan Karakteristik Session Storage:
  1. Data yang disimpan pada session storage akan terus tersimpan selama browser terbuka dan tidak hilang jika laman di-reload.
  2. Membuka banyak tab/window dengan URL yang sama, akan menciptakan session storage yang berbeda di masing-masing tab/window.
  3. Menutup tab/window akan mengakhiri session dan menghapus data yang tersimpan di session storage pada tab/window tersebut.
  4. Data yang tersimpan dalam session storage harus berbentuk string.
  5. Hanya dapat menyimpan data sebanyak 5MB.
##### Mengakses Local Storage & Session Storage
1. Local Storage
  - Menyimpan Data
  Untuk menyimpan data pada local storage, kita menggunakan method `setItem()` yang membutuhkan 2 parameter. Parameter pertama adalah key yang ingin kita simpan dan parameter kedua adalah data (value) dari key yang akan disimpan.
    ```javascript
    localStorage.setItem('key', value);
    ```
  - Mengambil Data
  Untuk mengambil data yang telah tersimpan pada local storage, kita dapat menggunakan method `getItem()` yang membutuhkan 1 parameter. Parameter tersebut adalah key dari data yang kita inginkan.
      ```javascript
      localStorage.getItem('key');
      ```
  - Menghapus Data
  Untuk menghapus data yang telah tersimpan pada local storage, kita dapat menggunakan method `removeItem()` yang membutuhkan 1 parameter. Parameter tersebut adalah key dari data yang ingin kita hapus.
    ```javascript
    // menghapus key tertentu
    localStorage.removeItem("key");

    // menghapus semua key
    localStorage.clear();
    ```
2. Session Storage
  - Menyimpan Data
  Sama dengan local storage, sintaks untuk menyimpan data pada session storage adalah sebagai berikut:
    ```javascript
    // menambah session storage
    sessionStorage.setItem('key', value);
    ```
  - Mengambil Data 
  Sama seperti local storage, cara mendapatkan data dari session storage juga menggunakan `getItem(),` seperti berikut ini:
    ```javascript
    // mendapatkan session storage
    sessionStorage.getItem('key');
    ```
  - Menghapus Data
  Syntax untuk menghapus data dari session storage ada 2, yaitu:
    ```javascript
    // menghapus session storage satu persatu berdasarkan key
    sessionStorage.removeItem('key');

    // menghapus seluruh session storage sekaligus
    sessionStorage.clear();
    ```



