## Send a message to me
1. Save the following public key to a file:
```
-----BEGIN PGP PUBLIC KEY BLOCK-----
Version: SKS 1.1.6
Comment: Hostname: pgp.mit.edu

mDMEYgYRXxYJKwYBBAHaRw8BAQdA1Kcjlh+m/tM4JGEcsiVhIVW2dGI0si/kfBhBtD159W60
GlVwa2FyIExpZGRlciA8dXBrYXJAcG0ubWU+iJQEExYKADwWIQSLzjN9q9+HZ+eY+auRRGFw
PaiEiQUCYgYRXwIbAwULCQgHAgMiAgEGFQoJCAsCBBYCAwECHgcCF4AACgkQkURhcD2ohIkN
GwEAwpGY+Dhdc+LE8/9YT/KxfxHDNKFPtuisAqR6lI+5NykBAPqUXiWQVV81wWLnS2fHAtag
jFmgtQ7SpiizzUwQ+V4IuDgEYgYRXxIKKwYBBAGXVQEFAQEHQH9y79bMVdTeSGVRCYBPZbfU
s7wR2Tl97AxrwyOhGPpIAwEIB4h4BBgWCgAgFiEEi84zfavfh2fnmPmrkURhcD2ohIkFAmIG
EV8CGwwACgkQkURhcD2ohInr0QD/Qj8jitZBSH7/ynPyo3o/UEWfW6xNzQ0F4u61h2/be5EA
+wUPAcz1YM+nInjJZVbYAuwjOTtU/+YlVvE3kEnAeWgF
=p3Iu
-----END PGP PUBLIC KEY BLOCK-----
```
2. import key to sign the message
```
gpg2 --import name_of_pub_key_file
```
## Notes for me
### Encrypt
```
echo "secret text" | gpg2 --encrypt --armor -r upkar@pm.me
```

### Decrypt
```
echo "-----BEGIN PGP MESSAGE-----helloworld-----END PGP MESSAGE-----" | gpg2 --decrypt
```
