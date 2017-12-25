## Installation

To start current application it's need to add ENCRYPT_KEY to Environment variables.

## Encrypting/Decrypting

The properties files contains encrypted passwords. 
It's working thanks for Environment variable 'ENCRYPT_KEY'. 
To encrypt some string it's need to send it in body of HTTP method:
POST http://config-service:8888/encrypt
It's also need to add Authorization Header which will contain username and password for Basic auth.

To decrypt some string it's need to do the same but uri will be:
POST http://config-service:8888/decrypt