---
title: Install Homebrew
label: envsetup-mac-homebrew
---

Your Mac runs a specialized version of Linux as its operating system. You will need to install several software packages in this course, so you'll want to use a tool known as a **package managers** to help keep everything installed in the correct place and up-to-date.

First, you'll install [**Homebrew**](https://brew.sh/), which is a widely-used, open-source utility referred to as "the missing package manager for the MacOS". Homebrew helps you install and update system-wide software packages.

## Install Homebrew

1. **Install Homebrew**
   * Open **Terminal** by pressing {kbd}`Cmd` + {kbd}`Space`, typing "Terminal", and pressing {kbd}`Enter`
   * Copy the following command:
     ```
     /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
     ```
   * Paste it into Terminal and press {kbd}`Enter`
   * Follow the instructions on the screen

   :::{note}
   You will need to have admin rights on your computer to install most of this software. Ensure you are logged in as an admin user whenver you are installing software!
   :::

   * When the installation is complete, **close the Terminal window**

2. **Verify the Installation**
   * Open a new **Terminal** window
   * Type the following command and press {kbd}`Enter`:
     ```
     brew --version
     ```
   * Confirm the output displays something similar to `Homebrew 5.0.9` (any version number of 5 or greater is fine!)