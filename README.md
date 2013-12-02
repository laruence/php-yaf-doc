####Yaf Document

####How to build

#####Requirement

1. PHP-5.3+
2. PHD
````
 $ pear install phpdocs/PhD
 $ pear install phpdocs/PhD_Generic phpdocs/PhD_PHP
 $ phd --help
````
#####English Manual
######Checkout PHP doc tree

````
 $ mkdir /tmp/svn
 $ cd /tmp/svn
 $ svn co https://svn.php.net/repository/phpdoc/modules/doc-en doc-en
 $ cd /tmp/svn/doc-en
````

######Yaf doc

Yaf documents could be found under doc-en/en/reference/yaf

######Build

````
$ /path-to-php/bin/php -n -d memory_limit=2G doc-base/configure.php --with-php=/path-to-php/bin/php --enable-xml-details
$ /path-to-ph/bin/phd -d doc-base/.manual.xml --format=php --package=PHP --partial=book.yaf
````

if no errros are reported, then you can find the output under doc-en/output

#####Chinese Manual

######Checkout PHP doc tree

````
 $ mkdir /tmp/svn
 $ cd /tmp/svn
 $ svn co https://svn.php.net/repository/phpdoc/modules/doc-zh doc-zh
 $ cd /tmp/svn/doc-zh
````

######Yaf doc

Yaf documents could be found under doc-zh/zh/reference/yaf

######Build

````
$ /path-to-php/bin/php -n -d memory_limit=2G doc-base/configure.php --with-php=/path-to-php/bin/php --enable-xml-details
$ /path-to-ph/bin/phd -d doc-base/.manual.xml --format=php --package=PHP --partial=book.yaf
````
