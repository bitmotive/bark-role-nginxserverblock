BARK: NGINXSERVERBLOCK
=========

Configure an NGINX Server Block with sane defaults.

Requirements
------------

All roles in the Bitmotive Ansible Role Kit are configuration driven.

Customize this role by providing environment variables in your 
shell, host specific in group_vars/, or at the CLI when
prompted during runtime. 

Role Variables
--------------

**NGINXSERVERBLOCK_HOSTNAME**:

The hostname for the server block.

**NGINXSERVERBLOCK_SERVERNAME_STRING**

The servername for the host block.

**NGINXSERVERBLOCK_HTTP_PORT**

The HTTP Port to be used by the server block.

**NGINXSERVERBLOCK_HTTPS_PORT**

"None" or the HTTPS Port to be used by the server block (optional).

**NGINXSERVERBLOCK_SSL_PRIVKEYPATH**

"None" or the filepath to the SSL certificate private key (optional).

**NGINXSERVERBLOCK_SSL_PUBKEYPATH**

"None" or the filepath to the SSL certificate public key file (optional).

**NGINXSERVERBLOCK_REDIRECT_WWW**

"YES" or "NO" to redirect all WWW requests to APEX domain.

**NGINXSERVERBLOCK_SUPPORT_PHP**

"YES" or "NO" to include support for PHP.


Dependencies
------------

Currently assumes sites will be served from `/var/www/` directories. 

Creates a repository for `private_html` and `public_html` and symlinks the
webroot from `public_html` to the desired filepath in `private_html`.

License
-------

MIT

Author Information
------------------

A Bitmotive Project: Build. Incubate. Train.
https://bitmotive.com 
