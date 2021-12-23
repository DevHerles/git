# Git useful commands

## Change the current working directory to the local repository in which you want to set your Git config

```bash
git config user.email "foo@bar.com"
git config user.name "Foo Bar"
```

## Verify your changes

```bash
$ git config user.email
foo@bar.com
```

```bash
$ git config user.name
Foo Bar
```

## Remove local untracked files from the current Git branch

```bash
❯ git clean -h
usage: git clean [-d] [-f] [-i] [-n] [-q] [-e <pattern>] [-x | -X] [--] <paths>...

    -q, --quiet           do not print names of files removed
    -n, --dry-run         dry run
    -f, --force           force
    -i, --interactive     interactive cleaning
    -d                    remove whole directories
    -e, --exclude <pattern>
                          add <pattern> to ignore rules
    -x                    remove ignored files, too
    -X                    remove only ignored files
```

**Examples**:
If you want to see which files will be deleted

```bash
❯ git clean -n
```

Use the **-f** option to delete files por real!

```bash
❯ git clean -n
```

To remove directories, use the **-f -d** or **-fd** option to delete files por real!

```bash
❯ git clean -f -d
❯ git clean -fd
```

To remove ignored files, use the **-f -X** or **-fX**

```bash
❯ git clean -f -X
❯ git clean -fX
```

To remove ignored and non-ingored files, use the **-f -x** or **-fx**

```bash
❯ git clean -f -x
❯ git clean -fx
```
