# Linux Fundamentals Part 1 Notes

## Filesystem Navigation

- `pwd` displays the current working directory.
- `ls` lists directory contents.
- `cd` changes directories.
- Absolute paths begin from `/`.
- Relative paths begin from the current directory.

---

## File Management

Create files

```bash
touch file.txt
```

Create directories

```bash
mkdir folder
```

Copy

```bash
cp file.txt backup.txt
```

Move / Rename

```bash
mv old.txt new.txt
```

Delete

```bash
rm file.txt
```

Delete directory

```bash
rm -r folder
```

---

## Viewing Files

```bash
cat
```

---

## Searching

Locate files

```bash
find
```

Search inside files

```bash
grep
```

---

## Finding Files with `find`

The `find` command searches for files and directories based on different criteria.

### Search by exact filename

```bash
find . -name "notes.txt"
```

### Wildcards help when you know part of a filename or its extension, but not the complete name

```bash
find . -name "*.txt"
```


---

### Why use `*.txt`?

The `*` wildcard matches any sequence of characters.

For example:

```text
report.txt
notes.txt
homework.txt
```

can all be found using:

```bash
find . -name "*.txt"
```

This is useful when you know the file extension but not the exact filename.

---

## Log Analysis

### Objective

Retrieve information from log files using pattern matching.

### Workflow

1. Locate the log file.
2. Search using `grep`.
3. Extract the required information.

### Best Practices

- Search known file locations.
- Avoid unnecessary recursive searches.
- Use `-w` when appropriate.
- Reduce noise by narrowing searches.

---

## Permissions

Basic permission concepts

- Read
- Write
- Execute

---

## Manual Pages

```bash
man ls
```

Use manual pages whenever you don't understand a command.

---

## Command History

```bash
history
```

Useful for reviewing previously executed commands.