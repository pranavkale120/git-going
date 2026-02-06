# Lesson 3: Installing Git

Git requires a client to be installed on your computer.
## 🪟 Windows

1. Download Git from [git-scm.com/download/win](https://git-scm.com/download/win)
2. Run the installer
3. **Important settings during installation**:
   - Choose your default editor (VS Code is a good choice if you have it)
   - "Adjusting your PATH environment" - select "Git from the command line and
     also from 3rd-party software"
   - "Choosing HTTPS transport backend" - select "Use the OpenSSL library"
   - "Configuring line ending conversions" - select "Checkout Windows-style,
     commit Unix-style line endings"
   - Accept defaults for other options
4. Open **Git Bash** (from Start menu, or right-click in a folder and select
   "Git Bash Here") and verify:
   ```bash
   git --version
   ```

Git Bash is now your terminal for all Git work. It gives you the same Unix-like
commands (ls, cd, pwd, etc.) that Mac and Linux users have.

**Note:** Don't worry if you're unfamiliar with terminals - the next lesson will explain why we use them and how to work with them effectively.

## 🍎 Mac

Open the Terminal app and type one of the following:

**Option 1: Xcode Command Line Tools** (easiest)
```bash
xcode-select --install
```
Click "Install" when prompted.

**Option 2: Homebrew** (if you have it)
```bash
brew install git
```

**Option 3: Direct download**
Download from [git-scm.com/download/mac](https://git-scm.com/download/mac)

Verify installation:
```bash
git --version
```

## 🐧 Linux

Git is likely already installed. If not:

**Debian/Ubuntu**:
```bash
sudo apt update
sudo apt install git
```

**Fedora**:
```bash
sudo dnf install git
```

**Arch**:
```bash
sudo pacman -S git
```

Verify:
```bash
git --version
```

## ⚙️ Configure Git (all platforms)

After installing Git, set up your identity. Open your terminal (Git Bash on
Windows, Terminal on Mac, or your terminal emulator on Linux) and run the
following commands. Git uses this information to label your commits:

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

Use the same email address you used for GitHub so your commits are properly
linked to your account.

Optional but recommended settings:

```bash
# Set your default branch name to "main"
git config --global init.defaultBranch main

# Set VS Code as your default editor (if you use VS Code)
# If you don't have an editor, don't worry about this now,
# We'll install it later.
git config --global core.editor "code --wait"

# Enable colorful output
git config --global color.ui auto

# Store credentials to avoid repeated password prompts
# Note: credentials are stored in plain text in ~/.git-credentials
git config --global credential.helper store
```

View your configuration:
```bash
git config --list
```

**Assignment**: Paste the output of the following into a GitHub comment for this lesson's issue:
- `git --version`
- `git config --list`

If anything is confusing, unclear, or could be improved, please leave a comment and we'll get back to you.

---

© 2026 BEC Systems. All rights reserved.
