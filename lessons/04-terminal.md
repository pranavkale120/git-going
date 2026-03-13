# Lesson 4: We're going to use the terminal to start and here's why

## 💡 Why not start with a GUI?

There are many graphical Git clients available: GitHub Desktop, SourceTree,
GitKraken, LazyGit, and others. They're visually appealing and seem easier at first. So
why am I asking you to use the terminal?

**Understanding over convenience**: GUI tools hide what's actually happening.
When something goes wrong (and it will), you won't know how to fix it. The
terminal shows you exactly what Git is doing.

**Universal knowledge**: Terminal commands work the same everywhere. GUI tools
vary, but `git status` is `git status` whether you're on Windows, Mac, Linux, or
a server.

**Power and flexibility**: The terminal gives you access to Git's full
capabilities. GUIs typically only expose common operations.

**Professional requirement**: Most development environments, servers, and CI/CD
systems require command-line Git knowledge.

**It's not magic**: Many people are intimidated by the terminal. It's not magic. Like anything else, with a little bit of effort, you can learn enough to do the things you need to do. It is much easier than the hard things you are doing in your job right now.

Trust me on this one. Start with the terminal, understand the fundamentals, and
then use a GUI later if you want to streamline your workflow. You'll be much
better equipped to handle problems.

## 🛠️ Terminal options

Below are terminal options for various platforms.
### Windows

We'll use **Git Bash**, which is installed automatically with Git for Windows.
Git Bash provides a Unix-like terminal experience, so the commands you learn
will work the same on Windows, Mac, and Linux. No need to learn Windows-specific
commands - we're all speaking the same language.

You installed Git Bash in the previous lesson. Launch it from the Start menu or
by right-clicking in any folder and selecting "Git Bash Here".

(Note, if the text is too small, you can adjust it by clicking on the icon in
the upper left of the terminal application and selecting
Options->Text->Select...)

### Mac

- **Terminal**: Built-in, found in Applications > Utilities > Terminal
- **iTerm2**: Popular third-party alternative with more features

### Linux

Use your distribution's default terminal emulator (GNOME Terminal, Konsole,
xterm, etc.).

### Advanced terminals

There are more cutting edge terminal options such as the following which give you slighter faster performance.

- [Alacritty](https://alacritty.org/)
- [Ghostty](https://ghostty.org/)

However, don't worry about that for now unless you really want to optimize.

## 📋 Basic terminal commands

Before we dive into Git, let's make sure you're comfortable with basic terminal
navigation:

| Command  | What it does                                   | Example                  |
| -------- | ---------------------------------------------- | ------------------------ |
| `pwd`    | Print Working Directory - shows where you are  | `pwd`                    |
| `ls`     | List files and folders in current directory    | `ls`                     |
| `ls -la` | List all files (including hidden) with details | `ls -la`                 |
| `cd`     | Change Directory - navigate to a folder        | `cd Documents`           |
| `cd ..`  | Go up one directory                            | `cd ..`                  |
| `cd ~`   | Go to your home directory                      | `cd ~`                   |
| `mkdir`  | Make a new directory                           | `mkdir projects`         |
| `cp`     | Copy a file                                    | `cp file.txt backup.txt` |
| `mv`     | Move or rename a file                          | `mv old.txt new.txt`     |
| `cat`    | Display contents of a file                     | `cat README.md`          |
| `rm`     | Remove (delete) a file                         | `rm unwanted.txt`        |
| `touch`  | Create an empty file                           | `touch myfile.txt`       |

**Important tips**:

- Use **Tab** to autocomplete file and folder names
- Use the **Up arrow** to recall previous commands
- File and folder names are **case-sensitive** on Mac and Linux
- Avoid spaces in file names, or wrap them in quotes: `cd "My Documents"`

**Practice exercise**: Open your terminal and try these commands:

```bash
pwd                    # Where am I?
cd ~                   # Go home
mkdir git-practice     # Create a practice folder
cd git-practice        # Enter the folder
pwd                    # Confirm you're there
ls                     # Should be empty
cd ..                  # Go back up
ls                     # See your new folder
```

**Assignment**: Practice navigating your file system using these commands. When
you feel comfortable moving around, add a GitHub comment to this lesson's issue
sharing your experience. Do you feel empowered using a terminal?

Refer back to this lesson in the future if you forget one of the commands.

If anything is confusing, unclear, or could be improved, please leave a comment and we'll get back to you.

---

© 2026 BEC Systems. All rights reserved.
