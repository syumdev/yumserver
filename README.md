# yumserver

## create a sudo user
```
adduser syum
usermod -aG syum sudo
```

## ssh with new user

```
mkdir .ssh
chmod 700 .ssh
echo "${public key}" >> .ssh/authorized_keys
chmod 600 .ssh/authorized_keys
```

## ssh without -i .pem file
```
PasswordAuthentication = yes
```
