# `chown` Command in UNIX

The `chown` (change ownership) command in UNIX is used to change the owner of a file or directory. This command allows users to modify both the owner and the group associated with files or directories.

## MCQ:

**Question: What is the primary use of the `chown` command in UNIX?**

- A) To change the permissions of a file  
- B) To change the owner and group of a file  
- C) To delete a file  
- D) To display file details

---

### **Explanation of Options:**

- **A) To change the permissions of a file**  
  Incorrect. Changing file permissions is done using the `chmod` command, not `chown`.

- **B) To change the owner and group of a file**  
  Correct. The `chown` command is used to change the ownership and group of files and directories. 

- **C) To delete a file**  
  Incorrect. The `rm` command is used to delete files, not `chown`.

- **D) To display file details**  
  Incorrect. The `ls -l` command is used to display detailed information about files, such as ownership, permissions, and more.

---

## Example:

Let's assume we have a file `example.txt` owned by `user1` and the group `group1`. To change the owner to `user2` and the group to `group2`, we use the following command:

```bash
$ ls -l example.txt
-rw-r--r-- 1 user1 group1 0 Oct 24 12:00 example.txt

$ sudo chown user2:group2 example.txt

$ ls -l example.txt
-rw-r--r-- 1 user2 group2 0 Oct 24 12:00 example.txt
```

### Explanation:
1. **Before the `chown` command:**  
   The file `example.txt` is owned by `user1` and belongs to the group `group1`.

2. **Command: `sudo chown user2:group2 example.txt`**  
   This changes the ownership of the file to `user2` and assigns the group `group2`.

3. **After the `chown` command:**  
   Now, `user2` is the owner and `group2` is the group associated with `example.txt`.

---

> **Note**: The `sudo` command is required for non-root users to modify file ownership.
