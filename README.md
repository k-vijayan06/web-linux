# web-linux
This README file provides a comprehensive overview of the **WebOS Grand Enterprise: Platinum Edition**, detailing its architecture, command suite, and advanced simulated features.

***

# 🐧 WebOS Grand Enterprise: Platinum Edition

Welcome to the **Platinum Edition** of WebOS, a high-fidelity, browser-based Linux terminal simulation. This version integrates advanced system administration tools, a persistent virtual filesystem, and dual-mode text editors to provide a near-authentic DevOps and Linux environment.

## 🚀 Key Platinum Features

* **Persistent Virtual Filesystem (VFS):** All files created via `touch`, `mkdir`, or editors, along with Git repositories and command history, are automatically saved to your browser's `localStorage`. Your work remains intact even after a page refresh.
* **Dual-Editor Integration:**
    * **GNU nano:** A user-friendly, modeless editor. Use `Ctrl+X` to save and exit.
    * **vi Editor:** A professional modal editor. Supports **Insert Mode** (`i`), **Command Mode** (`Esc`), and standard save/quit commands (`:w`, `:q`, `:wq`).
* **Advanced Tab Completion:** Boost your productivity with intelligent completion. Press **Tab** while typing to automatically complete filenames or system commands.
* **Sudo & User Management:** Experience Linux security protocols. Use the `sudo` command to escalate privileges from `guest` to `root` to access restricted directories like `/root`. The default administrative password is **`admin`**.
* **Live System Gauges:** The sidebar features real-time dynamic monitors for simulated CPU and RAM usage, providing a visual "Enterprise" server feel.
* **Robust Pipeline Logic:** Supports complex piping (e.g., `cat file | grep text | wc -l`) with internal `stderr` and `stdout` handling to prevent pipeline breaks during command errors.

## 🛠 Command Reference

### System Basics
* `ls`: List directory contents (supports basic path resolution).
* `pwd`: Print the current working directory.
* `whoami`: Display the current active user (guest or root).
* `clear`: Clear the terminal screen.
* `uptime`: Show how long the virtual session has been active.

### File Manipulation
* `cat [file]`: Display file contents.
* `touch [file]`: Create a new empty file.
* `mkdir [dir]`: Create a new directory.
* `rm [file]`: Remove a file from the VFS.
* `nano` / `vi`: Launch the respective text editors.

### Text Processing & Redirection
* `grep [pattern]`: Filter text matching a specific string.
* `wc`: Count lines in a file or piped input.
* `sort` / `uniq`: Alphabetically sort data or filter unique lines.
* `>` (Redirection): Save command output to a file (e.g., `ls > files.txt`).

### Version Control (Git Simulation)
* `git init`: Initialize a new repository.
* `git add [file]`: Stage files for commit.
* `git status`: View staged changes and repository state.

## 📖 Help & Documentation
The system includes a built-in manual for core utilities. Type `man [command]` (e.g., `man sudo` or `man nano`) to view detailed documentation and usage instructions within the terminal.

## ⚠️ Factory Reset
Because this version uses persistent storage, you can perform a "Factory Reset" via the sidebar or by clearing your browser's site data to return the filesystem to its default state.
