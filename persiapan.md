---
description: >-
  Sebelum kita mempelajari ruby kita persiapkan alat-alat yang dibutuhkan, anda
  bisa melewatkan bab ini jika memang anda benar yakin sudah memiliki alat yang
  dibutuhkan untuk mempelajari ruby.
---

# Persiapan

## Text Editor

Anda bisa menggunakan text editor kesayangan anda, namun jika anda tidak memiliki opsi saya merekomendasikan beberapa text editor yaitu [sublime](https://www.sublimetext.com/), [vscode](https://code.visualstudio.com/), [atom](https://atom.io/), [rubymine](https://www.jetbrains.com/ruby/) atau [VIM](https://www.vim.org/), semua text editor yang tersebut tersedia disemua sistem operasi\(Linux, Windows, MacOS\) tapi saya menyarankan menggunakan **vscode** jika anda bingung.

## Terminal

Ada beberapa jenis software terminal, yaitu [Tmux](https://github.com/tmux/tmux/wiki), [Bash](https://www.gnu.org/software/bash/), [Git Bash](https://git-scm.com/downloads), [Cmder](http://cmder.net/), [Hyper](https://hyper.is/), [XTerm](https://invisible-island.net/xterm/), dan sebagainya, gunakan terminal kesukaan anda, atau jika anda menggunakan sistem operasi Windows saya sarankan untuk menggunakan Git Bash atau Cmder.

## Ruby

Versi ruby yang digunakan pada buku ini adalah `ruby 2.5.2` jika anda mempunyai cara tersendiri untuk melakukan instalasi ruby, anda dapat mengikuti cara anda sendiri. Namun, jika tidak anda juga dapat mengikuti cara instalasi berikut ini sesuai dengan sistem operasi yang anda gunakan. 

{% tabs %}
{% tab title="Linux" %}
#### Instalasi pada Ubuntu

Pertama, instal dahulu dependency yang dibutuhkan

```text
sudo apt-get update
sudo apt-get install git-core curl zlib1g-dev build-essential libssl-dev libreadline-dev libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt1-dev libcurl4-openssl-dev python-software-properties libffi-dev nodejs
```

Kemudian kita akan menggunakan rbenv untuk menginstal ruby. rbenv ini tools yang dibuat khusus untuk menginstal ruby dan manajemen versi ruby di komputer kita. Dengan rbenv ini kita bisa memiliki lebih dari satu versi yang terinstall.

Langkah pertama adalah install rbenv itu sendiri. Jalankan perintah berikut

```text
cd
git clone https://github.com/rbenv/rbenv.git ~/.rbenv
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
echo 'eval "$(rbenv init -)"' >> ~/.bashrc
exec $SHELL
```

Selanjutnya install ruby-build. rbenv membutuhkan ruby-build ini untuk melakukan build terhadap source ruby sehingga kita tinggal enak aja menginstallnya. Jalankan perintah di bawah untuk menginstalnya.

```text
git clone https://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build
echo 'export PATH="$HOME/.rbenv/plugins/ruby-build/bin:$PATH"' >> ~/.bashrc
exec $SHELL
```

Nah sekarang baru kita instal rubynya. Kita gunakan versi yang terbaru yaitu 2.5.2.   
Caranya seperti ini

```text
rbenv install 2.5.2
rbenv global 2.5.2
ruby -v
```

Saat menjalankan perintah ruby -v maka di terminal harusnya muncul informasi yang menandakan kalau ruby yang terinstal adalah versi 2.5.2

Oke, instalasi ruby di Linux selesai dan anda bisa melanjutkan kebab selanjutnya
{% endtab %}

{% tab title="MacOs" %}
Install ruby di Mac kita juga akan menggunakan rbenv. Tetapi sebelumnya kita perlu menginstal brew buat instal rbenv, hee mbulet-mbulet yak. Jalankan perintah berikut buat install brew kalau brew belum diinstal di komputer mac mu.

```text
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Nah begitu sudah ada brew, tinggal instal deh rbenv dan ruby-build pakai perintah di bawah ini.

```text
brew install rbenv ruby-build
echo 'if which rbenv > /dev/null; then eval "$(rbenv init -)"; fi' >> ~/.bash_profile
source ~/.bash_profile
```

Langkah terakhir instal deh ruby-nya. Kita gunakan versi terbaru yang stabil, 2.5.2

```text
rbenv install 2.5.2
rbenv global 2.5.2
ruby -v
```

Pastikan ketika menjalan ruby -v maka di terminal muncul info yang isinya kalau versi ruby yang terinstal adalah 2.5.2
{% endtab %}

{% tab title="Windows" %}

{% endtab %}
{% endtabs %}

