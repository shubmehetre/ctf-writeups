# Bandit Level 9 → Level 10

## Level Goal

The password for the next level is stored in the file data.txt in one of the few human-readable strings, preceded by several ‘=’ characters.

## Commands you may need to solve this level

grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

## Solution

- strings command prints string of readable characters from a file

```
strings data.txt | grep '==='
```

# Login to next box
```
ssh bandit10@bandit.labs.overthewire.org -p 2220
```

Password to Level 10
```
truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk
```
