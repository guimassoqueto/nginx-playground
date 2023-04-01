# nginx-playground

[NGINX docs](https://nginx.org/en/docs/)
[NGINX main site](https://www.nginx.com/)

## Installing from tarball:

1 - go to nginx.org/en/download.html  
2 - save the tar.gz in your disc  
3 - `$ tar -xf [NGINX tar.gz file]`  
4 - enter in extracted folder and `$ ./configure`  
5 - Look for the errors and install the required packages [you may need install libssl-dev]  
6 - `$ ./configure --help`  
7 - For more information about instalation options go to https://nginx.org/en/docs/configure.html  
8 - Run the basic command (optional, for custom options see 7): `./configure --sbin-path=/usr/bin/nginx --conf-path=/etc/nginx/nginx.conf --error-log-path=/var/log/nginx/access.log --with-pcre --pid-path=/var/run/nginx.pid --with-http_ssl_module`  
9 - run `$ sudo make install`  
10 - `nginx`'  
11 - Certify that the instalation worked by checking nginx versio: `$ nginx -V`  

## Create an NGINX service
0 - stop ngix running processes  
1 - https://www.nginx.com/resources/wiki/start/topics/examples/systemd/  
2 - Save the script in the path provided by the link above  
3 - `systemctl start nginx`  
4 - `systemctl enable nginx` (start service automatically on boot)  
