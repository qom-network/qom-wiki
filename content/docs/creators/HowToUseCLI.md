---
title: How to Use CLI
date: 2025-07-01 00:00:00+00:00
draft: false
toc: false
images:
tags: 
---

## Frequently Used Terminal Commands (Mac/Windows)

In this section, we'll introduce commonly used terminal commands. Since Mac and Windows use different commands, we'll only focus on a few that are frequently used on both platforms. Try entering each command in your terminal (Mac) or PowerShell (Windows) as you read through the explanations.

There are many more useful commands—feel free to explore and learn beyond this list!

---

### `pwd`

Displays the current directory path (also known as the "current working directory"). A path is like an address within your computer. Even if you're in the same building, you can't find something unless you're on the right floor.

Understanding where you are in the file structure is essential.

```bash
$ pwd
```

→ Shows your current location within your computer's file system.

---

### `cd`

Changes the current directory.  
Running `cd` without arguments takes you to your home directory.  
You can check your new location using the `pwd` command.

```bash
$ cd desktop
```

→ Moves into the `desktop` directory.

```bash
$ cd ../
```

→ Moves one level up from the current directory.

```bash
$ cd ../../
```

→ Moves two levels up in the directory structure.

```bash
$ cd desktop/test
```

→ Moves directly into the `test` folder on the desktop.

If the specified directory doesn't exist, you'll get an error:  
`No such file or directory`.

---

### `mkdir`

Creates a new directory (short for "make directory").  
This command **requires** a directory name as an argument.

First, navigate to your desktop and then create a new folder:

```bash
$ cd desktop
$ mkdir test
```

→ This will create a new folder called `test` on your desktop.

---

### `touch` (Mac/Linux) / `New-Item` (PowerShell)

Creates a new file in the current directory.

On **Mac/Linux**:
```bash
$ touch memo.md
```

On **Windows PowerShell**:
```bash
$ New-Item memo.md
```

→ A new file named `memo.md` will be created in the current folder.

---

### `ls`

Lists the contents of a directory.  
Run `ls` without arguments to display the contents of the current directory.

You can also provide a path as an argument to list the contents of a specific directory.

```bash
$ ls test
```

→ Displays the contents of the `test` directory. You should see the `memo.md` file you created earlier.

---

Once you understand these commands, try the following exercise:

1. Create a new directory somewhere easy to manage.
2. Use the `cd` command to move into that directory.
3. Use `git clone` to copy the `hello-world` repository to your local machine.

You're now ready to begin working in your own development environment!
