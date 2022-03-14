# Bandit Level 11 → Level 12

## Level Goalll from master

The password for the next level is stored in the file data.txt, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions

## Commands you may need to solve this level

grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

## Solution

```
cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
```

# Login to next box
```
ssh bandit12@bandit.labs.overthewire.org -p 2220
```

Password for Level 12
```
5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu
```
