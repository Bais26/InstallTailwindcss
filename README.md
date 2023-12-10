# InstallTailwindcss
A simple HTML Tailwind Starter

Ini adalah panduan langkah demi langkah untuk menginstal dan menggunakan Tailwind CSS dalam proyek HTML. Proyek ini memiliki tujuan untuk membantu pemula memahami cara menggunakan Tailwind CSS dengan mudah.

## Instalasi

1. **Buat Proyek Baru**: Buatlah folder proyek baru dan buka terminal di dalamnya.
    ```bash
    mkdir ChallengePlugin
    cd ChallengePlugin
    ```
2. **Masuk VSCode**: Jalankan perintah untuk masuk VSCode di proyek Anda.
    ```bash
    code .
    ```
2. **Inisialisasi Node.js**: Jalankan perintah untuk menginisialisasi proyek Node.js.
    ```bash
    npm init -y
    ```
   ## Tampilan setelah di init
   
  > {
> 
  >"name": "challengeplugin",

  >"version": "1.0.0",

  >"description": "",
>
  >"main": "index.js",
>
  >"scripts": {
>
  >  "test": "echo \"Error: no test specified\" && exit 1"
>
  >},
>
  >"keywords": [],
>
  >"author": "",
>
  >"license": "ISC"
>
>}


4. **Instalasi Tailwind CSS**: Install Tailwind CSS dan paket terkait.
    ```bash
    npm install -D tailwindcss
    ```

5. **Konfigurasi Tailwind**: Buat file konfigurasi Tailwind.
    ```bash
    npx tailwindcss init
   ```
    Add the paths to all of your template files in your
   ```
   /** @type {import('tailwindcss').Config} */
   module.exports = {
     content: ["index.html"],
     theme: {
      extend: {},
     },
     plugins: [],
   }
    ```


7. **Buat File CSS dan HTML**: Buat file HTML (`index.html`) dan Folder (`src`) dengan file CSS (`input.css`) dalam proyek Anda.

8. **Edit File CSS**: Tambahkan referensi Tailwind CSS di dalam file input.css Anda.
    ```css
    @import 'tailwindcss/base';
    @import 'tailwindcss/components';
    @import 'tailwindcss/utilities';
    ```
9. **Start the Tailwind CLI build process :**
    Run the CLI tool to scan your template files for classes and build your CSS.
    ```bash
    npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch
    ```
    Bakalan Muncul Folder Dist

11. **Gunakan CSS dalam HTML**: Dalam file HTML (`index.html`), tambahkan referensi ke file CSS Anda.
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
      <meta charset="UTF-8">
      <title>Proyek Tailwind CSS</title>
      <link href="/dist/output.css" rel="stylesheet">
    </head>
    <body>
      <h1 class="text-3xl font-bold underline text-violet-800">
      Hello world!
      </h1>
    </body>
    </html>
    ```

## Menjalankan Proyek

Buka proyek Anda di browser untuk melihat Tailwind CSS berfungsi. Anda bisa menggunakan Live Server atau membuka file HTML di browser.

## PLUGIN
## by M Bais Yufan Mardiansah
