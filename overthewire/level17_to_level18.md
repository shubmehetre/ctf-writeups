# Bandit Level 17 → Level 18

## Level Goal

There are 2 files in the homedirectory: passwords.old and passwords.new. The password for the next level is in passwords.new and is the only line that has been changed between passwords.old and passwords.new

## Commands you may need to solve this level

cat, grep, ls, diff

## Solution

```
diff passwords.new passwords.old
```

# Login to next box

```
ssh bandit18@bandit.labs.overthewire.org -p 2220
```

Password for Level 17

```
kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd
```

- This will give Bye Bye.
