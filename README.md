# Apache-Virtual-Hosts
There are conf files for apache2 virtual hosts

1) dev.local.conf - conf file for the simple website
2) dev.local-ssl.conf - conf file for the website with ssl:
- to create the cert: <br />
`openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout mysitename.key -out mysitename.crt`

To enable the host: <br />
`sudo a2ensite dev.local`

Reload Apache2: <br />
`sudo service apache2 reload`
