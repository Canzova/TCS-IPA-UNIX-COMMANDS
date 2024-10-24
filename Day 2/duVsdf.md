# Difference Between `du` and `df` Commands in Unix

## `du` (Disk Usage)
- **What it does:** Shows how much disk space specific files and folders are using.
- **When to use it:** When you want to find out how much space a particular folder or file is taking up.
- **Example:** 
  ```bash
  du -h /path/to/folder
  ```
  This will show you the size of the specified folder in a friendly format (like KB, MB).

---

## `df` (Disk Free)
- **What it does:** Displays the total amount of disk space used and available on your entire system or disk drives.
- **When to use it:** When you want to see how much space is left on your hard drive or partition.
- **Example:** 
  ```bash
  df -h
  ```
  This will show you the total size, used space, and free space for all mounted drives.

---

## Quick Comparison
- **`du`:** Focuses on **how much space specific files or folders are using**.
- **`df`:** Focuses on **how much total space is used and available on your drives**.

---

## Visual Summary
- **`du`** = Size of files and folders.
- **`df`** = Total disk space information.
```
