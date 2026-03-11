 <p align="center">
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linux/linux-original.svg" height="70"/>
</p>

# Linux Commands Cheat Sheet

Linux commands allow users to interact with the operating system through the terminal. These commands help manage files, directories, and system operations efficiently.

This cheat sheet provides a quick reference to commonly used Linux commands.

---

## File and Directory Commands

<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linux/linux-original.svg" height="22"/>

These commands help manage files and directories in the Linux file system.

| Command             | Description                                                                |
| ------------------- | -------------------------------------------------------------------------- |
| `ls`                | Lists files and directories in the current folder                          |
| `ls -l`             | Lists files with detailed information such as permissions, owner, and size |
| `cd directory_name` | Changes the current directory                                              |
| `cd ..`             | Moves to the parent directory                                              |
| `mkdir folder_name` | Creates a new directory                                                    |
| `rmdir folder_name` | Removes an empty directory                                                 |
| `rm filename`       | Deletes a file                                                             |

Example:

```bash
ls
```

Example output:

```
file1.txt
file2.txt
folder1
```

---

## File Operations

<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/bash/bash-original.svg" height="22"/>

These commands are used to manipulate and view file contents.

| Command                 | Description                                        |
| ----------------------- | -------------------------------------------------- |
| `cp source destination` | Copies a file from one location to another         |
| `mv source destination` | Moves or renames a file                            |
| `cat filename`          | Displays the content of a file                     |
| `less filename`         | Views file content page by page                    |
| `grep "text" filename`  | Searches for a specific text pattern inside a file |

Example:

```bash
cp file1.txt backup.txt
```

This command creates a copy of `file1.txt` named `backup.txt`.

---

## Summary

Linux commands provide powerful tools for managing files and interacting with the operating system through the terminal. Learning these basic commands is essential for developers, system administrators, and anyone working with Linux-based environments.
