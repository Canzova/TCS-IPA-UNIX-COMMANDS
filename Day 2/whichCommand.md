# Unix Command: `which`

The `which` command in Unix is used to locate the executable file associated with a given command by searching through the directories listed in the environment variable `PATH`. It returns the binary path of the executable if found.

## Syntax
```bash
which [options] <command>
```

### Options
- `--skip-alias`: Skip any aliases that may exist for the command.
- `--skip-functions`: Skip shell functions.

## Example Usage
1. To find the path of the `ls` command:
   ```bash
   which ls
   ```

   **Output**:
   ```
   /bin/ls
   ```

2. To find the path of the `python` command:
   ```bash
   which python
   ```

   **Output**:
   ```
   /usr/bin/python
   ```

## Multiple Choice Question (MCQ)

**What does the `which` command do in Unix?**

A) It lists all available commands.  
B) It shows the location of the executable file associated with a command.  
C) It displays the current working directory.  
D) It changes the file permissions.

### Correct Answer: B) It shows the location of the executable file associated with a command.

## Explanation of Options

- **A) It lists all available commands.**  
  This option is incorrect. The `which` command does not list all available commands; it only finds the path of a specified command.

- **B) It shows the location of the executable file associated with a command.**  
  This option is correct. The primary function of the `which` command is to locate the executable file for the given command in the directories specified by the `PATH` environment variable.

- **C) It displays the current working directory.**  
  This option is incorrect. The command to display the current working directory is `pwd` (print working directory), not `which`.

- **D) It changes the file permissions.**  
  This option is incorrect. The command to change file permissions is `chmod`, not `which`.

## Conclusion

The `which` command is a simple yet powerful tool for locating executables in Unix systems. Understanding this command can help users navigate their system's commands more effectively.
```