---
title: Install Git
label: envsetup-windows-git
---

1. **Install Git for Windows**
   * Download the **Git for Windows installer** from the [official Git website](https://git-scm.com/download/win)
   * Run the downloaded `.exe` file to begin the setup
   * Click {kbd}`Next` through the license and installation location (keep the default `C:\Program Files\Git`)
   * On the **Select Components** screen, ensure **Git Bash Here** and **Git GUI Here** are checked, then click {kbd}`Next`
   * When asked to choose the default editor, select **Use Visual Studio Code as Git's default editor** from the dropdown menu
   * Continue clicking {kbd}`Next` to accept the recommended defaults for all remaining screens (including "Adjusting your PATH environment" and "Choosing the SSH executable")
   * Click {kbd}`Install` and, once finished, uncheck "View Release Notes" and click {kbd}`Finish`

2. **Verify the Git Installation**
   * Open the **Anaconda Prompt (miniconda3)** or a standard Windows command prompt
   * Copy the following command:
     ```
     git --version
     ```
   * Paste it into the prompt and press {kbd}`Enter`
   * Confirm the output displays a version number (e.g., `git version 2.x.x.windows.1`)