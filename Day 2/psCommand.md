## Multiple Choice Question

**Question:**  
Which Unix command is used to display the status of running processes?

- A) `ps`
- B) `top`
- C) `kill`
- D) `df`

**Correct Answer:**  
**A) ps**

---

### Explanation of Options:

#### A) `ps` (Correct Answer)
The `ps` command is used to display information about the current processes running on the system. It provides a snapshot of the processes with details such as the process ID (PID), terminal (TTY), CPU time, and the command that initiated the process.

- **Example:**
  ```bash
  ps
  ```
  This command will show a list of the processes running in the current terminal session.

  - **Output:**
    ```bash
    PID TTY          TIME CMD
    2244 pts/0    00:00:00 bash
    2255 pts/0    00:00:00 ps
    ```

#### B) `top`
The `top` command also displays the status of running processes, but it is more dynamic, providing a real-time view of system resource usage like CPU and memory. It continuously updates until stopped by the user.

- **Example:**
  ```bash
  top
  ```
  This command provides a continuously updating list of processes, showing system resource usage like memory and CPU percentage.

  - **Output:**
    ```bash
    top - 09:34:32 up 4:56,  3 users,  load average: 0.03, 0.08, 0.09
    Tasks: 126 total,   1 running, 125 sleeping,   0 stopped,   0 zombie
    %Cpu(s):  3.1 us,  0.6 sy,  0.0 ni, 96.1 id,  0.0 wa,  0.0 hi,  0.1 si,  0.0 st
    ```

#### C) `kill`
The `kill` command is used to terminate processes by sending a signal to the process. It is not used to display process status but is used for process control (such as terminating them).

- **Example:**
  ```bash
  kill 1234
  ```
  This sends a signal to terminate the process with PID 1234.

#### D) `df`
The `df` command is used to display disk space usage, not process status. It shows information about file system disk space usage.

- **Example:**
  ```bash
  df -h
  ```
  This command displays disk usage in human-readable format.

  - **Output:**
    ```bash
    Filesystem      Size  Used Avail Use% Mounted on
    /dev/sda1        50G   15G   33G  31% /
    ```
```
