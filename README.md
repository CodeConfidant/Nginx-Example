# Nginx-Example

    A tutorial for hosting static websites with Ubuntu & Nginx.

[![Static Website Hosting with Nginx](logo.png)](https://www.youtube.com/watch?v=FCjrnAP_zfk)

## Installing/Uninstalling Nginx

    To install Nginx type the following command into your terminal:
    sudo apt install nginx

    To remove Nginx type the following command into your terminal:
    sudo apt remove nginx

## Directories

    Website Root Directory:
    /var/www

    Server Configuration File Directory:
    /etc/nginx/sites-available
    
    Server Configuration Symbolic Link Directory:
    /etc/nginx/sites-enabled

    TLS/SSL Certificate & Key Directory:
    /etc/nginx/ssl

## Administrative Commands

    Starting the Server:
    sudo systemctl start nginx
    sudo service nginx start

    Stopping the Server:
    sudo systemctl stop nginx
    sudo service nginx stop

    Restarting the Server:
    sudo systemctl restart nginx
    sudo service nginx restart

    Reloading the Server:
    sudo systemctl reload nginx

    Checking the Server Status:
    sudo systemctl status nginx
    sudo service nginx status

    Disable the Server at Boot-Up:
    sudo systemctl disable nginx

    Enable the Server at Boot-Up:
    sudo systemctl enable nginx

## Private Key & Certificate Generation Commands

    Generate Self-Signed Private Key (2048 Bit Key Length) & Certificate:
    sudo openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout domainName.key -out domainName.crt

    Generate PEM File Certificate (For Secure Email Messaging):
    sudo openssl dhparam -out dhparam.pem 2048
