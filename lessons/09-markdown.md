# Lesson 9: Writing with Markdown

Markdown is a simple way to format text using plain characters. It's used
everywhere in the Git world - README files, documentation, issues, pull
requests, and comments. Learning Markdown is essential for working with Git
and GitHub.

## 💡 Why Markdown?

- **Simple**: Just plain text with a few special characters
- **Readable**: The source file is easy to read even without rendering
- **Portable**: Works everywhere - GitHub, VS Code, wikis, blogs
- **Version-friendly**: Since it's plain text, Git can track changes easily

## 📝 Basic Formatting

### Headings

Use `#` symbols for headings. More `#` = smaller heading:

```markdown
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
```

### Text Styles

```markdown
**bold text**
*italic text*
***bold and italic***
~~strikethrough~~
`inline code`
```

Renders as: **bold text**, *italic text*, ***bold and italic***,
~~strikethrough~~, `inline code`

### Links and Images

```markdown
[Link text](https://example.com)
[Link with title](https://example.com "Hover text")

![Alt text for image](image.png)
![Logo](https://example.com/logo.png)
```

### Lists

**Unordered lists** use `-`, `*`, or `+`:

```markdown
- Item one
- Item two
  - Nested item
  - Another nested item
- Item three
```

**Ordered lists** use numbers:

```markdown
1. First step
2. Second step
3. Third step
```

**Task lists** (great for tracking progress):

```markdown
- [x] Completed task
- [ ] Incomplete task
- [ ] Another task to do
```

Renders as:
- [x] Completed task
- [ ] Incomplete task
- [ ] Another task to do

### Code Blocks

For inline code, use single backticks: `git status`

For code blocks, use triple backticks with an optional language:

````markdown
```bash
git add .
git commit -m "My message"
git push
```
````

The language hint enables syntax highlighting:

```bash
git add .
git commit -m "My message"
git push
```

Common language hints: `bash`, `python`, `javascript`, `go`, `json`, `yaml`

### Blockquotes

```markdown
> This is a quote.
> It can span multiple lines.
>
> And have multiple paragraphs.
```

Renders as:

> This is a quote.
> It can span multiple lines.
>
> And have multiple paragraphs.

### Horizontal Rules

Use three or more dashes, asterisks, or underscores:

```markdown
---
```

---

### Tables

```markdown
| Name    | Role       | Status   |
|---------|------------|----------|
| Alice   | Developer  | Active   |
| Bob     | Designer   | Active   |
| Charlie | Manager    | On leave |
```

Renders as:

| Name    | Role       | Status   |
|---------|------------|----------|
| Alice   | Developer  | Active   |
| Bob     | Designer   | Active   |
| Charlie | Manager    | On leave |

Alignment with colons:

```markdown
| Left | Center | Right |
|:-----|:------:|------:|
| 1    | 2      | 3     |
```

## 📚 README Files

Every repository should have a `README.md` file. It's the first thing people
see when they visit your repo. A good README includes:

```markdown
# Project Name

Brief description of what this project does.

## Installation

How to install or set up the project.

## Usage

How to use the project, with examples.

## Contributing

How others can contribute.

## License

What license the project uses.
```

## 🔗 Linking Between Files

Your README is more than just a description - it's the **navigation hub** for your
repository. Create links to other files to help visitors explore your project.

### Relative Links

Use relative paths to link to other files in your repository:

```markdown
[Link text](path/to/file.md)
```

Examples:
```markdown
<!-- Link to a file in the same directory -->
[Notes](notes.md)

<!-- Link to a file in a subdirectory -->
[Documentation](docs/setup.md)

<!-- Link to a file in parent directory -->
[Main README](../README.md)
```

### Best Practice: Create a Navigation Section

Add a section to your README that links to other important files:

```markdown
## 📚 Documentation

- [Notes](notes.md) - My learning notes
- [About Me](about-me.md) - Who I am and why I'm learning Git
- [Resources](resources.md) - Helpful links and references
```

When someone clicks these links on GitHub, they'll navigate directly to the
rendered markdown file. This makes your repository easy to explore!

### Why This Matters

- **Discoverability**: Visitors can find all your content from one place
- **Organization**: Shows the structure of your repository
- **Professionalism**: Demonstrates attention to detail
- **User experience**: Makes it easy for others (and future you!) to navigate

## 👁️ Previewing Markdown

### In VS Code

VS Code has **built-in** markdown preview - no extensions needed!

- Open any `.md` file
- Press `Ctrl+Shift+V` (or `Cmd+Shift+V` on Mac) to open preview
- Or click the preview icon (📖) in the top right corner
- Use `Ctrl+K V` (or `Cmd+K V` on Mac) for side-by-side editing and preview

### On GitHub

GitHub automatically renders Markdown files. You can also:
- Click "Preview" when editing a file
- View any `.md` file and it renders automatically

---

**💡 Tip**: Bookmark this lesson! You can refer back to it anytime you need to
recall Markdown syntax. The formatting examples above cover everything you'll
need for documentation, README files, and GitHub issues.

## 💪 Practice Exercise

### Part 1: Create `about-me.md`

Create a file called `about-me.md` in your `git-going` repository:

```markdown
# About Me

## Why I'm Learning Git

[Write a sentence or two here]

## My Goals

- [ ] Complete the Git Going course
- [ ] Make my first pull request
- [ ] Contribute to an open source project

## Favorite Resources

- [Git Documentation](https://git-scm.com/doc)
- [GitHub Guides](https://guides.github.com/)

---

*Last updated: [today's date]*
```

### Part 2: Add Navigation to README

Update your `README.md` to include links to all your markdown files. Add a new
section like this:

```markdown
## 📚 My Files

- [Notes](notes.md) - Things I'm learning about Git
- [About Me](about-me.md) - My background and goals
```

### Commit Your Changes

```bash
# Stage all changes
git add README.md about-me.md

# Commit
git commit -m "Add about-me page and navigation links"

# Push
git push
```

**Assignment**: Complete both parts, then go to your repository on GitHub and
verify that the links in your README work. Click on each link to make sure it
navigates to the correct file. Add a GitHub comment to this lesson's issue with
the link to your README so I can see your navigation in action!

If anything is confusing, unclear, or could be improved, please leave a comment and we'll get back to you.

---

© 2026 BEC Systems. All rights reserved.
