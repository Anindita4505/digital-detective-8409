# Mission 3 — Understand the Operating System

## 1. Task / Objective

The objective of this mission was to explore the operating system, observe running processes, understand storage, paths and file permissions, and learn about the major responsibilities of an operating system.

## 2. Work Completed

### Task 3.1 — Explore Your Operating System

I used Terminal commands to identify my operating system, check the current account, inspect storage usage and observe system activity.

| Information explored       | What it tells you                                          | My observation                                                                 |
| -------------------------- | ---------------------------------------------------------- | ------------------------------------------------------------------------------ |
| Operating system           | Identifies the operating system and its version.           | macOS 27.2.1, Build 26B131                                                     |
| Current account            | Identifies the currently logged-in account.                | [redacted]                                                                     |
| Available and used storage | Shows filesystem capacity and storage usage.               | 460 GiB total, 13 GiB used, 362 GiB available, 4% capacity used                |
| System activity snapshot   | Shows running processes, CPU usage and memory information. | 753 processes in total, 2 running and 751 sleeping; CPU usage was 85.68% idle. |

### Task 3.2 — Understand Processes

A process is a program that is currently being executed by the operating system. Each process is assigned a Process ID (PID), which uniquely identifies it.

The process list showed system processes such as `launchd` and application processes such as Google Chrome.

- **PID:** A unique numerical identifier assigned to each process.The PID helps the operating system distinguish between different running processes.
- **Application process example:** Google Chrome.
- **Background process example:** `launchd`, which manages the starting and supervision of system services and processes.

### Task 3.3 — Understand Paths and Permissions

I used `pwd` to display the current working directory and `cd ..` to move to the parent directory.

**Absolute path:** A complete path beginning from the root directory.

Example: `/Users/[redacted]/Documents/digital-detective-8409/mission-03-operating-system`

**Relative path:** A path specified in relation to the current working directory.

Example: `mission-03-operating-system` when starting from the repository root.

I used `ls -l terminal-practice/original.txt` to inspect the file permissions.

The permission output was `-rw-r--r--`.

- `rw-`: The owner can read and write but cannot execute the file.
- `r--`: Group members can read the file.
- `r--`: Other users can read the file.

I did not modify any system permissions.

### Task 3.4 — Explain Operating System Responsibilities

| Responsibility           | Explanation                                                       | Simple example                                                   |
| ------------------------ | ----------------------------------------------------------------- | ---------------------------------------------------------------- |
| Process management       | Manages running processes and allocates CPU time.                 | Running Chrome while another application is open.                |
| Memory management        | Allocates and manages RAM for programs.                           | Providing memory to Chrome while it runs.                        |
| Device management        | Controls communication between the computer and hardware devices. | Managing keyboard and printer connections.                       |
| File management          | Organizes, stores and retrieves files and folders.                | Creating, renaming and deleting files.                           |
| User interface / shell   | Allows users to interact with the computer.                       | Using Terminal commands such as `ls` and `pwd`.                  |
| Security and permissions | Controls access to files and system resources.                    | Allowing the owner to edit a file while others can only read it. |

## 3. Commands / Tools Used

| Command / Tool      | Purpose                                                                  |
| ------------------- | ------------------------------------------------------------------------ |
| `sw_vers`           | Displays macOS version information.                                      |
| `whoami`            | Displays the current account username.                                   |
| `df -h /`           | Displays filesystem storage information in human-readable units.         |
| `top -l 1 -n 5`     | Displays a snapshot of system activity.                                  |
| `ps -A -o pid,comm` | Lists process IDs and command names.                                     |
| `head -n 12`        | Displays the first 12 lines of command output.                           |
| `pwd`               | Displays the current working directory.                                  |
| `cd ..`             | Moves to the parent directory.                                           |
| `ls -l`             | Displays detailed file and directory information, including permissions. |

## 4. My Understanding

I learned that the operating system manages the computer's hardware and software resources. It handles running processes, memory, storage, devices, files and user permissions.

I also understood the difference between absolute and relative paths, how to navigate directories using Terminal, and how file permissions determine what different users can do with a file.

## 5. Difficulties Faced

Understanding the detailed output of the `top` command and interpreting the file permission characters were the main difficulties.

## 6. How I Resolved Them

I examined the command outputs and learned what the different fields represented. I understood that the first three permission characters describe the owner's access, followed by the group's and other users' permissions.

## 7. Evidence / Files

The following screenshots are stored in the `evidence/` folder:

- `mission-03-system-info.png`
- `mission-03-processes.png`
- `mission-03-paths-permissions.png`

## 8. Commit Details

**Commit message:** `Document operating system and file management`
**Branch:** `main`
**Status:** 'Successfully committed and pushed to GitHub.'
