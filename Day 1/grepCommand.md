# Using the `grep` Command to Search for a Pattern at the Beginning of a Line

## Objective
Find lines in a file that start with a specific pattern (e.g., the string "pat") using the `grep` command.

## Command Syntax
```bash
grep "^pattern" filename
```

### Explanation
- `^`: Anchors the search to the **beginning of a line**.
- `pattern`: The specific string to search for (e.g., "pat").
- `filename`: The name of the file to search in.

---

## Example File (`sample.txt`)
Suppose you have a file called `sample.txt` with the following contents:

```
patience is a virtue
The patient waits
pat on the back
pathetic excuse
It's a pattern recognition task
```

---

## Options and Detailed Answers

### 1. Search for Lines Starting with "pat"
```bash
grep "^pat" sample.txt
```
**Output**:
```
patience is a virtue
pat on the back
pathetic excuse
```
**Explanation**: This command finds all lines starting with "pat".

---

### 2. Search for Lines Starting with "PAT" (Case Sensitive)
```bash
grep "^PAT" sample.txt
```
**Output**:
*(no output)*

**Explanation**: No matches are found because "PAT" does not appear at the start of any line.

---

### 3. Search for Lines Starting with "pat" (Case Insensitive)
```bash
grep -i "^pat" sample.txt
```
**Output**:
```
patience is a virtue
pat on the back
pathetic excuse
```
**Explanation**: The `-i` option makes the search case insensitive, matching "pat", "PAT", etc.

---

### 4. Count Lines Starting with "pat"
```bash
grep -c "^pat" sample.txt
```
**Output**:
```
3
```
**Explanation**: The `-c` option counts the number of matching lines, indicating there are 3 lines that start with "pat".

---

### 5. Show Line Numbers of Matching Lines
```bash
grep -n "^pat" sample.txt
```
**Output**:
```
1:patience is a virtue
3:pat on the back
4:pathetic excuse
```
**Explanation**: The `-n` option displays line numbers along with the matching lines.

---

### 6. Search in Multiple Files
```bash
grep "^pat" sample.txt another_sample.txt
```
**Output**:
*(output from both files where lines start with "pat")*

**Explanation**: Searches both `sample.txt` and `another_sample.txt` for lines starting with "pat".

---

## Conclusion
Using `grep` with the `^` symbol effectively searches for patterns at the beginning of lines. By employing options like `-i`, `-c`, and `-n`, you can customize your search to meet specific needs.
```
