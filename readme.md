# How to use this for AWS Linux Machine

0. Install `docker` and `docker-compose`
1. run `sh run.sh`
    - this will install certbot
2. Once installed, it will prompt:
    - `How would you like to authenticate with the ACME CA?`
    - You choose `Place files in webroot directory (webroot)`
    - Enter domain name
    - You will be asked for the root, insert `/var/www`
    - Certificates and private key would be generated
    - Turn the nginx off `ssl-setup-nginx`
    - Use your certificate and private key for your web
3. If expired, just run `sudo certbot renew`
