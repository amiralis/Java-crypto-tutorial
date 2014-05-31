# Java-crypto-tutorial


Tutorial on how to use Java Cryptography Extension for
  [Network Security](chimera.ccs.neu.edu).

  **Instructor**: [Amirali Sanatinia](http://www.ccs.neu.edu/home/amirali)

  **Email**: amirali@ccs.neu.edu


## Requirements

 * JDK 1.6+


## OpenSSL

To create *RSA* key pairs you can use the following commands:

   * ```BASH
   $ openssl genrsa -out private_key.pem 2048
   $ openssl pkcs8 -topk8 -inform PEM -outform DER -in private_key.pem -out private_key.der -nocrypt
   $ openssl rsa -in private_key.pem -pubout -outform DER -out public_key.der
   ```
