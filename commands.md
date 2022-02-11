### encrypt
```
echo "secret text" | gpg --encrypt --armor -r upkar@pm.me
```

### decrypt
```
echo "-----BEGIN PGP MESSAGE-----helloworld-----END PGP MESSAGE-----" | gpg2 --decrypt
```

### import my public key
```
gpg --import name_of_pub_key_file
```
