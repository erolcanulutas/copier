# Copier - Project File Dumper (Tkinter)

A lightweight Tkinter-based desktop tool that lets you **browse your project as a file tree**, select specific source files, and **dump their contents into a single text output** for easy copying, sharing, or analysis.

This tool is especially useful when:
- Preparing context for ChatGPT or other LLMs
- Sharing selected parts of a codebase
- Reviewing or exporting multiple files at once

---

## ✨ Features

- 📁 **File Tree View**
  - Displays the current project folder and all subfolders
  - Clear parent–child hierarchy (real file tree)
  - Folders and files are visually distinct

- ☑️ **Checkbox-Based File Selection**
  - Each file has an individual checkbox
  - Selection state is preserved even after refreshing the tree
  - Newly discovered files start unchecked (by design)

- 🔄 **Smart Refresh Options**
  - **Refresh Tree**: Rebuilds the file tree without losing selections
  - **Refresh Text**: Updates the output based on current selections
  - **Refresh & Copy All**: One-click refresh + clipboard copy

- 📋 **Bulk Actions**
  - **Check All**: Select all valid files at once
  - **Uncheck All**: Clear all selections instantly
  - **Copy All**: Copy the full dumped output to clipboard

- 🧠 **Safe & Practical**
  - Skips the running script automatically
  - Gracefully handles deleted or unreadable files
  - No destructive operations (read-only)

---

## 📂 Supported File Types

By default, the following extensions are included:

- `.py`
- `.json`
- `.ino`

You can easily extend this list in the code:
```python
FILE_EXTENSIONS = ('.py', '.json', '.ino')
