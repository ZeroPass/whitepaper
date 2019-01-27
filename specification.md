# Specification

## Cryptography

| Type | Algorithm |
| :--- | :--- |
| Digital Signature | ECDSA\* |
| Symmetric Encryption | AES256-GCM |
| Asymmetric Encryption | ECIES\* |
| Hash function | SHA256 / SHA512 |
| Message authentication code | HMAC |
| Public Key derivation function | Based on  [BIP32](https://github.com/bitcoin/bips/blob/master/bip-0032.mediawiki)\* |
| Secret Sharing | Shamir's Secret Sharing |

\* The algorithm uses [secp256k1](http://www.secg.org/sec2-v2.pdf#page=13) domain parameters to define Elliptic Curve

## Implemntation

**GithHub**: N/A \(yet\)   
  
 ZeroPass implementations will use Crypto++® Library [http://cryptopp.com/](http://cryptopp.com/)  
 to incorporate cryptographic algorithms. Crypto++ is currently the most validated implementations of cryptographic schemes \(for c++\).

©ZeroPass 2017

