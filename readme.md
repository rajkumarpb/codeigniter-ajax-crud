## About

This app contains a CRUD interface for flower pots as well a notifier on when to water the flowers.

Technologies used:
* Javascript
* jQuery
* Twitter Bootstrap
* PHP (with Codeigniter framework v3.1.4)

## Installation

1. Create a database using the sqldump file *database_dump.sql*.
2. Have Apache ```mod_rewrite``` enabled
3. Copy *.htaccess.example* to *.htaccess* and modify environment and database settings
4. Run ```bower install``` from the command line. This assumes that you have [bower](https://bower.io/) installed. 

## Running scheduler as Cron

Create a cron entry that runs every 5 minutes using this command:
```
*/5 * * * * /usr/local/bin/php /path/to/epam/index.php notifier cron
```

Note: Make sure email server is configured correctly. You may use this [link](https://codeigniter.com/user_guide/libraries/email.html) for reference.