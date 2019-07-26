---
description: >-
  Konvensi adalah tentang aturan penulisan pada buku ini supaya pembaca memahami
  maksud dari contoh-contoh yang diberikan oleh penulis, sehingga pembaca dapat
  membaca buku ini dengan pemahaman yang baik
---

# Konvensi Penulisan

Pada buku ini akan sering bertemu dengan _code block_ atau sebuah blok kode yang dalam buku ini mempunyai 2 jenis code block 

* Sebagai perintah Terminal
* Sebagai potongan code bahasa Ruby

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

Pada _code block_ diatas ditandai dengan tulisan `Terminal` pada pojok kiri atas sehingga pembaca mengetahui maksud bahwa kode didalam _code block_ diatas harus dieksekusi didalam terminal.

Tanda `$` \(dollar sign\) tidak perlu dituliskan, itu hanya sebagai tanda bahwa  berada pada lingkungan terminal, **** _line number_ disisi kiri pada code block berguna untuk penunjuk baris perintah.

Contoh penunjuk baris :  
Baris `2` adalah perintah untuk membuat sebuah file `hello.rb` .

### Kode Ruby

{% code-tabs %}
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

usr = User.new('Harpi', 'piharpi', 'justharpi@gmail', 'secret')

```
{% endcode-tabs-item %}
{% endcode-tabs %}

_Code block_ diatas   
 



