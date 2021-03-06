#Nginx Boilerplate 
Awesome Nginx configuration template and a set of handy must-have snippets.

***
## Features
 * Convenient include-based config structure
 * Optimized defaults
 * Connection and requests rate limitation settings
 * Backend response caching
 * Various predefined locations
 * Advanced logging

## Demo
 * http://nginx-boilerplate.umkus.com/

## Run in trial mode
 * Run `bin/run.sh` as privileged user to restart Nginx in boilerplate mode
 * (optional) Update the `root` directive in `src/nginx-bp/bootstrap/example.conf`
 * (optional) Check `src/nginx-bp/upstreams/php.conf` to match your php-fpm setup (socket vs TCP/IP)
 * Go to http://localhost/

## Run in UI generator mode
 * Run `bin/ui.sh` to start the UI (you can provide a `server:port` as an optional argument)
 * (optional) Or set up `ui/` as the document root for a new virtualhost and run it from a web-server
 * Got to `localhost:5517` (or whatever you specified as an optional argument)
 * Configure your boilerplate and hit the download button
 * (optional) If you have boilerplate running in a trial mode, hit test drive button to see how it works live!

## If something doesn't work
 * Make sure you have `cgi.fix_pathinfo` set to `1` or commented out in php.ini
 * Check the contents of `/var/log/nginx/yoursitename.error.log`
 * Make sure to have proper file/folder permissions for config files
 * Create an issue on the project's github page
