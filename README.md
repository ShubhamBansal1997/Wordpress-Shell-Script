# Wordpress Shell Script


It is a shell script to install WORDPRESS on the ubuntu server [php,mysql,nginx,wordpress].

  - Work on all cloud services (aws, digitalocean)
  - Easy to use
  - Setup in 2 mins
  - Work with most of php framworks and open scripts  
  - Use php7.0 and most of the php packages(php7.0-mysql php7.0-fpm php7.0-mbstring php7.0-xml php7.0-curl php7.0-json mcrypt php7.0-mcrypt php7.0-zip )
  - More Suitable for Ubuntu 14.04

# How to use !

  - In your ubuntu server 
    ```sh
    [sudo] git clone https://github.com/ShubhamBansal1997/Wordpress-Shell-Script.git
    cd Wordpress-Shell-Script.git
    [sudo] chmod +x wordpress.sh
    ./wordpress.sh
    ```
  - Wordpress Installation process started
    ```sh
    Use sudo[y]:y
    Enter your appname[hello-web]:testing
    Enter your domain name[mydomain.com]:testing.com
    Enter your database name[hello-world]:shubham
    Enter your server public ip[127.0.0.1]: 23.34.12.31
    Enter the wordpress version[4.7.5]: 4.7.2
    ```
  - Please connect your domain to your public ip otherwise it would show errors
  - Installation process started it asked for various permissions in between kept yes for them
    
Points to remember:
---
  - Please don't stop this after running otherwise you have to reset your server
  - Your nginx configuration can be edited here
    ```sh
    [sudo] nano /etc/nginx/conf.d/default.conf 
    ```
  - After changing your nginx configuration, restart ngnix
    ```sh
    [sudo] /etc/init.d/nginx restart
    ```
  - See error log of the server here
    ```sh
    cat /var/log/nginx/error.log
    ```
  - After making any change in php configuration.Run this
    ```sh
    [sudo] /etc/init.d/php7.0-fpm restart
    ```

Note for Users
----

  - Post your requirements and error in issue
  - Would update as per needs and issues

License
----

MIT


**Free Software, Hell Yeah!**


