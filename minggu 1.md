### ADI MAS SETIAWAN(BACK END)

### **----- Unix Command Line -----**

- **Shell** adalah program yang digunakan untuk berkomunikasi atau memerintah sistem
- **CLI (_Command Line Interface_)** adalah sebuah program yang memungkinkan user mengetik perintah atau command yang akan memerintahkan perangkat komputer untuk melakukan suatu tugas tertentu
- **Cara mengakses CLI di terminal** : User dan komputer dihubungkan dengan namanya terminal, yaitu tempat/aplikasi dimana user dapat mengetikan atau memberikan suatu perintah
- **File System** berfungsi untuk menyediakan mekanisme untuk penyimpanan data dan program yang dimiliki oleh sistem operasi serta seluruh pengguna dari sistem komputer

* Beberapa Command pada CLI beserta fungsinya :
  - Navigation
    - **ls** (_list_) yaitu command untuk melihat isi file yang ada di sebuah directory
  - File Manipulation
    - **touch** yaitu command untuk membuat sebuah file
    - **cp** (_copy_) yaitu command untuk mengcopy files atau directory
    - **mv** (_move_) yaitu command untuk memindahkan file atau directory. Bisa juga digunakan untuk rename file atau directory
    - **rm** (_remove_) yaitu command untuk menghapus file atau directory
  - Folder / Directory Manipulation
    - **mkdir** yaitu command untuk membuat sebuah directory
    - **cd** (_change directory_) yaitu command untuk berpindah directory
    - **pwd** (_Print working directory_) yaitu command untuk melihat current working directory
  - Text
    - **echo** yaitu command untuk menampilkan sesuatu kata atau kalimat dalam sebuah file
    - **cat** yaitu command untuk melihat isi sebuah file
    - **nano** yaitu command untuk menampilkan konten yang dapat diedit

### **----- Git & Github Dasar -----**

- **Git** merupakan aplikasi yang dapat melacak suatu perubahan yang terjadi di suatu folder ataupun file. Biasanya digunakan oleh programmer sebagai tempat untuk menyimpan file program mereka karena lebih efektif
- **Github** merupakan vendor penyedia layanan git yang dimiliki oleh microsoft atau secara definisi merupakan layanan hosting berbasis web sebagai repositori git
- **Alasan wajib menggunakan Git & Github**
  - Alasan utamanya adalah sepandai apapun programmer, tidak akan mampu untuk mengerjakan semuanya sendiri selamanya. Maka dari itu dengan menggunakan Git & Github akan memudahkan programmer untuk bisa bekerja sama dalam sebuah tim. Tujuan besarnya adalah programmer bisa berkolaborasi dengan programmer lainnya dengan mengerjakan proyek yang sama tanpa harus repot copy paste folder aplikasi yang terupdate
- **Command di dalam Git & Github**
  - **git init** <_nama_proyek_>, untuk membuat repositori baru
    - contoh : git init proyek01
  - **git commit** untuk melakukan commit atau menyimpan perubahan pada version control pada git. Bisa juga menambahkan pesan untuk memberikan checkout pada setiap perubahan
    - contoh : git commit
    - contoh : git commit -m "Commit Pertama"
  - **git push origin** untuk mempublish file atau aplikasi ke github
    - contoh : git push origin
  - **git clone** untuk melakukan cloning dari github ke komputer atau local
    - contoh : git clone https://github.com/shehaannisa/cobagit.git

### **----- HTML (_Hypertext Markup Language_) -----**

- **HTML**
  <br> merupakan bahasa komputer yang digunakan untuk membuat kerangka atau struktur untuk Web pages (halaman website) di internet.
- **Bagaimana peran HTML pada web development?** : Web browser seperti Chrome, Firefox, Edge, Safari, atau Opera akan membaca dokumen HTML. Dokumen HTML yang berisi tag-tag HTML akan memberitahu browser bagaimana cara menampilkan sebuah konten
- **Kerangka HTML**
  - Syntax dibawah ini biasa disebut dengan kerangka bahasa pemrograman HTML. Didalam website selalu ada title untuk tiap-tiap web, untuk memasukkan title didalam web kamu harus mengetikkan diantara tag title (dapat diisikan dengan nama website kamu atau yang lainnya). Untuk memasukkan konten-konten, kamu dapat memasukkannya atau mengetikkannya didalam program tepat diantara tag body

```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Belajar HTML</title>
  </head>
  <body>
    <h1>Hi.. I'm Sheha</h1>
    <h2>Track Back End Development</h2>
    <p>
      Back end merupakan sisi server atau server side dari sebuah website atau aplikasi. <br />
      Jadi, back end developer adalah seorang yang memiliki keahlian untuk merancang atau <br />
      mengembangkan software di sisi server yang berkaitan dengan logika serta database
    </p>
    <img src="https://media.istockphoto.com/photos/encryption-your-data-binary-code-and-digital-lock-hacker-attack-and-picture-id1346223165?b=1&k=20&m=1346223165&s=170667a&w=0&h=q6W4oLmto2l8of4xCGXI2aYdSBbLbgC5mZs1sFUWgj8=" />
    <ol type="a">
      <li>Linkedin</li>
      <li>Twitter</li>
      <li>Instagram</li>
    </ol>
  </body>
</html>

```

- **Tag HTML**

  > Tag adalah sebuah penanda awalan dan akhiran dari sebuah elemen di HTML. Tag dibuat dengan kurung siku (<...>), lalu di dalamnya berisi nama tag dan kadang juga ditambahkan dengan atribut. Tag selalu ditulis berpasangan. Ada tag pembuka dan ada tag penutupnya. Namun, ada juga beberapa tag yang tidak memiliki pasangan penutup. Tag penutup ditulis dengan menambahkan garis miring (/) di depan nama tag.
  > `Tag Pembuka <h1> Tag Penutup </h1>`

  - **Single Tag**
    > `contoh : </br>`
  - **HTML Double Tag**
    > `contoh : <p> </p>`
  - **HTML Comment**
    > `contoh : <!-- -->`
  - **HTML Attributes** : properties dari sebuah element HTML
    > `contohnya : id, class, name`

- **Membuat Tabel**

```
<!DOCTYPE html>
<html lang="en">
<table border="1">
       <thead>
           <tr>
               <td>Nama</td>
               <td>Umur</td>
               <td>Jurusan</td>
           </tr>
       </thead>
       <tbody>
           <tr>
               <td>Sheha Annisa</td>
               <td>20 Tahun</td>
               <td>Teknik Informatika</td>
           </tr>
       </tbody>
   </table>
</html>
```

- **Penjelasan** :

```- <thead> : membungkus konten bagian judul atau kepala tabel
    - <tr> : membuat baris pada tabel
    - <td> : membuat kolom di setiap baris pada tabel
    - <tbody> : membungkus konten bagian isi atau tubuh dari tabel
```

- **Beberapa Tag Semantic HTML**
  - **Element Header**
  ```
  <header>
    <h1>Belajar HTML</h1>
    <p>Belajar HTML untuk Pemula</p>
  </header>
  ```
  - **Element Nav**
  ```
  <nav>
    <a href="#">HTML</a> |
    <a href="#">CSS</a> |
    <a href="#">Javascript</a> |
    <a href="#">PHP</a> |
    <a href="#">SQL</a>
  </nav>
  ```
  - **Element Footer**
  ```
  <footer>
    Copyright & copy; 2022 - Sheha_
  </footer>
  ```
  - **Element Section**
  ```
   <section>
        <h3>Subjudul 1</h3>
        <p>Lorem ipsum, dolor sit amet consectetur adipisicing, elit. Laudantium unde ipsum molestiae deleniti iusto eos id vel voluptates, exercitationem autem!</p>
    </section>
  ```
- **Deploy HTML menggunakan Netlify**

1. Buat repository GitHub yang dalamnya berisi file HTML yang sudah dibuat tadi
2. Buka https://app.netlify.com/ di browser, lalu login dengan akun GitHub (jika belum punya akun daftar terlebih dahulu)
3. Kemudian pilih "Sites" dan pilih "Import from Git"
4. Pilih GitHub
5. pilih repository yang ingin di deploy
6. Pilih branch yang ingin dideploy, kemudian klik Deploy Site
7. File HTML sudah berhasil dideploy

### **----- CSS (_Cascading Style Sheets_) -----**

- **CSS** adalah bahasa yang digunakan untuk mendesain halaman website
- **Beberapa cara menyisipkan CSS kedalam HTML**

1. **Inline Styles** : menambahkan CSS pada atribute element HTML dengan menggunakan tag < style > pada file HTML

- contoh :

```

<!DOCTYPE html>
<html>
  <head>
    <title>
      Website Pertamaku
    </title>
  </head>
  <body>
    <h1 style="color:blue;">Selamat Datang</h1>
  </body>
</html>
```

2. **Internal CSS** : menggunakan element < style > untuk menyisipkan kode CSS. Element < style > tersebut diletakkan di dalam element

- contoh :

```
<!DOCTYPE html>
<html>
  <head>
    <title>Website Pertamaku</title>
    <style>
      body {
        background-color: yellow;
      }
      h1 {
        color: blue;
      }
      p {
        color: red;
      }
    </style>
  </head>
  <body>
    <h1>Website Pertama Sheha</h1>
    <p>Selamat Datang</p>
  </body>
</html>
```

3. **External CSS** : sebuah file CSS terpisah yang disambungkan dengan file HTML dengan menggunakan element < link >

- contoh :

  - file .HTML nya :

  ```
  <!DOCTYPE html>
  <html>
  <head>
    <title>External CSS</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <h1>Saya bahagia</h1>
  </body>
  </html>
  ```

  - file .CSS nya :

  ```
  h1 {
  color: brown;
  }
  ```

- **Syntax Dasar CSS**
  - **Selektor** :
  - Contoh :
    ```
    h1 {
          color: red;
      }
    ```
    > Selektor dapat berupa nama tag, class, id, dan atribut
  - **Contoh :**
- Selektor dengan nama tag
  ```
  h2 {
    color: blue
  }
  ```
- Selektor dengan class
  ```
  .bg-yellow {
      backgound-color: yellow;
  }
  ```
- Selektor dengan ID elemen
  ```
  #header {
      background: grey;
  }
  ```
- Selektor dengan Atribut
  ```
  input[type=text]{
      background: yellow;
  }
  ```
- **CSS Flexbox** adalah cara untuk mengatur layout, memiliki kemampuan untuk menyesuaikan layout secara otomatis
  - **Ordering & Orientation**
    - **flex-direction** : digunakan untuk mengatur letak item child
      <br> ![1](https://www.gamelab.id/uploads/modules/NEWS/817/Group%2021.png?1628228538451)
      <br> ![2](https://www.gamelab.id/uploads/modules/NEWS/817/Group%2022.png?1628228559883)
      1. row (default): secara default letak item child membentuk sebuah baris dari kiri ke kanan.
      2. row-reverse: letak item child membentuk sebuah baris dari kanan ke kiri
      3. column: letak item child membentuk sebuah baris dari atas ke bawah
      4. column-reverse: letak item child membentuk sebuah baris dari bawah ke atas
    - **flex-wrap** : flex secara default akan membuat tata letak item children dalam 1 line saja. flex akan menyesuaikan space yang ada. Namun jika kamu ingin membatasi jumlah item children dalam 1 line lalu item children yang lain akan pindah ke posisi line yang baru, maka kita bisa menggunakan flex-wrap
      <br> ![3](https://www.gamelab.id/uploads/modules/NEWS/817/Group%2023.png?1628228598739)
      <br> ![4](https://www.gamelab.id/uploads/modules/NEWS/817/Group%2024.png?1628228613938)
      1. no-wrap (default): secara default , flex tidak menggunakan flex-wrap
      2. wrap: flex item akan memiliki beberapa line dari atas ke bawah jika space dalam 1 line sudah full width.
      3. wrap-reverse: kebalikan dari wrap yaitu flex item akan memiliki beberapa line dari bawah ke atas jika space dalam 1 line sudah full width
    - **flex-flow** : digunakan sebagai shortcut untuk set up flex-direction dan flex-wrap bersamaan
    - **order** : berfungsi untuk ordering item mana yang ingin kita atur posisinya berdasarkan urutan order
      <br>![5](https://lh3.googleusercontent.com/F_rkGnqbpaoUvmoTyTnIzNuqG2345-FKNUdMXV62mDR-ZhMb4jTj5K7Ip5y5lg80h9KuuxH9KjBVlPnu02HB7RYWKaEq2xgdauNPFK1uqiJl-dWoIw5R32fCmTPkCOnpXqtxTx0)
      1. 1 : Item child yang di set order -1, maka item child tersebut akan berada di ordering paling awal atau paling kiri
      2. 2 : Flex secara default memiliki order 0 pada setiap item child. Ini berarti 0 akan membuat item child sesuai urutan pada html
      3. 5: Item child yang di set order 1, maka item child tersebut akan berada di ordering paling akhir atau paling kanan
  - Alignment
    - justify-content, memiliki 6 value, yaitu:
      - flex-start
      - flex-end
      - center
      - space-between
      - space-around
      - space-evenly
    - align-items, memiliki 5 value
      - flex-start
      - flex-end
      - center
      - baseline
      - stretch
    - align-self, memiliki 5 value yang sama dengan align-items
      - flex-start
      - flex-end
      - center
      - baseline
      - stretch
    - align-content
      - properti align-content memiliki konsep yang sama seperti justify-content
      - align-content digunakan untuk mengatur tata letak dan space antar item child secara vertikal atau cross axis.
      - align-content akan berjalan jika item lebih dari 1 line/baris.
      - align-content memiliki value yang sama dengan justify-content. bedanya ada 1 tambahan value yaitu stretch.
  - Flexibility
    - flex-grow
    - flex-shrink
    - flex-basis

### **----- Algoritma -----**

- **Algoritma**
  > adalah langkah-langkah yang dilakukan untuk menyelesaikan masalah, sedangkan struktur data untuk mengelola/memanajemen sebuah data
- **Jenis Proses Algoritma**
  - Sequence : Instruksi yang dijalankan secara berurutan
  - Selection : Instruksi yang dijalankan jika memenuhi suatu kondisi
  - Iteration : Instruksi yang berulang kali dijalankan selama memenuhi suatu kondisi
  - Concurrent : Instruksi yang dijalankan secara bersamaan
- **Penyajian Algoritma**
  - Deskriptif
  - Flow Chart
  - PseudoCode adalah menuliskan algoritma dengan umumnya bahasa inggris sebelum kita implementasikan ke bahasa pemograman tertentu.
- **Algoritma Sederhana**
  <br> Membuat algoritma dari kalkulator penambahan

1. Step 1: Mulai
2. Step 2 : Deklarasi variable angka_1, angka_2
3. Step 3 : Membaca nilai dari variable angka_1 dan angka_2
4. Step 4 : Panggil dan lakukan penambahan pada variable sum (sum = angka_1 + angka_2)
5. Step 5 : Menampilkan hasil sum
6. Step 6 : Selesai </br>
   <br> Berikut merupakan contoh penerapan algoritma diatas dalam JavaScript

```
console.log() // output :
```
- **PseudoCode sederhana menggunakan JavaScript**
```
const nama = "Sheha";
console.log("Nama Saya " + nama);
// Output : 
// Nama Saya Sheha
```
- **Big-O Notation** adalah sebuah cara atau metode untuk melakukan analisa terhadap sebuah algoritma pemrograman terhadap waktu eksekusi. Tentang seberapa efisien dan kompleksitas barisan kode dalam dimensi waktu

### **----- JavaScript -----**

1. **Intro to JavaScript**
   - Javascript dapat membuat website menjadi interaktif dan dinamis
   - Menjalankan JavaScript : Javascript dijalankan melalui browser pada device setiap user. misalnya chrome dan Mozilla firefox
   - Syntax dan Statement : menggunakan syntax tertentu untuk membuat statement program, instruksi untuk djalankan/dieksekusi oleh web browser, compiler, ataupun intrepreter
   - **Contoh Syntax JavaScript**
     - Alert()
     - Prompt()
     - Confirm()
     - Console.log
     - Console log juga tempat kita untuk melakukan debugging (mengetahui error pada code) pada pemograman web
   - **Tipe data** adalah klasifikasi yang kita berikan untuk berbagai macam data yang di gunakan dalam programing ada 6 yaitu
     - number
     <br> Tipe data number adalah tipe data yang mengandung semua angka termasuk angka desimal
     - string
     <br> Tipe data string adalah grup karakter yang ada pada keyboard laptop/PC kita yaitu letters (huruf), number (angka), spaces (spasi), symbol, dan lainnya
     - boolean
     <br> Tipe data boolean adalah tipe data yang hanya mempunyai 2 buah nilai
     - null
     <br> Tipe data yang diartikan bahwa sebuah variable/data tidak memiliki nilai
     - undefined
     <br> Tipe data yang merepresentasikan varibel/data yang tidak memiliki nilai
     - object
     <br> Koleksi data yang saling berhubungan (related). Tipe data pbject dapat menyimpan data dengan tipe data apapun (number, string, boolean, dan lainnya)
   - **Operator**.
     - Assignment (=)
       <br>Menyimpan sebuah nilai dalam variable
       ```
        let angka = 1;
       ```
     - Mathematical Assignment Operator
     ```
     let a = 4;
     a = a+1
     console.log(a); //output 5
     ```
     - Increment dan Decrement
       <br>Digunakan untuk menambah atau mengurangi sebuah nilai. Banyak tambah/kurangnya yaitu 1
     ```
     let a = 4;
     a++;
     console.log(a); //output 5
     ```
     ```
     let a = 4;
     a--;
     console.log(a); //output 3
     ```
     - Arithmetic Operator
       <br>Merupakan operator yang melibatkan operasi matematika -
       <br> Tambah (+), Kurang (-), Perkalian (\*), Pembagian (/), Modulus (%)
       ```
       console.log(7 + 3) // output : 10
       console.log(2 - 1) // output : 1
       console.log(5 * 2) // output : 10
       console.log(15 / 3) // output : 5
       console.log(8 % 2) // output : 0
       ```
     - Comparison
       <br>Operator yang membandingkan dua nilai. Hasilnya akan bersifat true atau false.
       <br> - Lebih kecil dari : <
       <br> - Lebih besar dari: >
       <br> - Lebih kecil atau sama dengan: <=
       <br> - Lebih besar atau sama dengan: >=
       <br> - Sama dengan: ===
       <br> - Tidak sama dengan: !==
       ```
       1 < 2 // output : True
       1 > 2; // output : False
       "Apple" === "Jeruk" // output : False
       "Apple" !== "Jeruk" // output : True
       ```
     - Logical Operator
       <br>Digunakan untuk sebuah conditional. Akan menghasilkan nilai Boolean (true/false)
       <br> - AND operator : &&
       ```
       console.log(true && true) // output : true
       console.log(true && false) // output : false
       console.log(false && false) // output : false
       ```
     - OR operator: ||
       ```
       console.log(true || true) // output : true
       console.log(true || false) // output : true
       console.log(false || false) // output : false
       ```
     - NOT operator: !
       ```
       let tahu = true;
       console.log(!tahu) // output : false
       ```

- **Conditional**.
  <br> Conditional digunakan saat dibutuhkan percabangan kasus. Komputer akan melakukan suatu tindakan jika suatu kondisi terpenuhi

  - If statement
    <br> contoh :
    ```
    let haus = true;
     if (haus){
          console.log("minum")
     }
     // output : prints "minum"
    ```
  - If ... Else Statement
    <br> contoh :
    ```
    let haus = true;
     if (haus){
          console.log("minum")
     } else {
        console.log("gak minum")
     }
    ```
  - If ... Else if Statement
    <br> contoh :
    ```
    let keadaan = "haus";
     if (keadaan == "haus"){
          console.log("minum dulu")
     } else if (keadaan == "laper"){
          console.log("makan dulu")
     } else {
          console.log("tidur aja")
     }
    ```
  - Truthy and Falsy : digunakan untuk mengecek apakah variabel telah terisi namun tidak mementingkan nilainya
  - Switch Case Conditional
    <br> Gunakan Switch case jika kondisi dan percabangan terlalu banyak
    ```
     let hitung = 2;
     switch (hitung){
        case 1 : console.log("hitungan ke - "+ hitung)
        break;
        case 2 : console.log("hitungan ke - "+ hitung)
        break;
        case 3 : console.log("hitungan ke - "+ hitung)
        break;
        case 4 : console.log("hitungan ke - "+ hitung)
        break;
        case 5 : console.log("hitungan ke - "+ hitung)
        break;
        default : console.log("dah gaada apa2")
     } // output : hitungan ke - 2
    ```
  - Ternary Operator : short-syntax dari statement if … else
    <br> contoh :
    ```
     let hujan = true;
     hujan ? console.log("Bawa Payung") : console.log("panas cuy");
     // output : prints "bawa payung"
    ```

- **Looping**.
  <br> Komputer dapat melakukan sebuah proses yang sama berulang-ulang. Jika membutuhkan perulangan dalam kasus tertentu, kita bisa menggunakan Looping.
  - **Manual Looping**
    ```
    console.log(1)
    console.log(2)
    console.log(3)
     }
     //output :
     // 1
     // 2
     // 3
    ```
  - **for loop**
    <br> Gunakan FOR LOOP jika kita tahu seberapa banyak nilai pasti untuk pengulangannya. For loop akan terus berjalan selama kondisi ini terpenuhi. Selama kondisi bernilai TRUE
    <br>contoh :
    ```
     let a = 1;
     for (a; a <= 3; a++){
          console.log(a)
     }
     //output :
     // 1
     // 2
     // 3
    ```
  - **While loop**
    <br> Gunakan WHILE LOOP jika kita tidak mengetahui jumlah pasti pengulangan. WHILE LOOP akan menjalankan instruksi pengulangan kondisi bernilai TRUE
    <br> contoh :
    ```
     let warga = 2;
     let i;
     while (i <= jumlah warga){
          console.log("tampilkan data warga ke - " + warga)
          i++;
     }
    ```
  - **Do while**
    <br>Statement akan dikerjakan terlebih dahulu baru pengecekan kondisi
    ```
    let makanan = 5;
    do {
         console.log("makan dulu, masih ada makanan")
         makanan--;
    } while (makanan = 0){
         console.log("makanan sudah habis, kamu sih makan mulu")
    }
    ```
  - **Nested Loop**
    <br> Jika kita membuat looping didalam looping. Maka ini dinamakan Nested Loop. Looping pertama dianalogikan sebagai baris. Looping kedua dianalogikan sebagai kolom
    ```
     for (let i = 0; i <= 10; i++){
          for (let j = 1; j <= i; j++){
                console.log("baris" + i)
                console.log("kolom" + j)
          }
     }
    ```
