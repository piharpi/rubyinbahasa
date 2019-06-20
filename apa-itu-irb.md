# Apa itu irb ?

Interactive Ruby Shell juga biasa dipanggil irb terinstall otomatis dari ruby, fungsinya sebagai area menjalankan kode ruby tanpa harus menyimpan kedalam sebuah file atau biasa dikenal dengan sandbox / playground, sehingga kita dapat langsung menjalankan kode ruby yang kita tullis, biasanya irb ini dimanfaatkan untuk eksperiment atau hanya mencoba beberapa baris kode ruby saja.

## Cara menjalankan irb

Jalankan irb melalui terminal anda dengan cara mengetikan `irb` , jika tidak bisa kemungkinan ruby tidak terinstall, silahkan kembali kemateri tentang [penginstallan Ruby](https://ruby-in-bahasa.gitbook.io/project/-LW_W43pTyw3DPRHPPDP/~/drafts/-LWqQpXBONd7AHjh8UDX/primary/persiapan#ruby) jika belum menginstall.

```bash
irb(main):001:0> 
```

Diatas adalah tampilan ketika irb terbuka, selanjutnya kita menuliskan kode Ruby pada irb, seperti belajar bahasa pemprograman pada umumnya kita menuliskan ritual `"Hello World"` dengan bahasa Ruby.

```bash
irb(main):001:0> puts "Hello World"
```

Jika kita tekan tombol **ENTER** pada keyboard maka kode tersebut akan dieksekusi oleh irb dan menghasilkan seperti dibawah ini.

```bash
irb(main):001:0> puts "Hello World"
Hello World
=> nil
irb(main):002:0> 
```

Sekarang kode ruby sudah dieksekusi dan menghasilkan output `Hello World` dan return value `nil`, Jangan bingung terlebih dahulu dengan hasil eksekusi kode tersebut karena disini lingkup penjelasanya adalah cara menjalankan irb,  hasil eksekusi kode tersebut akan dibahas di materi selanjutnya.

## Cara keluar dari irb

Untuk keluar dari irb anda bisa mengetikan `exit` atau `quit`, maka dengan salah satu itu kita kembali tampilan terminal semula.

```bash
# ketikkan exit atau quit untuk keluar dari irb
irb(main):002:0> exit
```

Itulah penjelasan tentang irb, semoga tidak ada kesulitan dalam memahami irb.

