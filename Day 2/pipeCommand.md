## MCQ: Which Unix command is used to send the output of one command as input to another command?

**A)** `&`  
**B)** `>`  
**C)** `|`  
**D)** `<`

---

### Explanation:

- **A) &**  
  This option is incorrect. The `&` symbol in Unix is used to run a process in the background, not to send the output of one command as input to another command.  
  **Example**:  
  ```bash
  sleep 5 &
  echo "This will run immediately"
  ```

- **B) >**  
  This option is incorrect. The `>` symbol is used for redirecting the output of a command to a file, not another command.  
  **Example**:  
  ```bash
  echo "Hello" > file.txt
  # Output: "Hello" will be written to file.txt
  ```

- **C) |**  
  This option is correct. The `|` (pipe) symbol is used to send the output of one command as input to another command.  
  **Example**:  
  ```bash
  ls | grep "file"
  # Output: Will show the files containing "file" in their names from the ls command output.
  ```

- **D) <**  
  This option is incorrect. The `<` symbol is used to redirect input from a file to a command, not from another command.  
  **Example**:  
  ```bash
  sort < file.txt
  # Output: Sorts the contents of file.txt
  ```

---

### Correct Answer: **C) |**
