<h1 align="center">
 Docker File from php8.2  <br>
 (Laravel, Symfony, Wordpress, etc..)
</h1>


![Packagist PHP Version Support](https://img.shields.io/badge/php-%5E8.2-blue)


Docker file for use in PHP Laravels support for php 8.2.
- Symfony
- Laravel
- PhpCake.
- Wordpress.
- Drupal.
- etc.




## 🚀 Installation
### Docker Hub.

From Docker Hub.

In your terminal execute this sentences
```terminal
docker pull xavi78/xavi-php-fpm82-nginx
docker run -p 9000:9000 xavi78/xavi-php-fpm82-nginx  
```
From Docker File.

In your terminal in same folder you down dockerfile execute this sentences.
```terminal
docker build -t xavi78/xavi-php-fpm82-nginx .
docker run -p 9000:9000  --name xavi_php82 xavi78/xavi-php-fpm82-nginx 
```

## :arrow_forward: How to use.
In your web server to use this container add the proxy pass for example:.
### Apache.
```conf
ProxyPassMatch ^/(.*\.php(/.*)?)$ fcgi://xavi_php82:9000/var/www/html/public/$1
```

## :mag_right: Change log
Please see <a href="">CHANGELOG</a> for more information what has changed recently.



## :superhero_woman: Contribute.
Feel free to make as many pull requests as you think fit, because there are so many things to do, all help is welcome.

Here is a guide if you want to take a look()

If you find a bug, let us know <a href="https://github.com/JavierRodriguez78/xavi-php-fpm82-nginx/issues">here</a> .

If you request a new  <a href ="https://github.com/JavierRodriguez78/xavi-php-fpm82-nginxx/pulls"> feature</a>.