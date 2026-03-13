# Lesson 5: Setting Up a Text Editor

You'll need a good text editor for editing files. If you don't already have a
favorite text editor, we recommend **Visual Studio Code** (VS Code) - it's free,
powerful, and works great with Git.

## 🚀 Installing VS Code

### Windows

1. Download VS Code from [code.visualstudio.com](https://code.visualstudio.com)
2. Run the installer
3. **Important**: Check these options during installation:
   - "Add to PATH" (allows running `code` from terminal)
   - "Add 'Open with Code' action to Windows Explorer context menu"
4. Restart Git Bash after installation

### Mac

1. Download VS Code from [code.visualstudio.com](https://code.visualstudio.com)
2. Open the downloaded `.zip` file
3. Drag Visual Studio Code to your Applications folder
4. Open VS Code, then press `Cmd+Shift+P` and type "shell command"
5. Select "Install 'code' command in PATH"

### Linux

**Debian/Ubuntu**:

```bash
sudo apt update
sudo apt install code
```

Or download the `.deb` package from
[code.visualstudio.com](https://code.visualstudio.com)

**Fedora**:

```bash
sudo dnf install code
```

**Arch**:

```bash
sudo pacman -S code
```

## ✅ Verify installation

Open your terminal (Git Bash on Windows) and run:

```bash
code --version
```

You should see a version number like `1.85.0` or similar.

## ⚙️ Configure Git to use VS Code

Set VS Code as your default Git editor:

```bash
git config --global core.editor "code --wait"
```

The `--wait` flag tells Git to wait until you close the VS Code tab before
continuing. This is important for commit messages and other Git operations.

## Opening files and folders

From the terminal, you can open files or folders in VS Code:

```bash
# Open a specific file
code README.md

# Open the current folder
code .

# Open a specific folder
code ~/projects/git-going
```

## 💡 Essential VS Code features for Git

VS Code has excellent built-in Git support:

- **Source Control panel** (Ctrl+Shift+G / Cmd+Shift+G): See changed files,
  stage changes, and commit
- **GitLens extension**: Enhanced Git features like blame annotations and
  history
- **Diff viewer**: Click any changed file to see a side-by-side comparison
- **Integrated terminal** (Ctrl+` / Cmd+`): Run Git commands without leaving the
  editor

## Recommended extensions

Click the Extensions icon in the sidebar (or press Ctrl+Shift+X / Cmd+Shift+X)
and install:

- **GitLens**: Supercharges Git capabilities
- **Git Graph**: Visualize your repository's branch structure

**Note**: Markdown preview is built into VS Code - no extension needed! Press
`Ctrl+Shift+V` (or `Cmd+Shift+V` on Mac) to preview any `.md` file.

## Alternative editors

If you prefer a different editor, here are some options:

- **Vim/Neovim**: Terminal-based, powerful but steep learning curve
- **Helix**: Similar to Vim, but commands are more intuitive

To set a different editor for Git:

```bash
# Vim
git config --global core.editor "vim"

# Helix
git config --global core.editor "hx"
```

**Assignment**: Install VS Code (or your preferred editor), configure Git to use
it, and paste the output of the following into a GitHub comment for this lesson's
issue:

- `code --version` (or equivalent for your editor)
- `git config --global core.editor`

If anything is confusing, unclear, or could be improved, please leave a comment and we'll get back to you.

---

© 2026 BEC Systems. All rights reserved.
