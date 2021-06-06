# EPSI Password Manager

EPM (EPSI Password Manager) is a project to apply cryptographic concepts in an application to build a secure password manager.

## Goal

Create password management software, this software should allow users to store their passwords securely.

Deploy this software on a server with a CI / CD.

## Constraints

All development will be done on Github by forking this repository.

Passwords must be stored securely:
 - database compromise must not lead to the compromise of passwords
 - server compromise (Man In The Middle) must not lead to the compromise of passwords

Users should be able to:
 - Save a password with metadata (description, site address, etc.)
 - List their passwords
 - Get a password
 - Delete a password

The software must be deployed securely on a server. Deployment should be done automatically by means of a CI / CD.

Best practices for securing a Linux server should be respected as much as possible:
  - TLS
  - File rights
  - Firewall
  - ...

## Expected work

The source code and all scripts must be versioned and published on Github

The application must be usable at a minimum via a REST API in JSON.

The API should be briefly documented: markdown, Swagger, Postman collection, ...

The application will need to be deployed on a remote server.

A document should explain the process of
  - secure passwords
  - securing the server

## Bonus

Managing your own passwords is good, but managing team passwords is better!

Transform the manager so that he can manage team passwords.

Allow file sharing: use of a hybrid cryptosystem.

Using Kuzzle.

## Appendices

_Some resources to help you_

### Kuzzle

_Don't loose time developping an API, there is very few backend business logic in this project._

https://docs.kuzzle.io/core/2/guides/getting-started/run-kuzzle/  
https://docs.kuzzle.io/core/2/guides/getting-started/write-application/  
https://docs.kuzzle.io/core/2/guides/main-concepts/data-storage/  
https://docs.kuzzle.io/sdk/js/7/getting-started/node-js/  
https://docs.kuzzle.io/sdk/js/7/controllers/document/create/  

### Javascript

https://www.npmjs.com/package/node-rsa

### Ruby

https://ruby-doc.org/stdlib-2.6.1/libdoc/openssl/rdoc/OpenSSL/PKey/RSA.html
https://gist.github.com/gevans/6004752

### PHP

https://www.php.net/manual/en/function.openssl-public-encrypt.php
https://www.php.net/manual/en/function.openssl-private-decrypt.php

### Python

https://stuvel.eu/python-rsa-doc/usage.html#encryption-and-decryption

### Java (for masochists)

https://niels.nu/blog/2016/java-rsa
https://www.ruby-lang.org/en/documentation/ruby-from-other-languages/to-ruby-from-java/

### DevOps / SecOps

https://www.digitalocean.com/community/tutorials/how-to-secure-nginx-with-let-s-encrypt-on-ubuntu-20-04  
https://www.ssllabs.com/ssltest/  
https://www.logsign.com/blog/best-practices-for-security-in-ssh/  
https://www.acunetix.com/blog/web-security-zone/hardening-nginx/  
https://docs.kuzzle.io/core/2/guides/getting-started/deploy-your-application/   
