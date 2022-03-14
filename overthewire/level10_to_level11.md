# Bandit Level 10 → Level 11

## Level Goal

The password for the next level is stored in the file data.txt, which contains base64 encoded data

## Commands you may need to solve this level

grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

## Solution

```
base64 -d data.txt
```

# Login to next box
```
ssh bandit11@bandit.labs.overthewire.org -p 2220
```

Password for Level 11
```
IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR
```
