# Tugas Mandiri 5

**Nama:** MOHAMMAD RIZKI HOIRUR ROFI
**NIM:** 2024520037

---

## 1. Apa perbedaan SQL mentah dan ORM?

SQL mentah adalah cara mengakses database dengan menulis perintah SQL secara langsung, seperti `SELECT`, `INSERT`, `UPDATE`, dan `DELETE`.

Sedangkan ORM (Object-Relational Mapping) memungkinkan programmer mengakses database menggunakan objek, fungsi, atau metode dari bahasa pemrograman tanpa harus menulis SQL secara langsung untuk setiap operasi.

## 2. Apa kelebihan SQL mentah?

Kelebihan SQL mentah adalah programmer memiliki kontrol yang lebih besar terhadap query database. SQL juga cocok digunakan untuk query yang kompleks dan membutuhkan optimasi khusus.

## 3. Apa kelebihan ORM?

ORM membuat proses mengakses database menjadi lebih sederhana dan terstruktur. Programmer dapat menggunakan fungsi atau metode seperti `findUnique()`, `findMany()`, `create()`, `update()`, dan `delete()` tanpa menulis query SQL secara langsung.

## 4. Apa risiko SQL Injection?

SQL Injection adalah serangan ketika input dari pengguna dimasukkan ke dalam query SQL secara tidak aman sehingga penyerang dapat memanipulasi query database.

Contoh query yang tidak aman:

```js
const query = "SELECT * FROM jadwal WHERE id = " + id;
```

Jika input pengguna tidak divalidasi atau diparameterisasi dengan benar, query dapat dimanipulasi.

## 5. Mengapa penggunaan parameter query dapat mengurangi risiko SQL Injection?

Parameter query memisahkan perintah SQL dengan data yang diberikan oleh pengguna.

Contohnya:

```js
const [rows] = await db.execute(
  'SELECT * FROM jadwal WHERE id = ?',
  [id]
);
```

Tanda `?` digunakan sebagai placeholder. Nilai `id` dikirim sebagai parameter sehingga tidak dianggap sebagai bagian dari perintah SQL.

Dengan demikian, penggunaan parameterized query dapat membantu mencegah input pengguna menjadi bagian dari sintaks SQL.

## 6. Bagaimana ORM membantu programmer dalam mengakses database?

ORM menyediakan abstraksi untuk berinteraksi dengan database. Programmer dapat menggunakan metode yang lebih sederhana untuk mengambil, menambahkan, mengubah, atau menghapus data.

Contohnya dengan Prisma:

```js
const jadwal = await prisma.jadwal.findUnique({
  where: {
    id: 1
  }
});
```

Programmer cukup menggunakan metode `findUnique()` untuk mencari data berdasarkan ID tanpa harus menulis query `SELECT` secara langsung.
