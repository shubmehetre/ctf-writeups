# Bandit Level 8 → Level 9

## Level Goal

The password for the next level is stored in the file data.txt and is the only line of text that occurs only once

## Commands you may need to solve this level

grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

## Solution

- uniq -u gives lines that are unique in a file. uniq can take piped output as arguments
- But the file has to be sorted so we use sort and then pipe it to uniq

```
sort data.txt | uniq -u
```
