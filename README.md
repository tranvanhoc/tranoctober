# docker-lamp
Docker example with Apache, MySql 5.7, PhpMyAdmin and Php

I use docker-compose as an orchestrator. To run these containers:


## Setup new site
1. docker-compose up -d
2. rm -rf www
3. composer create-project october/october www (isntall octobercms)
4. at config/cms.php
  `'disableCoreUpdates' => true,`
5. at www/composer.json
    ```
    "october/rain": "dev-develop as 1.0",
    "october/system": "dev-develop",
    "october/backend": "dev-develop",
    "october/cms": "dev-develop",
    "laravel/framework": "5.5.*@dev",
    ```
6. php artisan october:env
7. php artisan key:generate


## Installation
1. docker-compose up --build
2. cd wwww
3. composer install

* Connect to PhpMyAdmin: 0.0.0.0:8000
  - Username : user
  - Password : test

* Open website:   http://0.0.0.0:8001  

That's it!
