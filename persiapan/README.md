---
description: >-
  Sebelum kita mempelajari ruby kita persiapkan alat-alat yang dibutuhkan, anda
  bisa melewatkan bab ini jika memang anda benar yakin sudah memiliki alat yang
  dibutuhkan untuk mempelajari ruby.
---

# Persiapan

## Text Editor

Anda bisa menggunakan text editor kesayangan anda, namun jika anda tidak memiliki opsi saya merekomendasikan beberapa text editor yaitu [sublime](https://www.sublimetext.com/), [vscode](https://code.visualstudio.com/), [atom](https://atom.io/), [rubymine](https://www.jetbrains.com/ruby/) atau [VIM](https://www.vim.org/), semua text editor yang tersebut tersedia disemua sistem operasi \(Linux, Windows, MacOS\) tapi saya menyarankan menggunakan **vscode** jika anda bingung.

## Terminal

Ada beberapa jenis software terminal, yaitu [Tmux](https://github.com/tmux/tmux/wiki), [Bash](https://www.gnu.org/software/bash/), [Git Bash](https://git-scm.com/downloads), [Cmder](http://cmder.net/), [Hyper](https://hyper.is/), [XTerm](https://invisible-island.net/xterm/), dan sebagainya, gunakan terminal kesukaan anda, atau jika anda menggunakan sistem operasi Windows saya sarankan untuk menggunakan Git Bash atau Cmder.

## Ruby

Versi ruby yang digunakan pada buku ini adalah `ruby 2.5.3` jika anda mempunyai cara tersendiri untuk melakukan instalasi ruby, anda dapat mengikuti cara anda sendiri. Namun, jika tidak anda juga dapat mengikuti cara instalasi berikut ini sesuai dengan sistem operasi yang anda gunakan. 

{% tabs %}
{% tab title="Ubuntu" %}
Pertama, install terlebih dahulu dependency, ini adalah bagian-bagian yang dibutuhkan untuk melanjutkan instalasi selanjutnnya.

```text
curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list

sudo apt-get update
sudo apt-get install git-core curl zlib1g-dev build-essential libssl-dev libreadline-dev libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt1-dev libcurl4-openssl-dev software-properties-common libffi-dev nodejs yarn
```

Selanjutnya, kita akan menggunakan [rbenv](https://github.com/rbenv/rbenv) untuk menginstall ruby. rbenv ini alat yang dibuat khusus untuk menginstall ruby dan manajemen versi ruby di komputer kita. Dengan adanya rbenv ini kita bisa memiliki lebih dari satu versi ruby yang terinstall.

Langkah pertama adalah instalasi rbenv itu sendiri. Jalankan perintah berikut ini.

```text
cd
git clone https://github.com/rbenv/rbenv.git ~/.rbenv
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
echo 'eval "$(rbenv init -)"' >> ~/.bashrc
exec $SHELL
```

Setelah itu, install ruby-build. rbenv membutuhkan ruby-build ini untuk melakukan build terhadap source ruby. Jalankan perintah di bawah untuk menginstallnya.

```text
git clone https://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build
echo 'export PATH="$HOME/.rbenv/plugins/ruby-build/bin:$PATH"' >> ~/.bashrc
exec $SHELL
```

Sekarang kita menginstall Ruby. Kita menggunakan versi 2.5.3, Caranya sebagai berikut

```text
rbenv install 2.5.3
rbenv global 2.5.3
ruby -v
```

Saat menjalankan perintah ruby -v maka diterminal pastikan menampilkan informasi yang menyatakan ruby yang terinstall adalah versi 2.5.3, jika informasi tersebut tampil berarti instalasi ruby berhasil dikomputer anda.

Oke, instalasi ruby di Ubuntu selesai dan anda bisa melanjutkan kebagian selanjutnya.
{% endtab %}

{% tab title="MacOs" %}
Di MacOs kita menggunakan [rbenv](https://github.com/rbenv/rbenv) sebagai alat yang dibuat khusus untuk menginstall ruby dan manajemen versi ruby di komputer kita, namun sebelum itu kita menginstall [Homebrew](https://brew.sh/), brew ini dibutuhkan untuk menginstall rbenv yang tidak tersedia di Apple.

```text
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Selanjutnya, jika instalasi brew selesai, install rbenv dan ruby-build menggunakan perintah di bawah ini.

```text
brew install rbenv ruby-build

# Menambahkan rbenv dibash dengan itu akan memuat setiap waktu anda membuka terminal
echo 'if which rbenv > /dev/null; then eval "$(rbenv init -)"; fi' >> ~/.bash_profile
source ~/.bash_profile
```

Langkah terakhir menginstall ruby. Kita menggunakan versi, 2.5.3

```text
# Install Ruby
rbenv install 2.5.3
rbenv global 2.5.3
ruby -v
```

Saat menjalankan perintah ruby -v maka diterminal pastikan menampilkan informasi yang menyatakan ruby yang terinstall adalah versi 2.5.3, jika informasi tersebut tampil berarti instalasi ruby berhasil dikomputer anda.

Oke, instalasi ruby di Ubuntu selesai dan anda bisa melanjutkan kebagian selanjutnya.
{% endtab %}

{% tab title="Windows" %}
Ada sebuah alat bantu yang membantu Anda memasang Ruby : [RubyInstaller](https://rubyinstaller.org/). Ini memberikan apapun yang Anda butuhkan untuk memasang Ruby _development environment_ sepenuhnya pada Windows.

Unduh Ruby installer [disini](https://rubyinstaller.org/downloads/) yang bertuliskan **WITH DEVKIT** versi 2.5.3 dan sesuaikan sistem anda 64/32 bit, jalankan instalasi tersebut, pilih _language_ dan centang _agree to the terms,_ jika terdapat beberapa checkbox centang sebagian saja : 

* [ ] _Install Td/Tk support_
* [x] _Add Ruby executables to your PATH_
* [x] _Associate .rb and .rbw files with this Ruby installation_

Setelah itu klik _"install"_ dan tunggu beberapa menit, dan Selesai !
{% endtab %}
{% endtabs %}

