## MCQ: Which command is used to print the last 100 lines of a file named `data.txt` in Unix?

A) `tail -100 data.txt` OR `tail -n 100 data.txt`
B) `head -100 data.txt`  
C) `cat data.txt`  
D) `grep -100 data.txt`

### Correct Answer:

**A) `tail -100 data.txt`**

### Explanation of Each Option:

- **A) `tail -100 data.txt`**  
   This command prints the last 100 lines of the file `data.txt`. The `tail` command is used to display the end (last part) of a file, and the `-100` option specifies the number of lines to be printed.

  - **Implementation Example:**
    ```bash
    tail -100 data.txt
    ```
    Output: Displays the last 100 lines of the file `data.txt`.

- **B) `head -100 data.txt`**  
   This command prints the first 100 lines of the file `data.txt`. The `head` command is used to display the beginning (first part) of a file, and the `-100` option specifies the number of lines to be printed.

  - **Implementation Example:**
    ```bash
    head -100 data.txt
    ```
    Output: Displays the first 100 lines of the file `data.txt`.

- **C) `cat data.txt`**  
   This command prints the entire content of the file `data.txt` to the terminal. `cat` is used to display the content of a file but does not limit the output to a specific number of lines.

  - **Implementation Example:**
    ```bash
    cat data.txt
    ```
    Output: Displays the full content of `data.txt`.

- **D) `grep -100 data.txt`**  
   This command is incorrect. The `grep` command is used for searching text patterns within files, not for displaying a specific number of lines.

  - **Implementation Example:**
    ```bash
    grep "pattern" data.txt
    ```
    Output: Displays lines containing the search pattern in `data.txt`, but it doesn't limit the output to any number of lines.

---

### Usage Tip:

If you want to see a different number of lines, you can replace `100` with any number. For example, to display the last 50 lines, use:

```bash
tail -50 data.txt
```
