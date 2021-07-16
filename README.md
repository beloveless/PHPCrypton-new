# PHPCrypton

<p style="text-align: justify;">PHPCrypton dikembangkan untuk dapat melakukan obfuskasi layout dan enkripsi menggunakan algoritme AES-256 pada kode sumber PHP. <br />
Terdapat dua fungsi yang dapat digunakan oleh pengguna PHPCrypton yaitu <em>single obfuscation</em> dan <em>directory obfuscation.</em></p>
<p style="text-align: justify;">&nbsp;</p>

| Fungsi PHPCrypton | Kegunaan |
| ------ | ------ |
| Single Obfuscation | Melakukan obfuskasi layout dan enkripsi pada satu berkas PHP yang telah ditentukan |
| Directory Obfuscation | Melakukan obfuskasi layout dan enkripsi pada suatu direktori yang telah ditentutkan  |

## How to Install PHPCrypton?

### 1. Download Requirement
        sudo apt-get install git gcc make re2c php php-json php-dev libpcre3-dev libboost-all-dev 

### 2. Install PHP-CPP first

        git clone https://github.com/CopernicaMarketingSoftware/PHP-CPP.git
        cd PHP-CPP/
        make
        sudo make install

### 3. Install PHPCrypton

        git clone https://github.com/ismakhrnsa/PHPCrypton.git
        cd PHPCrypton/
        sudo make install

## Important!

Change INI_DIR in Makefile according to your machine

make sure you have enable php mod using
        
        phpenmod phpcrypton


## Single Obfuscation

```php
<?php

       PHPCrypton::singleobfuscation("/home/ubuntu/PHPCrypton/examples/DirA/action.php");

?>
```

## Directory Obfuscation

```php
<?php

       PHPCrypton::directoryobfuscation("/home/ubuntu/PHPCrypton/examples/DirA/");

?>
```
