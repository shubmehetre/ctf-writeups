# Bandit Level 15 → Level 16

## Level Goal

The password for the next level can be retrieved by submitting the password of the current level to port 30001 on localhost using SSL encryption.

## Commands you may need to solve this level

ssh, telnet, nc, openssl, s_client, nmap

## Solution

```
echo 'BfMYroe26WYalil77FoDi9qh59eK5xNr' | openssl s_client -connect localhost:30001 -ign_eof
```

# Login to next box
```
ssh bandit16@bandit.labs.overthewire.org -p 2220
```

Password for Level 12
```
cluFn8wTiGryunymYOu4RcffSxQluehd
```
