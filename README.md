# Nginx-Example

    A tutorial for hosting static websites with Ubuntu & Nginx.

[![Static Website Hosting with Nginx](logo.png)](https://www.youtube.com/watch?v=OHMWGj6D01U)

## Installing/Uninstalling Nginx

    To install Nginx type the following command into your terminal:
    sudo apt install nginx

    To remove Nginx type the following command into your terminal:
    sudo apt remove nginx

## Directories

    Website Root Directory:
    /var/www

    Server Configuration File Directory:
    /etc/nginx/sites-enabled

    TLS/SSL Certificate & Key Directory:
    /etc/nginx/ssl

## Administrative Commands

    Starting the Server:
    sudo service nginx start

    Stopping the Server:
    sudo service nginx stop

    Restarting the Server:
    sudo service nginx restart

    Checking the Server Status:
    sudo service nginx status

## Certificate & Key Generation Commands

    Generate Certificate & Private Key:
    sudo openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout domainName.key -out domainName.crt

    Generate PEM File Certificate (For Secure Email Messaging):
    sudo openssl dhparam -out dhparam.pem 2048
