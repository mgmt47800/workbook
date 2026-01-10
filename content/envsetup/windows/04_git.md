---
title: Install Git
label: envsetup-windows-git
---

**Git** is version control software that you will use to ensure your work is preserved and, later, able to be shared with teammates.

Git stores your work in a **repository**, which keeps track of the files needed to run the code you create. Those repositories are both _local_ (on your computer) and _remote_ (on a site such as GitHub). We'll work with repositories later.

For now, you simply need to ensure that the Git software is installed on your computer.

## Install Git

1. **Install Git for Windows**
   * Download the **Git for Windows installer** from the [official Git website](https://git-scm.com/download/win)
   * Run the downloaded `.exe` file to begin the setup
   * Click {kbd}`Next` through the license and installation location (keep the default `C:\Program Files\Git`)
   * On the **Select Components** screen, ensure **Git Bash Here** and **Git GUI Here** are checked, then click {kbd}`Next`
   * When asked to choose the default editor, select **Use Visual Studio Code as Git's default editor** from the dropdown menu
   * Continue clicking {kbd}`Next` to accept the recommended defaults for all remaining screens (including "Adjusting your PATH environment" and "Choosing the SSH executable")
   * Click {kbd}`Install` and, once finished, uncheck "View Release Notes" and click {kbd}`Finish`

2. **Configure Git with Your Identity**
   * Open **PowerShell** by pressing {kbd}`Win` + {kbd}`X` and selecting **Windows PowerShell** (or **Terminal** on Windows 11)
   * Copy the following command, replacing `Your Name` with your actual name:
     ```
     git config --global user.name "Your Name"
     ```
   * Paste it into PowerShell and press {kbd}`Enter`
   * Copy the following command, replacing `youremail@example.com` with your Purdue email:
     ```
     git config --global user.email "youremail@example.com"
     ```
   * Paste it into PowerShell and press {kbd}`Enter`

3. **Verify the Git Installation**
   * In PowerShell, copy and run this command:
     ```
     git --version
     ```
   * Confirm the output displays a version number (e.g., `git version 2.x.x.windows.1`)
   * Copy and run this command to verify your configuration:
     ```
     git config --list
     ```
   * Confirm you see your name and email in the output
