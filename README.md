# Admin Login Finder
Tool to search admin panel instantly and quickly

## How to Use
```
apt-get update && apt-get upgrade
apt install curl
apt install php
apt install ruby
apt install git
git clone https://guthub.com/reyyproject/admin-finder
cd admin-finder
php find php
```
Input your target, then select the panel type or leave it blank to use your own wordlist instead default one

##### Results:
![img](https://github.com/reyyproject/admin-finder/blob/main/admin.jpg)

## Dependencies
+ PHP
+ PHP-Curl

## Optional Dependencies
+ Custom Wordlists

## Default Supported Panel Type
+ **ASP** - This filetype may contain scripts written in VBScript or JavaScript
+ **ASPX** - Same as ASP, but Extended
+ **BRF** - This filetype encodes contracted Braille characters using a numbering system, it's barely used as login panel
+ **CFM** - This filetype are using ColdFusion Markup Language, similar to HTML and XML
+ **CGI** - This filetype are often used for running basic web scripts like formmail or advertisements
+ **JS** - This filetype are used to execute JavaScript instructions in webpages
+ **PHP** - This filetype only used at webpages with extended functionality, most of login panel use this filetype

## HTTP Response Explanation
+ **200 OK** - Request succeded, there is high probability that the login panel is there
+ **302 Found** - Temporary redirected, maybe the login panel is there, maybe not
+ **403 Forbidden** - You don't have access rights because it's unauthorized
+ **404 Not Found** - It's means the URL doesn't recognized
