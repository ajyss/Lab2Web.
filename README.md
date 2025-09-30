Oke, saya bantu poles README Anda agar lebih menarik, rapi, dan tetap SEO-friendly dengan tambahan elemen visual (emoji, heading lebih hidup, dan sedikit copywriting supaya tidak kaku). Berikut hasil revisinya:

---

# 🌐 Praktikum 1 – HTML Dasar

👤 **Nama**: Muhammad Aziz Tri Ramadhan
🆔 **NIM**: 312410380
🏫 **Kelas**: TI.24.A3

---

## 📂 File yang Digunakan

* 📄 **lab.html** → berisi struktur HTML utama serta deklarasi **internal CSS**.
* 🎨 **style_eksternal.css** → file CSS eksternal yang dipanggil dari `lab.html`.

---

## 🚀 Jawaban Tugas

### 🔹 1. Eksperimen Mengubah Properti CSS

Pada file `lab.html` terdapat deklarasi awal untuk elemen `<h1>`:

```css
h1 {
  font-size: 24px;
  color: #0F189F;
  text-align: center;
  padding: 20px 10px;
}
```

📸 Tampilan awal: <img src="img4.png" width="700">

Kemudian saya lakukan eksperimen dengan menambahkan properti baru:

```css
h1 {
  font-size: 28px;
  color: darkblue;
  text-align: center;
  padding: 20px 10px;
  background-color: lightgray;
  border-radius: 10px;
}
```

📸 Hasil setelah perubahan: <img src="img6.png" width="700">

✨ **Perubahan yang terlihat:**

* Ukuran teks lebih besar.
* Warna menjadi biru tua.
* Ada latar belakang abu-abu dengan sudut melengkung.

---

### 🔹 2. Perbedaan `h1 {…}` dengan `#intro h1 {…}`

* `h1 {…}` → berlaku untuk **semua elemen `<h1>`**.
* `#intro h1 {…}` → hanya berlaku pada `<h1>` di dalam elemen dengan **id="intro"**.

📌 Contoh dari `lab.html`:

```html
<header>
  <h1>CSS Internal dan <i>Inline CSS</i></h1>
</header>

<div id="intro">
  <h1>Hello World</h1>
</div>
```

Jika ditambahkan CSS berikut:

```css
h1 {
  color: red;
}

#intro h1 {
  color: green;
}
```

📸 Hasil: <img src="image copy 5.png" width="700">

👉 **Kesimpulan:**

* Judul di `<header>` → **merah**.
* Judul di dalam `#intro` → **hijau**.

---

### 🔹 3. Prioritas CSS (Eksternal, Internal, Inline)

Urutan prioritas CSS:

1. **Inline CSS** (paling kuat 💪).
2. **Internal CSS** (didefinisikan dalam `<style>`).
3. **Eksternal CSS** (paling lemah jika konflik).

📌 Contoh:

```html
<p style="color: blue;">Teks ini Inline CSS</p>
```

```css
/* Internal */
p { color: green; }

/* Eksternal */
p { color: red; }
```

👉 Hasil: Teks tetap **biru**, karena inline CSS lebih dominan.

---

### 🔹 4. Prioritas ID vs Class

Jika elemen memiliki **ID** dan **Class**, maka **ID lebih kuat**.

📌 Contoh dari `lab.html`:

```html
<p id="paragraf-1" class="text-paragraf">
  Ini contoh teks dengan ID dan Class
</p>
```

```css
.text-paragraf {
  color: blue;
}

#paragraf-1 {
  color: red;
}
```

👉 Hasil: Teks berwarna **merah**, karena ID selector lebih spesifik dibanding Class.

---

## 📝 Kesimpulan

📌 Dari praktikum ini dapat disimpulkan bahwa:

1. CSS bisa diperkaya dengan berbagai properti untuk memperindah tampilan web.
2. Selector umum (`h1`) berbeda dengan selector spesifik (`#intro h1`).
3. Urutan prioritas CSS adalah: **Inline > Internal > Eksternal**.
4. ID memiliki tingkat prioritas lebih tinggi dibandingkan Class.

---

## Langkah Langkah Praktikum

### 1. tampilan Browser

📸 Hasil:

<img src="image.png" width="700">

### 2. Membuat dokumen HTML
📸 Hasil:

<img src="image copy 2.png" width="700">
