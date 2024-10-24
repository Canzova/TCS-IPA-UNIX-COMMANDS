### Which Unix command is used to display the manual or help pages of a command?

- A. `man`
- B. `help`
- C. `info`
- D. `whatis`

#### Correct Answer: A. `man`

#### Explanation of each option:

- **A. `man`**: The `man` command in Unix is used to display the manual pages of other commands. For example, typing `man ls` shows the manual or documentation for the `ls` command, providing detailed information on its usage, options, and other features.
  
- **B. `help`**: The `help` command provides a brief description of shell built-in commands, but it is not used to display full manual pages like `man`. It's more specific to built-in commands such as `cd` or `echo`, which may not have `man` pages.
  
- **C. `info`**: The `info` command shows more detailed documentation, often more in-depth than `man` pages. However, it's not as commonly used for simple command reference as `man`. It’s more of a general help system than one specific to short command explanations.
  
- **D. `whatis`**: The `whatis` command provides a one-line summary of a command, but it does not display the full manual pages. For example, `whatis ls` will give you a brief description of what `ls` does, but without the details found in a `man` page.

---

### Example Usage:

To display the manual page of the `ls` command, you would use the following command in Unix:

```bash
man ls
```

This command will open the manual page for `ls`, where you can see all the options and explanations for how `ls` works.

Sample output:

```
LS(1)                   User Commands                   LS(1)

NAME
       ls - list directory contents

SYNOPSIS
       ls [OPTION]... [FILE]...

DESCRIPTION
       List information about the FILEs (the current directory by default).
       Sort entries alphabetically if none of -cftuvSUX nor --sort is specified.
```