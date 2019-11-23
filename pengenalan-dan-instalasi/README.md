---
description: Mengetahui bahasa sejarah singkat bahasa ruby dan karakteristiknya.
---

# Pengenalan Bahasa Ruby

Sebelum mempelajari pengkodean bahasa ruby alangkah baiknya kita mengenal dahulu sejarah bahasa Ruby dan karakteristik bahasa ini.

### Tentang Ruby

Ruby adalah Object Oriented Programming Language \(OOP\) diciptakan oleh [Yukihiro Matsumoto](https://en.wikipedia.org/wiki/Yukihiro_Matsumoto) atau yang lebih dikenal Matz,  awal mula penamaan bahasa ini, saat sesi percakapan daring antara Matz dengan Keiju Ishitsuka, sebelum bahasa ini ditulis, pada saat itu terdapat dua pilihan nama: "Coral" dan "Ruby", kemudian Matz memilih Ruby, alasan Matz memilih nama "Ruby" karena ruby merupakan _birthstone_ \(batu peramata yang menggambarkan kelahiran seseorang\) salah satu koleganya.

Ruby terpengaruh oleh Perl, Smalltalk, Eiffel, Ada, Basic, dan Lisp yang mana bahasa itu disukai oleh Matz, yang dibentuk bahasa baru.

Matz mengatakan “trying to make Ruby natural, not simple,”  yang berarti bahasa Ruby terlihat natural seperti bahasa manusia sintaxnya namun dalam prosesnya itu tidak sederhana. 

Matz juga mengatakan Ruby dirancang untuk meningkatkan produktifitas para programmer, menikmati saat menggunakan bahasa Ruby dan tentunya menyenangkan bagi si programmer, Dia menekankan bahwa desain sistem perlu menekankan kepada manusia, bukan komputer.

![](../.gitbook/assets/image%20%281%29.png)

Bisa dillihat pada header situs resmi bahasa Ruby [https://www.ruby-lang.org](https://www.ruby-lang.org), menyatakan 👨🏻💻 Ruby adalah sahabat programmer. 

### Everything in Ruby is an Object

Ini yang perlu diperhatikan bahwa pada Ruby setiap informasi dan kode adalah object, sehingga dapat diberikan properties dan actions, dalam OOP properties disebut _instance variables_, sedangkan actions disebut _methods,_ setiap object memiliki methods dan instance variables, diberikan contoh sebagai berikut**.**

{% code title="learn.rb" %}
```ruby
3.times { print "Saya belajar Ruby" }
```
{% endcode %}

Kamu tidak perlu bingung maksud kode diatas, tapi sepertinya kamu sudah tahu hasil kode tersebut, disini penulis hanya ingin menunjukan kode Ruby yang sederhana dan mudah untuk dituliskan.

Pada bahasa lain kebanyakan primitive types bukanlah sebuah object, namun pada Ruby _primitive types_ adalah object yang dapat memiliki methods dan instance variables pada contoh kode diatas, 3 adalah sebuah primitive types integer dan mempunyai method times.

{% code title="love.rb" %}
```ruby
"saya senang belajar ruby".length
```
{% endcode %}

Penamaan method yang digunakan Ruby natural sehingga mudah untuk diingat seperti pada method `.length` diatas, yang berarti perintah berapa panjang karakter string tersebut, perlu diperhatikan lagi `.length` adalah method yang terdapat pada object String tersebut. 

