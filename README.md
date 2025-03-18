# Phase-1-Week-1

# JavaScript Week 1: Node.js Basic

## 1. Pengenalan Node.js

### Penjelasan
Node.js adalah runtime JavaScript yang berjalan di luar browser, menggunakan mesin V8 milik Google Chrome. Node.js memungkinkan kita untuk menjalankan JavaScript di sisi server dan membangun aplikasi berbasis jaringan, seperti web server dan API.

### Fitur Utama Node.js
- Asynchronous dan event-driven
- Non-blocking I/O
- Berbasis modul dengan npm (Node Package Manager)
- Dapat digunakan untuk membangun berbagai jenis aplikasi, termasuk API, server web, dan aplikasi real-time

### Instalasi Node.js
1. Unduh dan instal Node.js dari [nodejs.org](https://nodejs.org/)
2. Cek versi Node.js dan npm setelah instalasi:
   ```sh
   node -v  # Mengecek versi Node.js
   npm -v   # Mengecek versi npm
   ```

---

## 2. Contoh Penggunaan

### Menjalankan JavaScript dengan Node.js
Setelah Node.js terinstal, kita bisa menjalankan kode JavaScript menggunakan terminal.

#### Contoh: Menampilkan "Hello, Node.js!"
Buat file `app.js` dan tambahkan kode berikut:
```javascript
console.log("Hello, Node.js!");
```
Lalu jalankan perintah di terminal:
```sh
node app.js
```
Output:
```
Hello, Node.js!
```

### Membuat Server Sederhana dengan Node.js
Node.js dapat digunakan untuk membuat server HTTP dengan modul bawaan `http`.

```javascript
const http = require("http");

const server = http.createServer((req, res) => {
    res.writeHead(200, { "Content-Type": "text/plain" });
    res.end("Hello, World!");
});

server.listen(3000, () => {
    console.log("Server berjalan di http://localhost:3000");
});
```
Jalankan dengan:
```sh
node server.js
```
Kemudian buka browser dan akses `http://localhost:3000`.

---

## 3. Assignment

### Tugas 1: Menjalankan Script dengan Node.js
1. Buat file `hello.js`.
2. Tulis kode JavaScript yang mencetak `Hello, Node.js!` ke terminal.
3. Jalankan file tersebut menggunakan Node.js.

### Tugas 2: Membuat Server HTTP Sederhana
1. Buat file `server.js`.
2. Buat server yang merespons dengan teks `Welcome to My Node.js Server` saat diakses.
3. Jalankan server dan akses melalui browser di `http://localhost:3000`.

Selamat belajar Node.js! 🚀

