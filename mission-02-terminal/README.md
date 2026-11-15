# Mission 2 — Become Comfortable with the Terminal

## 1. Mission Title

Become Comfortable with the Terminal

## 2. Task / Objective

The objective of this mission was to practise basic Terminal operations, safely create and manage files, understand command flags and pipes, and learn how package managers work.

## 3. Work Completed

### Task 2.1 — Basic Terminal Operations

| Operation                    | Command                        | What it does / What I observed                                |
| ---------------------------- | ------------------------------ | ------------------------------------------------------------- |
| Display current location     | 'pwd'                          | Displays the full path of the current working directory.      |
| List files and folders       | 'ls'                           | Displays the contents of the current directory.               |
| Detailed listing             | 'ls -l'                        | Displays permissions, owner, file size and modification date. |
| Move to parent directory     | 'cd ..'                        | Moves one directory level up.                                 |
| Return to previous directory | 'cd -'                         | Returns to the previous working directory.                    |
| Create a folder              | 'mkdir basic-practice'         | Creates a new directory named 'basic-practice'.               |
| Enter the folder             | 'cd basic-practice'            | Changes the current working directory.                        |
| Create an empty file         | 'touch original.txt'           | Creates an empty text file.                                   |
| Copy a file                  | 'cp original.txt copy.txt'     | Creates a separate copy of the original file.                 |
| Rename a file                | 'mv copy.txt renamed-copy.txt' | Renames the copied file.                                      |
| List practice files          | 'ls'                           | Displayed 'original.txt' and 'renamed-copy.txt'.              |
| Display file contents        | 'cat original.txt'             | Displayed no text because the file was empty.                 |

### Task 2.2 — Safe File Management

Created a folder named 'terminal-practice' and worked inside it.

Commands used:

```bash
mkdir terminal-practice
cd terminal-practice
pwd

echo "This is the first line." > notes.txt
echo "This is the second line." >> notes.txt
cat notes.txt

cp notes.txt backup.txt
mv backup.txt notes-backup.txt
ls
```

The 'cat notes.txt' command displayed both lines:

'''text
This is the first line.
This is the second line.
'''

The final directory listing showed:

- 'notes.txt'
- 'notes-backup.txt'

**Answers to the questions:**

1. **Replacing vs appending:** The '>' operator replaces the existing file contents, while '>>' adds new content at the end without removing existing content.
2. **Copying vs moving:** 'cp' creates a separate copy while keeping the original file. 'mv' moves a file or renames it.
3. **Purpose of 'pwd':** It displays the current working directory so that I know where I am working.
4. **Purpose of 'ls':** It displays files and folders in a directory, helping me understand its contents.

### Task 2.3 — Flags and Pipes

Commands used:

'''bash
ls
ls -lhA
ls -l | head -n 5
'''

**Observations:**

- 'ls' displayed the regular files and folders.
- 'ls -lhA' displayed detailed information, including hidden files such as '.DS_Store' and '.git'. File sizes were shown in human-readable units such as KB and bytes.
- 'ls -l | head -n 5' displayed only the first five lines of the detailed listing.

**Explanation of flags:**

| Flag / Command | Purpose                                      |
| -------------- | -------------------------------------------- |
| '-l'           | Displays a detailed listing.                 |
| '-h'           | Displays file sizes in human-readable units. |
| '-A'           | Includes hidden files except '.' and '..'.   |
| 'head -n 5'    | Displays the first five lines of input.      |

**What is a pipe?**

The pipe symbol '|' sends the output of one command as input to another command.

In 'ls -l | head -n 5', the first command produces a detailed directory listing, and the second command displays its first five lines.

### Task 2.4 — Package Managers

Checked Homebrew using:

'''bash
brew --version
brew list
'''

**Observations:**

- Homebrew was already installed.
- The installed version was 'Homebrew 7.0.9'.
- 'brew list' displayed the installed formulae and casks.

**What is a package manager?**

A package manager is a tool that helps users install, update and manage software packages. Homebrew is a package manager for macOS that allows users to manage software through Terminal commands, making software installation and maintenance easier.

No software was installed or uninstalled during this task.

## 4. Commands / Tools Used

The commands and tools used in this mission included:

- 'pwd' — displays the current working directory.
- 'ls' — lists directory contents.
- 'ls -l' — displays detailed file information.
- 'ls -lhA' — displays detailed information, hidden files and human-readable sizes.
- 'cd ..' — moves to the parent directory.
- 'cd -' — returns to the previous directory.
- 'mkdir' — creates directories.
- 'touch' — creates empty files.
- 'echo' — writes text to a file.
- '>' — replaces file contents.
- '>>' — appends text to a file.
- `cp' — copies files.
- `mv' — moves or renames files.
- 'cat' — displays file contents.
- 'head -n 5' — displays the first five lines.
- '|' — passes output between commands.
- 'brew --version' — checks the Homebrew version.
- 'brew list' — lists installed Homebrew packages.

## 5. My Understanding

Through this mission, I learned how to navigate directories, inspect files, create and manage files, and understand the difference between copying and moving files.

I also understood how redirection operators work, how command flags modify output, and how pipes connect commands. I learned that package managers such as Homebrew help manage software from the Terminal.

## 6. Difficulties Faced

No major difficulties were faced while completing the practical tasks.

## 7. How I Resolved Them

I followed the commands step by step, checked the output after executing them, and verified that the expected files and directory contents were created successfully.

## 8. Evidence / Files

The practical work was saved in the following locations:

- 'basic-practice/original.txt'
- 'basic-practice/renamed-copy.txt'
- 'terminal-practice/notes.txt'
- 'terminal-practice/notes-backup.txt'
- 'mission-02-terminal/README.md'

The terminal outputs were checked during the practical exercises. Personal usernames and full local file paths have not been included in this documentation.

## 9. Commit Details

- **Branch:** 'main'
- **Commit message:** 'Complete Terminal and file management mission'
- **Commit frequency:** One dedicated commit for Mission 2, after completing and reviewing all tasks.
- **Push status:** To be verified after committing.
