# Unix Command for String Substitution in a File

## MCQ Question:
**Which Unix command is used to substitute a string in a file?**

A) `grep`  
B) `awk`  
C) `sed`  
D) `cat`

### Answer:  
**C) `sed`**

---

## Explanation of Each Option:

- **A) `grep`:**  
  `grep` is used to search for a string or pattern in a file, but it doesn't modify or replace content. It only outputs the matching lines.

- **B) `awk`:**  
  `awk` is primarily used for pattern scanning and processing. While it can be used for text substitution in complex scenarios, it is not the ideal tool for simple string substitution.

- **C) `sed`:**  
  `sed` (Stream Editor) is used to perform basic text transformations, including substituting a string in a file. It’s commonly used for find-and-replace operations.

- **D) `cat`:**  
  `cat` is used to concatenate and display the contents of a file. It doesn't support text substitution.

---

## Implementation Example:

### Scenario:
We have a file called `example.txt` with the following content:

```
Hello, world!
Welcome to Unix.
Unix is powerful.
```

### Task:
Substitute the word `Unix` with `Linux` in the file.

### Command:

```bash
sed 's/Unix/Linux/g' example.txt
```

### Explanation of the Command:
- **`sed`:** Invokes the stream editor.
- **`s/Unix/Linux/`:** Substitutes the first occurrence of `Unix` with `Linux`.
- **`g`:** The `g` flag ensures that all occurrences in the line are replaced, not just the first one.

### Output:
```
Hello, world!
Welcome to Linux.
Linux is powerful.
```

### In-Place Substitution:
To save the changes directly to the file, use the `-i` option:

```bash
sed -i 's/Unix/Linux/g' example.txt
```

Now, the file `example.txt` will be updated with the new content.

```bash
cat example.txt
```

### Output:
```
Hello, world!
Welcome to Linux.
Linux is powerful.
```