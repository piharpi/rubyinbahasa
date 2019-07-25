---
description: >-
  Sebelum kita mempelajari bahasa Ruby kita menginstall alat-alat yang
  dibutuhkan, kamu bisa melewatkan bagian ini jika sudah memiliki alat yang
  dibutuhkan untuk mempelajari ruby.
---

# Pesiapan Alat dan Ruby

## Text Editor

Kamu bisa menggunakan text editor kesayanganmu, namun jika kamu tidak memiliki opsi saya merekomendasikan beberapa text editor yaitu [sublime](https://www.sublimetext.com/), [vscode](https://code.visualstudio.com/), [atom](https://atom.io/), [rubymine](https://www.jetbrains.com/ruby/) atau [VIM](https://www.vim.org/), semua text editor yang tersebut tersedia disemua sistem operasi \(Linux, Windows, MacOS\) tapi saya menyarankan menggunakan **vscode** jika kamu bingung.

## Terminal

Ada beberapa jenis software terminal, yaitu [Tmux](https://github.com/tmux/tmux/wiki), [Bash](https://www.gnu.org/software/bash/), [Git Bash](https://git-scm.com/downloads), [Cmder](http://cmder.net/), [Hyper](https://hyper.is/), [XTerm](https://invisible-island.net/xterm/), dan sebagainya, gunakan terminal kesukaan kamu, atau jika kamu menggunakan sistem operasi Windows saya sarankan untuk menggunakan Git Bash atau Cmder.

## Ruby

Versi ruby yang digunakan pada buku ini adalah `ruby 2.5.3` jika kamu mempunyai cara tersendiri untuk melakukan instalasi ruby, kamu bisa mengikuti cara kamu sendiri. Namun, jika tidak kamu bisa mengikuti cara instalasi berikut ini pilih sesuai dengan sistem operasi yang kamu gunakan. 

{% tabs %}
{% tab title="Ubuntu" %}
Pertama, install terlebih dahulu dependency, ini adalah bagian-bagian yang dibutuhkan untuk melanjutkan instalasi berikutnya.

{% code-tabs %}
{% code-tabs-item title="Terminal" %}
```text
curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list

sudo apt-get update
sudo apt-get install git-core curl zlib1g-dev build-essential libssl-dev libreadline-dev libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt1-dev libcurl4-openssl-dev software-properties-common libffi-dev nodejs yarn
```
{% endcode-tabs-item %}
{% endcode-tabs %}

Selanjutnya, kita akan menggunakan [rbenv](https://github.com/rbenv/rbenv) untuk menginstall ruby. rbenv ini alat yang dibuat khusus untuk menginstall ruby dan manajemen versi ruby di komputer kita. Dengan adanya rbenv ini kita bisa memiliki lebih dari satu versi ruby yang terinstall.

Langkah pertama adalah instalasi rbenv itu sendiri. Jalankan perintah berikut ini.

{% code-tabs %}
{% code-tabs-item title="Terminal" %}
```text
cd
git clone https://github.com/rbenv/rbenv.git ~/.rbenv
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
echo 'eval "$(rbenv init -)"' >> ~/.bashrc
exec $SHELL
```
{% endcode-tabs-item %}
{% endcode-tabs %}

Setelah itu, install ruby-build. rbenv membutuhkan ruby-build ini untuk melakukan build terhadap source ruby. Jalankan perintah di bawah untuk menginstallnya.

{% code-tabs %}
{% code-tabs-item title="Terminal" %}
```text
git clone https://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build
echo 'export PATH="$HOME/.rbenv/plugins/ruby-build/bin:$PATH"' >> ~/.bashrc
exec $SHELL
```
{% endcode-tabs-item %}
{% endcode-tabs %}

Sekarang kita menginstall Ruby. Kita menggunakan versi 2.5.3, Caranya sebagai berikut

{% code-tabs %}
{% code-tabs-item title="Terminal" %}
```text
rbenv install 2.5.3
rbenv global 2.5.3
ruby -v
```
{% endcode-tabs-item %}
{% endcode-tabs %}

Saat menjalankan perintah ruby -v maka diterminal pastikan menampilkan informasi seperti berikut ini.

`ruby -v ruby 2.5.3p105 (2018-10-18 revision 65156) [x86_64-linux]`

itu artinya adalah telah berhasil terinstall dengan versi 2.5.3. 

Oke, instalasi ruby di Ubuntu selesai dan kamu bisa melanjutkan kebagian berikutnya.
{% endtab %}

{% tab title="MacOs" %}
Di MacOs kita menggunakan [rbenv](https://github.com/rbenv/rbenv) sebagai alat yang dibuat khusus untuk menginstall ruby dan manajemen versi ruby di komputer kita, namun sebelum itu kita menginstall [Homebrew](https://brew.sh/), brew ini dibutuhkan untuk menginstall rbenv yang tidak tersedia di Apple.

{% code-tabs %}
{% code-tabs-item title="Terminal" %}
```text
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
{% endcode-tabs-item %}
{% endcode-tabs %}

Selanjutnya, jika instalasi brew selesai, install rbenv dan ruby-build menggunakan perintah di bawah ini.

{% code-tabs %}
{% code-tabs-item title="Terminal" %}
```text
brew install rbenv ruby-build

# Menambahkan rbenv dibash dengan itu akan memuat setiap waktu kamu membuka terminal
echo 'if which rbenv > /dev/null; then eval "$(rbenv init -)"; fi' >> ~/.bash_profile
source ~/.bash_profile
```
{% endcode-tabs-item %}
{% endcode-tabs %}

Langkah terakhir menginstall ruby. Kita menggunakan versi, 2.5.3

{% code-tabs %}
{% code-tabs-item title="Terminal" %}
```text
# Install Ruby
rbenv install 2.5.3
rbenv global 2.5.3
ruby -v
```
{% endcode-tabs-item %}
{% endcode-tabs %}

Saat menjalankan perintah `ruby -v` maka diterminal pastikan menampilkan informasi yang menyatakan ruby yang terinstall adalah versi 2.5.3, jika informasi tersebut tampil berarti instalasi ruby telah berhasil dikomputermu.

Oke, instalasi ruby di Ubuntu selesai dan kamu bisa melanjutkan kebagian selanjutnya.
{% endtab %}

{% tab title="Windows" %}
Ada sebuah alat bantu yang membantu kamu memasang Ruby : [RubyInstaller](https://rubyinstaller.org/). Ini memberikan apapun yang kamu butuhkan untuk memasang Ruby _development environment_ sepenuhnya pada Windows.

Unduh Ruby installer [disini](https://rubyinstaller.org/downloads/) yang bertuliskan **WITH DEVKIT** versi 2.5.3 dan sesuaikan sistem kamu 64/32 bit, jalankan instalasi tersebut, pilih _language_ dan centang _agree to the terms,_ jika terdapat beberapa checkbox centang sebagian saja : 

* [ ] _Install Td/Tk support_
* [x] _Add Ruby executables to your PATH_
* [x] _Associate .rb and .rbw files with this Ruby installation_

Setelah itu klik _"install"_ dan tunggu beberapa menit, dan Selesai !
{% endtab %}
{% endtabs %}



