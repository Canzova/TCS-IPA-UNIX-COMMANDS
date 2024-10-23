# MCQ: Sorting Data in Reverse Order in Unix

## Question:
Which of the following commands is used to sort the contents of a file in reverse order in Unix?

### Options:
A. `sort -r filename`  
B. `sort -R filename`  
C. `sort -o filename`  
D. `sort -n filename`  

### Correct Answer: 
**A. `sort -r filename`**

---

## Explanation of Options:

### A. `sort -r filename`
- **Explanation**: This command sorts the contents of `filename` in **reverse** order. The `-r` option is specifically used to reverse the results of the sort. For example, if `filename` contains a list of numbers or strings, this command will display them from highest to lowest (or last to first alphabetically).
  
### B. `sort -R filename`
- **Explanation**: This command is **incorrect**. The `-R` option does not exist in the `sort` command. The user may confuse this with `-r` (reverse) but `-R` has no defined function in standard Unix sort operations.

### C. `sort -o filename`
- **Explanation**: This command is also **incorrect**. The `-o` option is used to specify an output file, meaning it will sort the contents and write them to `filename`, but it does not reverse the order of sorting. It needs an additional `-r` option to sort in reverse.

### D. `sort -n filename`
- **Explanation**: This command is **incorrect** as well. The `-n` option sorts the data in **numerical order**, not reverse order. It will sort numbers in ascending order, which is opposite of what the question asks for. To sort numerically in reverse order, you would need to combine `-n` with `-r` (i.e., `sort -nr filename`).

---

## Summary
The correct command to sort data in reverse order in Unix is **A. `sort -r filename`**. This command effectively reverses the natural sorting order of the contents of the specified file.
