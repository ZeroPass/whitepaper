# FAQ

## Bip32 key derivation

* _Why don't you use standard Key derivation function PBKDF2?_

PBKDF2 \(Password-Based Key Derivation Function 2\) is designed for password inputs. We don't input password, but a long, random number. Even more importantly, it does not offer derivation of public/private keypairs. Bip32 does.  
  


* _Bip32 is used in deterministic \(bitcoin\) wallets. How does your scheme relate to that?_

Key derivation process is the same, usage of key-pair is different;

| bip32 | bitcoin deterministic wallet | ZeroPass Backup tier |
| :--- | :--- | :--- |
| Master Private Key | Used to transfer/reconstruct whole wallet within different services. | Gets split/distributed and then erased. It can be put together if you lock yourself out \(recovery procedure\). |
| Master Public Key | Used to generate \(child\) public bitcoin addresses without exposing private keys. | Used to encrypt all your passwords \(with his child keys\) that can be decrypted only with \(at this point already erased\) MasterPrivateKey. |

We can then safely sync MasterPublicKey between devices. Even if it gets leaked... it's Public key, it can not expose anything.

