# Method print

Hampir sama seperti puts method tak lain tak bukan print ini merupakan method yang digunakan untuk mengevaluasi dan menampilkan pada layar console/terminal, **namun** `print` **memiliki perbedaan** yaitu tidak membuat baris baru pada saat mencetak pada layar, perhatikan kode berikut ini.

{% tabs %}
{% tab title="contoh\_print\_string.rb" %}
{% code title="contoh\_print\_string.rb" %}
```ruby
print "Tolong!"
print "Tolong!" 
print "Tolong!"
```
{% endcode %}
{% endtab %}

{% tab title="contoh\_puts\_string.rb" %}
{% code title="contoh\_puts\_string.rb" %}
```ruby
puts "Tolong!"
puts "Tolong!"
puts "Tolong!"
```
{% endcode %}
{% endtab %}

{% tab title="Result print" %}
{% code title="Terminal" %}
```bash
$ ruby contoh_print_string.rb
Tolong!Tolong!Tolong!
```
{% endcode %}
{% endtab %}

{% tab title="Result puts" %}
{% code title="Terminal" %}
```bash
$ ruby contoh_puts_string.rb
Tolong!
Tolong!
Tolong!
```
{% endcode %}
{% endtab %}
{% endtabs %}

Bisa di lihat perbedaanya diatas antara tab **Result print** dan **Results puts**, pada print terlihat bahwa menghasilkan satu baris dan pada puts menghasilkan baris baru.

Keduanya memiki fungsi yang sama yaitu mengoutputkan, namun secara penggaunaan tergantung pada kebutuhan kita, apakah kita membutuhkan baris baru atau tidak.

**Contoh lain.**

{% tabs %}
{% tab title="contoh\_print\_string.rb" %}
{% code title="contoh\_print\_string.rb" %}
```ruby
print "Selamat datang di Ind***ret"
print ", "
print "Selamat berbelanja"
```
{% endcode %}
{% endtab %}

{% tab title="contoh\_puts\_string.rb" %}
{% code title="contoh\_puts\_string.rb" %}
```ruby
puts "Selamat datang di Ind***ret,"
puts ", "
puts "Selamat berbelanja"
```
{% endcode %}
{% endtab %}

{% tab title="Result print" %}
{% code title="Terminal" %}
```bash
$ ruby contoh_print_string.rb
Selamat datang di Ind***ret, Selamat berbelanja
```
{% endcode %}
{% endtab %}

{% tab title="Result puts" %}
{% code title="Terminal" %}
```bash
$ ruby contoh_puts_string.rb
Selamat datang di Ind***ret
,
Selamat berbelanja
```
{% endcode %}
{% endtab %}
{% endtabs %}

Kamu juga dapat menggunakan _escape sequences_ `\n` untuk membuat baris baru pada method `print` .

{% tabs %}
{% tab title="contoh\_print\_newline.rb" %}
{% code title="contoh\_print\_newline.rb" %}
```ruby
print "saya juga bisa membuat baris baru\n"
print "yah aku dibawah"
```
{% endcode %}
{% endtab %}

{% tab title="Result" %}
{% code title="Terminal" %}
```bash
$ ruby contoh_print_newline.rb
saya juga bisa membuat baris baru
yah aku dibawah
```
{% endcode %}
{% endtab %}
{% endtabs %}

Namun cara diatas tidak efektif dan tujuan `print` adalah mencetak pada console tanpa baris baru/newline.

