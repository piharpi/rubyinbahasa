# Method p

Cara lain yang juga digunakan untuk mengoutputkan pada layar adalah dengan menggunakan method `p`, fungsi dari method `p` ini untuk mengoutputkan secara literal dari suatu object, keuntungang menggunakan method ni kita bisa mengetahui informasi apa sebenarnya dari suatu object. 

Lihat blok kode berikut ini kita akn membandingkan dengan method `puts`. 

{% tabs %}
{% tab title="p\_and\_puts.rb" %}
```ruby
puts "Ruby is Dynamic Programming Language"
p "Ruby is Dynamic Programming Language"
```
{% endtab %}

{% tab title="Result" %}
```
Ruby is Dynamic Programming Language
"Ruby is Dynamic Programming Language"
```
{% endtab %}
{% endtabs %}

Lihat dari hasil diatas `puts` menghasilkan output tanpa tanda petik, sedangkan `p` disertai dengan tanda petik, itu menginforamasikan bahwa nilai yang diinputkan oleh `p` bertipe adalah [String](../strings.md).

Contoh lain 

{% tabs %}
{% tab title="Ruby" %}
```ruby
puts [1, 2, nil, nil, 5] 
p [1, 2, nil, nil, 5]
```
{% endtab %}

{% tab title="Output" %}
```bash
1
2


5
[1, 2, nil, nil, 5]
```
{% endtab %}
{% endtabs %}

puts memanggil sebuah fungsi to\_is sedangkan p referenced terhadap fungsi inspect

