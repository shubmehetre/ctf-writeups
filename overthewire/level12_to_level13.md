# Bandit Level 12 → Level 13

## Level Goal

The password for the next level is stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work using mkdir. For example: mkdir /tmp/myname123. Then copy the datafile using cp, and rename it using mv (read the manpages!)

## Commands you may need to solve this level

grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd, mkdir, cp, mv, file

## Solution

Check file type
```
file filename
```

Rename files
```
mv oldname newname
```

To extract gzip: (rename file to .gz extension)
```
gzip -d file.gz
```

To extract bzip2: (rename file to .bz2 extension)
```
bzip2 -d file.bz2
```

To extract tar: (rename file to .tar extension)
```
tar xf file.tar
```

Do above stuff alot of times. In end you will get a ASCII file
```
cat file
```

# Login to next box
```
ssh bandit13@bandit.labs.overthewire.org -p 2220
```

Password for Level 13
```
8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL
```
