# Hotel Management System
## Table of Contents
- [Setup](#setup)
- [Screenshots](#screenshots)
- [For developer](#for-developer)

## Setup
1. Make sure you have `MySQL` and a web server to run/interpret `PHP` in your system.
2. Clone or download the repo and put it to `xampp/htdocs/` if you're using windows, otherwise check tutorial(s) for your corresponding web server and OS. 
3. Install dependencies for JavaScript, `npm install` and PHP, `composer install`.
4. Create a database named `hotel` and run the script `hotel.sql` to create tables. Make sure your configuration matches with `app/DB.php`, otherwise make the desired changes.
5. Run the app by `http://localhost/hotel-mgmt-system-master/index.php`.
 


## For developer
**Run PHP unit tests**
```
$ ./vendor/bin/phpunit tests
```
```
$ ./vendor/bin/phpunit tests/CustomerHandlerTest.php
```
```
$ ./vendor/bin/phpunit --filter testUpdateCustomer tests
```
**Run PHP code beautifier and fixer**
```
$ ./vendor/bin/phpcbf app/process_login.php --standard=ruleset.xml
```
```
$ ./vendor/bin/phpcbf app/*/*.php --standard=ruleset.xml
```
**Run ESLint to format/fix JavaScript code**
```
npm run eslint
```
```
npm run eslint -- --fix
```
