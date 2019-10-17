# Strings

**String** adalah sekumpulan dari sebuah karakter, penulisan string ini dengan cara menggunakan tanda petik\("..."\) ****dan bisa juga menggunakan _****_tanda petik tunggal\('...'\).

{% code-tabs %}
{% code-tabs-item title="ex\_strings.rb" %}
```ruby
# Tanda petik
puts "Semangat belajar ruby!!"

# Tanda petik tunggal
puts 'Semangat belajar ruby!!'
```
{% endcode-tabs-item %}
{% endcode-tabs %}

Kedua cara baik tanda petik maupun tanda petik tunggal akan dapat dipahami oleh Ruby, namun kedua cara tersebut mempunyai tujuan penggunaan yang berbeda, sebagai contoh berikut ini.

{% code-tabs %}
{% code-tabs-item title="create\_strings.rb" %}
```ruby
# Jika dalam kasus kita ingin menggunakan tanda petik tunggal
# didalam tanda petik, maka kita menggunakan tanda petik.
puts "ditimbali 'dipanggil dalam bahasa jawa'"

# Namun saat kita ingin menggunakan tanda petik, kita bisa
# menggunakan tanda petik tunggal sebagai pengahapitnya. 
puts '"Merdeka atau mati!" seru Bung Tomo dalam pidatonya.'
```
{% endcode-tabs-item %}
{% endcode-tabs %}

Bisakah semisalnya saya ingin menggunakan tanda petik tunggal untuk menghapit tanda petik tunggal juga ?, Bisa

{% code-tabs %}
{% code-tabs-item title="escape\_charcter.rb" %}
```ruby
# Tanda petik didalam tanda petik.
puts "\"Merdeka atau Mati!\", seru Bung Tomo dalam pidatonya."

# Tanda petik tunggal didalam tanda petik tunggal.
puts 'ditimbali \'dipanggil dalam bahasa jawa\''
```
{% endcode-tabs-item %}
{% endcode-tabs %}

Dengan menggunakan Escape Character\(`\`\), Ruby menganggap suatu karakter yang tidak diinterpretasi, sehingga dapat dieksekusi dengan baik.

