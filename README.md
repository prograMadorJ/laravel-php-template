# laravel-php-template
Template projeto com Laravel PHP

alguns passos para instalar o PHP completo com laravel

# atualizar repositorio para obter o PHP7.1

sudo apt-get install -y python-software-properties

sudo add-apt-repository -y ppa:ondrej/php

sudo apt update -y

sudo apt install php

# pacotes adicionais necessarios para o PHP

sudo apt install php-mbstring php-xml php-zip php-mysql

# instalar o MySQL

sudo apt install mysql-server

# instalar o Composer 

php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"

php -r "if (hash_file('SHA384', 'composer-setup.php') === '544e09ee996cdf60ece3804abc52599c22b1f40f4323403c44d44fdfdd586475ca9813a858088ffbc1f233e9b180f061') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"

php composer-setup.php

php -r "unlink('composer-setup.php');"

# mover e renomear o arquivo composer.phar para o diretorio /usr/local/bin/

sudo mv composer.phar /usr/local/bin/composer

# instalar o laravel pelo composer 

composer global require "laravel/installer"

# criar um link simbolico e mover para o diretorio /usr/local/bin/

ln -s ~/.config/composer/vendor/laravel/installer/laravel laravel-link
 && sudo mv laravel-link /usr/local/bin/laravel
 
 # comando para criar um novo projeto com laravel 

laravel new nome-do-projeto

# comando para iniciar o servidor 

'primeiro deve acessar o diretorio do projeto'

cd nome-do-projeto/

'depois executar o comando com o php artisan'

php artisan serve





