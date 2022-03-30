<p align="center"><a href="https://laravel.com" target="_blank">
<img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

Este projeto básico para início de um sistema com Laravel 8 conta com Autenticação de usuários, autorizações de usuários com Perfis e Permissões utilizando o pacote do <a href="#">Spatie</a> <a href="https://github.com/spatie/laravel-permission">Laravel Permission</a>, gerenciamento de usuários e perfis. 
O projeto possui implementação de registro de logs utilizando o Pacote <a href="https://github.com/spatie/laravel-activitylog">laravel-activitylog</a>

O padrão de projeto utilizado é o Repository Patern.


## Start

- cp .env.example .env

Modifique e/ou acrescente as variáveis de ambiente referentes ao Data Base
E-Mail etc.

- Caso precise, modifique as variáveis de valores do usuário Administrador padrão e o nome 
do Perfil de Administrador do Sistema.

- USER_ADMIN="Administrator"
- USER_EMAIL_ADMIN="admin@gmail.com"
- USER_PWD_ADMIN=('123456')

- ROLE_ADMIN="Administrator"

- composer install
- php artisan db:seed --class=PermissionTableSeeder
- php artisan db:seed --class=CreateAdminUserSeeder
