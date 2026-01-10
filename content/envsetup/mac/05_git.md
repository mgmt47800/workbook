---
title: Install Git
label: envsetup-mac-git
---

**Git** is version control software that you will use to ensure your work is preserved and, later, able to be shared with teammates.

Git stores your work in a **repository**, which keeps track of the files needed to run the code you create. Those repositories are both _local_ (on your computer) and _remote_ (on a site such as GitHub). We'll work with repositories later.

For now, you simply need to ensure that the Git software is installed on your computer.

## Install Git

1. **Check if Git is Already Installed**
   * Open **Terminal** by pressing {kbd}`Cmd` + {kbd}`Space`, typing "Terminal", and pressing {kbd}`Enter`
   * Copy the following command:
     ```
     git --version
     ```
   * Paste it into Terminal and press {kbd}`Enter`
   * If you see a version number (e.g., `git version 2.x.x`), Git is already installed—skip to step 3
   * If you see a prompt to install Command Line Developer Tools, click {kbd}`Install` and follow the prompts, then skip to step 3
   * If Git is not installed and no prompt appears, continue to step 2

2. **Install Git via Homebrew**
   * 🚨 _ONLY perform this step if Git is **not** installed!_
   * Copy this command:
     ```
     brew install git
     ```
   * Paste it into Terminal and press {kbd}`Enter` to install Git

3. **Configure Git with Your Identity**
   * Copy the following command, replacing `Your Name` with your actual name:
     ```
     git config --global user.name "Your Name"
     ```
   * Paste it into Terminal and press {kbd}`Enter`
   * Copy the following command, replacing `youremail@example.com` with your Purdue email:
     ```
     git config --global user.email "youremail@example.com"
     ```
   * Paste it into Terminal and press {kbd}`Enter`

4. **Set VS Code as Git's Default Editor**
   * Copy the following command:
     ```
     git config --global core.editor "code --wait"
     ```
   * Paste it into Terminal and press {kbd}`Enter`

5. **Verify the Git Installation**
   * In Terminal, copy and run this command:
     ```
     git --version
     ```
   * Confirm the output displays a version number (e.g., `git version 2.x.x`)
   * Copy and run this command to verify your configuration:
     ```
     git config --list
     ```
   * Confirm you see your name and email in the output
