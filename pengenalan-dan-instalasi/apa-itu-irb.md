---
description: 'Mengenal apa itu irb, cara menggunakan irb dan mengetahui hal-hal didalam irb.'
---

# Apa itu irb?

Interactive Ruby Shell juga biasa dipanggil irb terinstall otomatis pada saat kita menginstall ruby, fungsinya sebagai area menjalankan kode ruby tanpa harus menyimpan kedalam sebuah file atau biasa dikenal dengan sandbox / playground, sehingga kita dapat langsung menjalankan kode ruby yang kita tullis, biasanya irb ini dimanfaatkan untuk eksperiment atau hanya mencoba beberapa baris kode ruby saja.

## Cara menjalankan irb

Jalankan irb melalui terminal kamu dengan cara mengetikan `irb` , jika tidak bisa kemungkinan ruby tidak terinstall, silahkan kembali kepembahasan tentang [installasi Ruby](https://ruby-in-bahasa.gitbook.io/project/-LW_W43pTyw3DPRHPPDP/~/drafts/-LWqQpXBONd7AHjh8UDX/primary/persiapan#ruby) jika belum menginstall.

{% code-tabs %}
{% code-tabs-item title="Terminal" %}
```bash
$ irb
irb(main):001:0> 
```
{% endcode-tabs-item %}
{% endcode-tabs %}

Diatas adalah tampilan ketika irb terbuka, selanjutnya kita menuliskan kode Ruby pada irb, seperti belajar bahasa pemprograman pada umumnya kita menuliskan ritual `"Hello World"`.

{% code-tabs %}
{% code-tabs-item title="Terminal" %}
```bash
irb(main):001:0> puts "Hello World"
```
{% endcode-tabs-item %}
{% endcode-tabs %}

Jika kita tekan tombol **`ENTER`** pada keyboard maka kode tersebut akan dieksekusi oleh irb dan menghasilkan seperti dibawah ini.

{% code-tabs %}
{% code-tabs-item title="Terminal" %}
```bash
irb(main):001:0> puts "Hello World"
Hello World
=> nil
irb(main):002:0> 
```
{% endcode-tabs-item %}
{% endcode-tabs %}

Sekarang kode ruby sudah dieksekusi dan menghasilkan output `Hello World` dan return value `nil`, jangan bingung akan kita bahas sekarang,  `puts` adalah kependekan dari "put string" adalah perintah untuk menampilkan sesuatu dilayar.

Jika kita amati pada hasil eksekusi diatas terdapat `Hello World` yang dimana sebagai hasil output, dan tanda `=>`  ini  adalah tanda _return value_ yang bernilai `nil` ,  pada ruby hasil output dan nilai kembalian berbeda, pada contoh ini puts adalah sebuah perintah yang output yang menjadi string dan mengembalikan nilai hampa atau `nil`. 

Contoh lain,

{% code-tabs %}
{% code-tabs-item title="Terminal" %}
```bash
irb(main):004:0> 20 + 15
=> 35
```
{% endcode-tabs-item %}
{% endcode-tabs %}

Diatas adalah perintah penjumlahan pada ruby, sederhana saja diatas __mengembalikan nilai / _return value_ `35` tapi tidak memberikan output.

Semoga sampai sini bisa dipahami.

## Cara keluar dari irb

Untuk keluar dari irb kamu bisa mengetikan `exit` atau `quit`, maka dengan salah satu itu kita kembali tampilan terminal semula.

{% code-tabs %}
{% code-tabs-item title="Terminal" %}
```bash
# ketikkan exit atau quit untuk keluar dari irb
irb(main):002:0> exit
```
{% endcode-tabs-item %}
{% endcode-tabs %}

Itulah penjelasan tentang irb, semoga tidak ada kesulitan dalam memahami irb. 

