---
description: >-
  Konvensi adalah tentang aturan penulisan pada buku ini supaya pembaca memahami
  maksud dari contoh-contoh yang diberikan oleh penulis, sehingga pembaca dapat
  membaca buku ini dengan pemahaman yang baik
---

# Konvensi Penulisan

Pada buku ini akan sering bertemu dengan _code block_ atau sebuah blok kode yang dalam buku ini mempunyai 2 jenis code block.

* Sebagai perintah Terminal
* Sebagai potongan kode Ruby

### Perintah Terminal

{% code-tabs %}
{% code-tabs-item title="Terminal" %}
```bash
$ cd belajar # tanda $(dollar sign) tidak perlu dituliskan
$ touch hello.rb
$ exit
```
{% endcode-tabs-item %}
{% endcode-tabs %}

Pada _code block_ berjudul `Terminal` maksud penulis bahwa perintah didalam _code block_ diatas harus dieksekusi didalam terminal.

Tanda `$` \(dollar sign\) tidak perlu dituliskan, itu hanya sebagai tanda bahwa  berada pada lingkungan terminal, **** _line number_ disisi kiri pada code block berguna untuk penunjuk baris perintah.

Contoh penunjuk baris :  
Baris `2` adalah perintah untuk membuat sebuah file `hello.rb` .

### Kode Ruby

{% code-tabs %}
{% code-tabs-item title="main.rb" %}
```ruby
require_relative 'user.rb'

usr = User.new('Harpi', 'piharpi', 'justharpi@gmail', 'secret')
```
{% endcode-tabs-item %}

{% code-tabs-item title="user.rb" %}
```ruby
# User class didalam file user.rb
class User
  attr_accessor :name, :username, :email
  attr_writer :password

  def initialize(name, username, email, password)
    @name = name
    @email = email
    @username = username
    @password = password
  end
  
  def info
    "Halo nama saya #{name}, hubungi saya di #{email}"
  end
end
```
{% endcode-tabs-item %}
{% endcode-tabs %}

Code Block diatas terdapat `main.rb` \(bewarna merah tab aktif\) dan `user.rb` kedua file tersebut berkaitan, terkadang saya hanya menyematkan satu file saja, pada kasus ini saya menyematkan dua file untuk memberikan contoh.

Pada code block tersebut berisi kode ruby dari file `main.rb` karena sedang aktif coba klik bagian `user.rb` maka isi code block juga akan berubah, dan sisi kiri code block terdapat line number yang mempermudah untuk menunjuk kode ruby yang ingin penulis jelaskan.

Contoh penunjuk baris :  
Baris `13` pada file `user.rb` adalah sebuah method `info` yang berfungsi untuk mengembalikan informasi dari `Class User`.    

{% hint style="info" %}
Meskipun code block menyediakan fitur copy secara otomatis, saya sarankan tidak menggunakan itu, saya harap kamu mengerti alasanya, disini kamu tujuanya belajar pemprograman ruby **bukan** salin dan tempel.
{% endhint %}

  
 



