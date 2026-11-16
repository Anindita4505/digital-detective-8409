# Mission 3: Understand the Operating System

## 1. Mission Title

Understand the Operating System

## 2. Task / Objective

Explore the operating system, running processes, storage, file paths and permissions. Understand the main responsibilities of an operating system.

## 3. Work Completed

### Task 3.1 — Explore the Operating System

Used Terminal commands to inspect system information.

| Information explored | What it tells you                                | Observation                                                                                               |
| -------------------- | ------------------------------------------------ | --------------------------------------------------------------------------------------------------------- |
| Operating system     | Identifies the operating system and its version. | macOS 26.5                                                                                                |
| Current account      | Identifies the active user account.              | [redacted]                                                                                                |
| Available storage    | Shows total, used and available storage.         | 460 GiB total, 12 GiB used, 369 GiB available, 4% usage                                                   |
| System activity      | Shows running processes and resource usage.      | 659 processes: 2 running and 657 sleeping; CPU was approximately 88.97% idle at the time of the snapshot. |

### Task 3.2 — Understand Processes

A process is a program that is currently running on a computer. It uses system resources such as CPU time and memory.

PID stands for Process ID. It is a numerical identifier assigned to a running process.

Examples of processes:

- Google Chrome — application process.
- `logd` — background system process.

### Task 3.3 — Understand Paths and Permissions

**Absolute path:** A complete path starting from the root directory.

Example: '/Users/[redacted]/digital-detective-8409/basic-practice'

**Relative path:** A path described in relation to the current working directory.

Example: `basic-practice/original.txt`

**File permissions observed:**

The permission listing for `original.txt` was `-rw-r--r--`.

- `r` means read permission.
- `w` means write permission.
- `x` means execute permission.
- `-` means the permission is not granted.

The owner has read and write permissions but does not have execute permission. The group and others have read-only permissions.

### Task 3.4 — Operating System Responsibilities

| Responsibility           | Explanation                                      | Example                                                          |
| ------------------------ | ------------------------------------------------ | ---------------------------------------------------------------- |
| Process management       | Manages running programs and allocates CPU time. | Running Chrome alongside other applications.                     |
| Memory management        | Allocates and manages RAM for programs.          | Giving a browser memory while it runs.                           |
| Device management        | Controls hardware devices through drivers.       | Managing a keyboard, mouse or printer.                           |
| File management          | Organises files and folders and manages storage. | Creating, moving and copying files.                              |
| User interface / shell   | Allows users to interact with the computer.      | Using the macOS desktop or Terminal.                             |
| Security and permissions | Controls access to files and system resources.   | Allowing the owner to edit a file while others can only read it. |

## 4. Commands / Tools Used

- `sw_vers` — displays macOS version information.
- `whoami` — displays the current account name.
- `df -h /` — displays filesystem storage information.
- `top -l 1 -n 5` — displays a snapshot of system activity.
- `ps -axo pid,comm | head -n 15` — displays process IDs and command names.
- `cd` — changes the current directory.
- `pwd` — displays the current working directory.
- `ls -l` — displays detailed file information, including permissions.

## 5. My Understanding

I learned that the operating system manages processes, memory, hardware devices, files and security. I also learned how to inspect running processes, understand PIDs, navigate using paths and identify file permissions.

## 6. Difficulties Faced

Understanding the permission symbols and distinguishing between absolute and relative paths required attention.

## 7. How I Resolved Them

I used `pwd` to observe directory locations and `ls -l` to inspect file permissions. I also reviewed the meaning of each permission symbol.

## 8. Evidence / Files

- Terminal observations recorded in this README.
- File permission output for `basic-practice/original.txt`.
- Operating system and process information recorded above.

## 9. Commit Details

- Commit message: `Complete operating system mission`
- Commit status: To be committed after completing all Mission 3 tasks and reviewing the files.
