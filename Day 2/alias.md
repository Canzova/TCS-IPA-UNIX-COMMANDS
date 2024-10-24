# Alias Command in Unix

## What is the `alias` Command?

The `alias` command in Unix is used to create shortcuts or custom commands for longer command strings. By creating an alias, you can simplify the command-line experience, making it easier to execute frequently used commands with a shorter or more memorable name.

### Syntax

```
alias name='command'
```

### Example of Creating an Alias

To create an alias that allows you to list all files (including hidden files) with detailed information, you can use:

```bash
alias ll='ls -la'
```

After creating this alias, typing `ll` in the terminal will execute `ls -la`.

## MCQ on Alias Command

**Question:** What does the following command do?  
```bash
alias gs='git status'
```

### Options:
1. A) Creates an alias named 'gs' that executes the 'git status' command.
2. B) Removes the alias named 'gs' from the system.
3. C) Displays the current status of the Git repository.
4. D) Lists all the aliases defined in the current session.

### Correct Answer:
**1. A) Creates an alias named 'gs' that executes the 'git status' command.**

## Explanation of Each Option:

- **A) Creates an alias named 'gs' that executes the 'git status' command.**  
  This is the correct answer. The command creates a shortcut `gs` for `git status`, allowing the user to type `gs` to quickly check the status of their Git repository.

- **B) Removes the alias named 'gs' from the system.**  
  This option is incorrect. To remove an alias, you would use the `unalias` command, such as `unalias gs`.

- **C) Displays the current status of the Git repository.**  
  This option is misleading. While `git status` does display the status of the repository, the command `alias gs='git status'` does not execute it. It only defines the alias.

- **D) Lists all the aliases defined in the current session.**  
  This option is incorrect. To view all aliases, you can simply type `alias` in the terminal, but the provided command does not perform this action.

## Implementation Examples

### Example 1: Creating an Alias

```bash
alias ll='ls -la'
```
- **Usage:** Typing `ll` will execute `ls -la`, listing all files in the current directory in long format, including hidden files.

### Example 2: Viewing Existing Aliases

To view all defined aliases, simply type:

```bash
alias
```

### Example 3: Removing an Alias

To remove the alias you created:

```bash
unalias ll
```

Now, typing `ll` will no longer have any effect.

### Example 4: Making Aliases Permanent

To make aliases permanent, you can add them to your shell configuration file (e.g., `.bashrc`, `.bash_profile`, or `.zshrc`):

```bash
echo "alias ll='ls -la'" >> ~/.bashrc
source ~/.bashrc
```

This will ensure the alias is available in every new terminal session.

```