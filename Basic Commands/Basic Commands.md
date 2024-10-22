
---

### **1. mkdir 
   - **What it does**: Creates a new directory (folder).
   - **When to use**: Use when you want to create a new folder.
   - **How to use**:  
     ```bash
     mkdir directory_name
     ```

---

### **2. touch 
   - **What it does**: Creates an empty file.
   - **When to use**: Use when you need to create new files.
   - **How to use**:  
     ```bash
     touch file_name.txt
     ```

---

### **3. cat> 
   - **What it does**: Opens a file for input, allowing you to type content into it.
   - **When to use**: Use when you want to create or overwrite a file by typing content into it.
   - **How to use**:  
     ```bash
     cat > file_name.txt
     ```

---

### **4. cat file_name 
   - **What it does**: Displays the contents of a file.
   - **When to use**: Use when you want to view what’s inside a file.
   - **How to use**:  
     ```bash
     cat file_name.txt
     ```

---

### **5. pwd 
   - **What it does**: Prints the current working directory (the folder you’re in).
   - **When to use**: Use when you want to know your current directory.
   - **How to use**:  
     ```bash
     pwd
     ```

---

### **6. passwd 
   - **What it does**: Changes your user password.
   - **When to use**: Use when you need to update or change your login password.
   - **How to use**:  
     ```bash
     passwd
     ```

---

### **7. mv 
   - **What it does**: Moves a file to another location, or renames it.
   - **When to use**: Use to move files or rename them.
   - **How to use**:  
     ```bash
     mv file_name destination_directory
     ```

---

### **8. cp 
   - **What it does**: Copies a file to another location.
   - **When to use**: Use to duplicate files.
   - **How to use**:  
     ```bash
     cp source_file destination_file
     ```

---

### **9. nano 
   - **What it does**: Opens the `nano` text editor.
   - **When to use**: Use when you want to edit files in a simple text editor.
   - **How to use**:  
     ```bash
     nano file_name
     ```

---

### **10. diff 
   - **What it does**: Compares two files and displays the differences.
   - **When to use**: Use when you want to compare two files.
   - **How to use**:  
     ```bash
     diff file1 file2
     ```

---

### **11. tac 
   - **What it does**: Displays file contents in reverse order (last line first).
   - **When to use**: Use to read a file backward.
   - **How to use**:  
     ```bash
     tac file_name.txt
     ```

---

### **12. uniq 
   - **What it does**: Removes duplicate lines from a file or input.
   - **When to use**: Use to remove duplicates and keep unique lines.
   - **How to use**:  
     ```bash
     uniq file_name.txt
     ```

---

### **13. chmod 
   - **What it does**: Changes file permissions.
   - **When to use**: Use to control who can read, write, or execute a file.
   - **How to use**:  
     ```bash
     chmod permissions file_name
     ```

---

### **14. wc 
   - **What it does**: Counts words, lines, and characters in a file.
   - **When to use**: Use to know the size or content count of a file.
   - **How to use**:  
     ```bash
     wc file_name.txt
     ```

---

### **15. rmdir 
   - **What it does**: Removes (deletes) a directory if it is empty.
   - **When to use**: Use to delete empty folders.
   - **How to use**:  
     ```bash
     rmdir directory_name
     ```

---

### **16. rm 
   - **What it does**: Removes (deletes) files or directories.
   - **When to use**: Use to delete files or folders.
   - **How to use**:  
     ```bash
     rm file_name
     ```

---

### **17. nl 
   - **What it does**: Displays the contents of a file along with line numbers.
   - **When to use**: Use when you need to see line numbers in a file.
   - **How to use**:  
     ```bash
     nl file_name.txt
     ```

---

### **18. history 
   - **What it does**: Displays a list of previously entered commands.
   - **When to use**: Use to check your command history.
   - **How to use**:  
     ```bash
     history
     ```

---

### **Deleting Directories with `rm` Command**
To delete directories using the `rm` command in UNIX, use the `-r` (recursive) option to remove the directory and its contents.

#### **Syntax:**
```bash
rm -r directory_name
```

#### **Example:**
To delete a directory named `my_folder` and all its contents:
```bash
rm -r my_folder
```

#### **Important:**
- To delete without confirmation prompts, use the `-rf` option (force deletion):
  ```bash
  rm -rf directory_name
  ```
- Be **cautious** when using `rm -rf`, as it permanently deletes the directory and all its contents without recovery.

---