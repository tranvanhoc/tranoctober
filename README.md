# docker-lamp
Docker example with Apache, MySql 5.7, PhpMyAdmin and Php

I use docker-compose as an orchestrator. To run these containers:

```
docker-compose up -d
```





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



That's it!
