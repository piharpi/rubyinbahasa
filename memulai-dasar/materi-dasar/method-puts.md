# Method puts

Method `puts` adalah kependekan dari put string yang berfungsi untuk mengevaluasi dan menampilkan/mencetak pada layar console/terminal yang sedang kita gunakan, silahkan eksekusi kode berikut.

{% tabs %}
{% tab title="contoh\_puts.rb" %}
{% code title="contoh\_puts.rb" %}
```ruby
puts "Halo Dunia!"
puts "Bagaimana kabarmu?"
```
{% endcode %}
{% endtab %}

{% tab title="Result" %}
{% code title="Terminal" %}
```bash
$ ruby contoh_puts.rb
Halo Dunia!
Bagaimana kabarmu?
=> nil
```
{% endcode %}
{% endtab %}
{% endtabs %}

Diatas adalah contoh dimana kita mencetak object String dimana string adalah sekumpulan sebuah karakter yang ditandai dengan tanda petik tunggal maupun ganda yang nanti kita akan [bahas](../strings.md) setelah menyelesaikan bab dasar ini.

`puts` dapat digunakan di object apa saja, tidak hanya digunakan pada object String saja, put string berarti mengubah suatu type object apapun menjadi string termasuk `nil` namun dia akan menghasilkan blank line saja.

Berikut contoh ketika mencetak object `nil`

{% tabs %}
{% tab title="contoh\_puts\_nil\_object.rb" %}
{% code title="contoh\_puts\_nil\_object.rb" %}
```ruby
puts nil
puts [1, 2, nil, nil, 5]
```
{% endcode %}
{% endtab %}

{% tab title="Result" %}
{% code title="Terminal" %}
```bash
$ ruby contoh_puts_nil_object.rb

1
2


5
=> nil
```
{% endcode %}
{% endtab %}
{% endtabs %}

Jangan kuwatir juga nanti kita akan membahas tentang [nil object](return-value-dan-nil-object.md) dan [Arrays](../arrays.md) collection, dibab ini saya hanya ingin menunjukan bagaimana mengoutputkan sebuah nilai dengna menggunakan method puts.

Next ya ? semoga dapat dipahami.

