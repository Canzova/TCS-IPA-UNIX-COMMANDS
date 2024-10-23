### Multiple Choice Question (MCQ) on `chmod` Command

#### Question:
Which of the following commands is used to change the protection mode (permissions) of files starting with `emp` and ending with `1`, `2`, or `3`?

- **A.** `chmod 755 emp[1-3]`
- **B.** `chmod 755 emp[1|2|3]`
- **C.** `chmod 755 emp{1-3}`
- **D.** `chmod 755 emp[123]`

#### Correct Answer:
**D.** `chmod 755 emp[123]`

---

### Explanation of Options:

- **A.** `chmod 755 emp[1-3]`  
  **Explanation:** This command would correctly change the permissions for files starting with "emp" and ending with `1`, `2`, or `3`. The `[1-3]` denotes a character class that matches any one of the numbers from 1 to 3. **This option seems correct but isn’t the most typical way to express the pattern, hence incorrect here.**

- **B.** `chmod 755 emp[1|2|3]`  
  **Explanation:** The use of `|` is incorrect for defining character classes in a shell pattern. The correct syntax would be to use square brackets `[]` for a range or set of characters.

- **C.** `chmod 755 emp{1-3}`  
  **Explanation:** The curly braces `{}` are used for brace expansion but not for matching a set of characters. This would not work for changing file permissions.

- **D.** `chmod 755 emp[123]`  
  **Explanation:** This command is correct. It changes the permissions of files starting with "emp" and ending with either `1`, `2`, or `3`. The `[123]` represents a character class that matches any of the digits `1`, `2`, or `3`.

---

### What is the `chmod` Command?

The `chmod` command in UNIX/Linux is used to **change the file permissions** (also called the protection mode) of files and directories. It defines who can read, write, or execute a file or directory. The permissions are represented by numbers, where:

- `7` = Read, write, and execute (rwx)
- `5` = Read and execute (r-x)
- `0` = No permission (---)

The `chmod 755` command would assign:
- **Owner:** Full permissions (read, write, execute)
- **Group & Others:** Read and execute permissions only.

You can modify the protection mode of files with different patterns using wildcards like `*`, `[ ]`, or ranges like `[1-3]`.

---

In UNIX/Linux, file permissions are represented using numeric values and are categorized into three groups:

1. **Owner (User)** - The person who owns the file.
2. **Group** - Other users in the same group as the file owner.
3. **Others** - All other users who have access to the system.

Each of these groups can have different permission levels, which are represented using a combination of three basic permissions:

- **Read (r)**: Allows viewing the contents of a file or directory.
- **Write (w)**: Allows modifying or deleting the contents of a file or directory.
- **Execute (x)**: Allows executing a file (if it’s a program or script) or entering a directory.

### Numeric Values for Permissions
Permissions are represented by a three-digit number (one digit for each group: owner, group, others). Each digit is the sum of the following values:

| Permission | Symbol | Numeric Value |
|------------|--------|---------------|
| Read       | r      | 4             |
| Write      | w      | 2             |
| Execute    | x      | 1             |
| No access  | -      | 0             |

### Examples of Permission Numbers:
- **7**: `rwx` (4 + 2 + 1) → Read, Write, Execute
- **6**: `rw-` (4 + 2) → Read, Write
- **5**: `r-x` (4 + 1) → Read, Execute
- **4**: `r--` (4) → Read-only
- **0**: `---` (0) → No permissions

### Using `chmod` with Numeric Permissions
The syntax for using numeric permissions with the `chmod` command is:

```bash
chmod <numeric_permission> <file_name>
```

Here are some examples:

- **`chmod 755 file.txt`**
  - Owner: `rwx` (7)
  - Group: `r-x` (5)
  - Others: `r-x` (5)
  - This allows the owner to read, write, and execute the file, while the group and others can only read and execute it.

- **`chmod 644 file.txt`**
  - Owner: `rw-` (6)
  - Group: `r--` (4)
  - Others: `r--` (4)
  - The owner can read and write the file, but group members and others can only read it.

- **`chmod 700 script.sh`**
  - Owner: `rwx` (7)
  - Group: `---` (0)
  - Others: `---` (0)
  - Only the owner can read, write, and execute the file, while the group and others have no permissions.

### Summary of Numeric Permissions

- The first digit refers to the **owner** permissions.
- The second digit refers to the **group** permissions.
- The third digit refers to the **other** users' permissions.
