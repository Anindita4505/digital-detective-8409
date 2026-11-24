# Mission 2 — Become Comfortable with the Terminal

## 1. Mission Title

Become Comfortable with the Terminal

## 2. Task / Objective

The objective of this mission was to practise basic Terminal operations, safely create and manage files, understand command flags and pipes, and learn how package managers work.

## 3. Work Completed

### Task 2.1 — Basic Terminal Operations

The following commands were executed inside the Digital Detective repository.

| Operation                 | Command                        | What it does / What I observed                                |
| ------------------------- | ------------------------------ | ------------------------------------------------------------- |
| Display current location  | `pwd`                          | Displays the full path of the current working directory.      |
| List files and folders    | `ls`                           | Displays the contents of the current directory.               |
| Detailed listing          | `ls -l`                        | Displays permissions, owner, file size and modification date. |
| Move to parent directory  | `cd ..`                        | Moves one directory level up.                                 |
| Return to repository      | `cd digital-detective-8409`    | Changes the current directory back to the repository.         |
| Create a practice folder  | `mkdir terminal-practice`      | Creates a new directory named terminal-practice.              |
| Enter the practice folder | `cd terminal-practice`         | Changes the current working directory to terminal-practice.   |
| Create an empty file      | `touch original.txt`           | Creates an empty text file.                                   |
| Copy a file               | `cp original.txt copy.txt`     | Creates a separate copy of the original file.                 |
| Rename a file             | `mv copy.txt renamed-copy.txt` | Renames the copied file.                                      |
| List practice files       | `ls`                           | Displayed original.txt and renamed-copy.txt.                  |
| Display file contents     | `cat original.txt`             | Initially displayed no text because the file was empty.       |

### Task 2.2 — Safe File Management

Created a folder named `terminal-practice` inside the repository and performed all file-management exercises inside it.

Commands used:

```bash
mkdir terminal-practice
cd terminal-practice
pwd

touch original.txt
echo "This is my original practice file." > original.txt
echo "This is the second line." >> original.txt
cat original.txt

cp original.txt backup.txt
mv backup.txt original-backup.txt
ls
```

The `cat original.txt` command displayed:

```text
This is my original practice file.
This is the second line.
```

The final directory listing showed:

- `original.txt`
- `original-backup.txt`
- `renamed-copy.txt`

**Answers to the questions:**

1. **Replacing vs appending:** The `>` operator replaces the existing contents of a file, whereas `>>` adds new content at the end without removing the existing contents.
2. **Copying vs moving:** `cp` creates a separate copy while keeping the original file. `mv` moves a file to another location or renames it.
3. **Purpose of `pwd`:** It displays the current working directory and helps identify where commands are being executed.
4. **Purpose of `ls`:** It lists files and directories in the current location, helping users understand the contents of a directory.

### Task 2.3 — Flags and Pipes

Commands used:

```bash
ls
ls -lhA
ls -l | head -n 5
```

**Observations:**

- `ls` displayed the regular files and directories in the repository.
- `ls -lhA` displayed detailed information, including hidden files such as `.git`, along with human-readable file sizes.
- `ls -l | head -n 5` displayed only the first five lines of the detailed listing.

**Explanation of flags and commands:**

| Flag / Command | Purpose                                      |
| -------------- | -------------------------------------------- |
| `-l`           | Displays a detailed directory listing.       |
| `-h`           | Displays file sizes in human-readable units. |
| `-A`           | Includes hidden files except `.` and `..`.   |
| `head -n 5`    | Displays the first five lines of input.      |

**What is a pipe?**

The pipe symbol `|` sends the output of one command as input to another command.

In `ls -l | head -n 5`, the first command produces a detailed directory listing, and the second command displays only its first five lines.

### Task 2.4 — Package Managers

Checked Homebrew using:

```bash
brew --version
brew list
```

**Observations:**

- Homebrew was already installed on the system.
- The installed version was **Homebrew 7.0.15**.
- `brew list` displayed the installed formulae and casks.
- The cask listing included `copilot-cli`.

**What is a package manager?**

A package manager is a tool that helps users install, update and manage software packages. Homebrew is a package manager for macOS that allows users to manage software through Terminal commands, making software installation and maintenance easier.

No software was installed or uninstalled during this task.

## 4. Commands / Tools Used

The commands and tools used in this mission included:

- `pwd` — displays the current working directory.
- `ls` — lists directory contents.
- `ls -l` — displays detailed file information.
- `ls -lhA` — displays detailed information, hidden files and human-readable sizes.
- `cd ..` — moves to the parent directory.
- `cd` — changes the current working directory.
- `mkdir` — creates directories.
- `touch` — creates empty files.
- `echo` — displays text or sends text to a file.
- `>` — replaces file contents through output redirection.
- `>>` — appends content through output redirection.
- `cp` — copies files.
- `mv` — moves or renames files.
- `cat` — displays file contents.
- `head -n 5` — displays the first five lines.
- `|` — passes output from one command to another.
- `brew --version` — checks the Homebrew version.
- `brew list` — lists installed Homebrew packages.

## 5. My Understanding

Through this mission, I learned how to navigate directories, inspect files, create and manage files, and understand the difference between copying and moving files.

I also understood how redirection operators work, how command flags modify output, and how pipes connect commands. I learned that package managers such as Homebrew help manage software from the Terminal.

## 6. Difficulties Faced

No major difficulties were faced while completing the practical tasks.

## 7. How I Resolved Them

I followed the commands step by step, checked the output after executing them, and verified that the expected files and directory contents were created successfully.

## 8. Evidence / Files

The practical work and screenshots are saved in the following locations:

**Practice files:**

- `terminal-practice/original.txt`
- `terminal-practice/original-backup.txt`
- `terminal-practice/renamed-copy.txt`

**Mission documentation:**

- `mission-02-terminal/README.md`

**Screenshots:**

- `evidence/mission-02-basic-commands.png`
- `evidence/mission-02-file-practice.png`
- `evidence/mission-02-flags-pipes.png`
- `evidence/mission-02-homebrew.png`

The screenshots document the Terminal commands, file-management operations, flags, pipes and Homebrew checks. Personal usernames and full local file paths have been excluded from the documentation.

## 9. Commit Details

- **Branch:** 'main'
- **Commit message:** 'Complete Terminal and file management mission'
- **Status:** 'Successfully committed and pushed to GitHub.'
