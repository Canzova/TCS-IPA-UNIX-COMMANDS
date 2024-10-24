# Understanding the `$?` Variable in UNIX

The `$?` variable in UNIX is used to capture the exit status of the last executed command. An exit status of `0` usually indicates success, while any non-zero value indicates an error.

## MCQ Question

**What does the `$?` variable signify in UNIX?**

1. A) The number of active processes
2. B) The last executed command
3. C) The exit status of the last command
4. D) The current user's home directory

### Explanation of Options

- **A) The number of active processes**  
  This option is incorrect. `$?` does not provide information about active processes. To check active processes, you would use commands like `ps` or `top`.

- **B) The last executed command**  
  This option is misleading. While `$?` is related to the last executed command, it does not contain the command itself but rather the status of that command.

- **C) The exit status of the last command**  
  This option is correct. `$?` holds the exit status of the last command executed, indicating whether it was successful (`0`) or failed (non-zero).

- **D) The current user's home directory**  
  This option is incorrect. The current user's home directory can be accessed using the variable `HOME` or `~`.

## Implementation Examples

### Example 1: Successful Command

```bash
$ ls
file1.txt  file2.txt  directory
$ echo $?
0
```

In this example, the `ls` command executed successfully, and `$?` returned `0`.

### Example 2: Failing Command

```bash
$ cd non_existent_directory
bash: cd: non_existent_directory: No such file or directory
$ echo $?
1
```

Here, attempting to change to a non-existent directory resulted in an error, and `$?` returned `1`, indicating failure.

### Example 3: Chaining Commands

```bash
$ mkdir test_directory
$ echo $?
0
$ cd test_directory
$ echo $?
0
$ rmdir test_directory
$ echo $?
0
```

In this sequence, all commands execute successfully, and `$?` consistently returns `0`.

### Example 4: Using in Scripts

```bash
#!/bin/bash

cp source.txt destination.txt
if [ $? -eq 0 ]; then
    echo "Copy successful!"
else
    echo "Copy failed!"
fi
```

In this script, the exit status of the `cp` command is checked, and an appropriate message is displayed based on the result.

## Conclusion

The `$?` variable is a powerful tool for checking the success or failure of commands in UNIX, helping users and scripts to handle errors effectively.