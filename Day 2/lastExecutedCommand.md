# MCQ on UNIX Command to Repeat the Last Executed Command

### Question:
Which UNIX command is used to repeat the last executed command?

A) `!!`  
B) `repeat`  
C) `last`  
D) `history`  

### Correct Answer: 
**A) `!!`**

### Explanation of Each Option:

- **A) `!!`**  
  The `!!` command is used to repeat the last command that was executed in the shell. This is useful for quickly re-running a command without retyping it.  
  **Example:**  
  ```bash
  $ echo "Hello World"  
  Hello World  
  $ !!  
  echo "Hello World"  
  Hello World  
  ```

- **B) `repeat`**  
  The `repeat` command is not a standard UNIX command. It is available in some specific shells (like C shell) but is not commonly found in most UNIX environments. It is used to execute a command multiple times.  
  **Example:**  
  ```csh
  % repeat 3 echo "Hello"  
  Hello  
  Hello  
  Hello  
  ```

- **C) `last`**  
  The `last` command is used to display a list of the last logged-in users, showing the user's login history. It does not repeat the last executed command.  
  **Example:**  
  ```bash
  $ last  
  user1    pts/0        :0           Mon Oct 24 09:24 - 10:00 (00:36)  
  user2    pts/1        :0           Mon Oct 23 14:00 - 15:00 (01:00)  
  ```

- **D) `history`**  
  The `history` command displays the list of previously executed commands. While it helps in viewing past commands, it does not directly repeat them. You can use `!n` (where `n` is the command number) to execute a specific command from history.  
  **Example:**  
  ```bash
  $ history  
  1  echo "Hello World"  
  2  ls  
  3  pwd  
  $ !1  
  echo "Hello World"  
  Hello World  
  ```

### Conclusion:
The correct command to repeat the last executed command is `!!`. It allows users to quickly re-run their previous command without needing to retype it.
