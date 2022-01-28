# Bandit Level 13 → Level 14

## Level Goal

The password for the next level is stored in /etc/bandit_pass/bandit14 and can only be read by user bandit14. For this level, you don’t get the next password, but you get a private SSH key that can be used to log into the next level. Note: localhost is a hostname that refers to the machine you are working on

## Commands you may need to solve this level

ssh, telnet, nc, openssl, s_client, nmap

## Solution

Copy bandit14 key
```
cat sshkey.private
```

Copy this key. Exit bandit13.
save this key in a file. Ex. bandit14_key

Modify permissions
```
chmod 400 bandit14_key
```

Login to bandit14 using key not password
```
ssh bandit14@bandit.labs.overthewire.org -p 2220 -i bandit14_key
```
