Nginx config layout
===================

This is a configuration layout for nginx. This layout requires
at least nginx 1.0 for work correctly.

Usage
-----

Make sure nginx package is already installed on your system.

    cd /etc
    mv nginx nginx.dist
    git clone git://github.com/hron84/nginx-configs.git nginx

After it, check the original nginx.conf (in nginx.dist/nginx.conf) and
if it is needed modify pid file and logging directory location if your 
system is not expects the following paths:

 - Pid file: /var/run/nginx.pid
 - Log directory: /var/log/nginx

The example virtual host configuration files are creating separated log file
for each virtual host. It is needed because the configured log format does 
not contain information about vhosts (which virtual host served the actual 
request).

Copyright and licensing
-----------------------

These configuration files are licensed under same terms as
nginx. See the LICENSE file in the root of this repository

Bugs and support
----------------

If you have a trouble with using of this layout or need help
with it, feel free to use GitHub [issue tracker](https://github.com/hron84/nginx-configs/issues).

Do it if you have an idea how can I improve this layout.
