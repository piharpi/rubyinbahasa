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

Diatas adalah contoh dimana kita mencetak pada layar tentang 

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
{% code title="" %}
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

contoh kedua adalah merupakan 

