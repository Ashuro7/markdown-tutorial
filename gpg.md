# GPG (GNU Privacy Guard)

## Generate keys
To generate public and private keys, run the following command:

```console 
gpg --full-gen-key
```
This would give several prompts like the encryption type, key size, name, email, passphrase, expiration etc. Provide the required information and the keys will be generated.

## List keys

GPG Keys can be listed using the following command:

```console
gpg --list-keys
```

Keys are IDs using their hash signatures.

## Revoke a key

A key can be revoked by importing the revoke certificate. This can be done if the key has been compromised. This step is recommended before deleting the key.

```console
gpg --import path_to_revoke_certificate/revoke_cert.rev
```

Note: The revoke certificate is automatically generated in newer versions of GPG but earlier it had to be manually created.

## Deleting a key

For this first we need to delete the secret (private) key and then the public key.
To delete the secret (private) key, run:

```console
gpg --delete-secret-key <hash_value_of_the_key>
```

To then delete the public key:

```console
gpg --delete-key <hash_value_of_the_key>
```

After the keys have been deleted, we can delete the revoke certificate as well.

## List secret and public key

To list the secret (private) keys:

```console
 gpg --list-secret-keys
 ```

 To list the public keys:

 ```console
 gpg --list-public-keys
 ```
