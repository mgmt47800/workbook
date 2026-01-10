---
title: Install Python
label: envsetup-mac-python
---

Now you will use Homebrew to install Python. Python is the programming language we will use this semester for all our data analytics operations.

While macOS comes with a "system" Python, you should **never** use it for development. It is often outdated and reserved for the operating system's own functions.

## Install Python

1. **Use Homebrew to Install Python**
   * Open **Terminal** by pressing {kbd}`Cmd` + {kbd}`Space` to open Spotlight, then type "Terminal" and press {kbd}`Enter`
   * Copy the following command:
     ```
     brew install python
     ```
   * Paste it into Terminal and press {kbd}`Enter`
   * This will install the latest stable version of Python to your computer

2. **Verify Installation**
   * After Python is installed, copy the following command to check your Python setup:
     ```
     which python3
     ```
   * Paste it into the Terminal and press {kbd}`Enter`
   * The output should show a path similar to `/opt/homebrew/bin/python3`
      * If you see `homebrew` in the path, Python is installed and configured correctly. You may move to the next page
      * If you do not see `homebrew` in the path, proceed to step 3

3. **Update Python Path**
   * 🚨 _This is ONLY necessary if your Python path **does not** include `homebrew`_
   * Copy the following command to associate the "python3" command with the correct Python installation:
     ```
     export PATH="$(brew --prefix python)/libexec/bin:$PATH"
     ```
   * Paste it into the Terminal and press {kbd}`Enter`
   * Copy the following command to restart the shell (which will refresh your connection to Python)
     ```
     source ~/.zshrc
     ```
   * Paste it into the Terminal and press {kbd}`Enter`
   * Copy the following command to check which Python version is now being used:
     ```
     which python3
     ```
   * Paste it into the Terminal and press {kbd}`Enter`
   * The output should show a path similar to `/opt/homebrew/bin/python3`

   :::{note}
   If you still do not see `homebrew` in your Python3 path, ask your favorite AI tool for support. Here's a sample prompt to use:

   _**I am on a Mac running OS {XYZ}. I have installed Python3 with Homebrew but when I use the command `which python3`, it does not seem to associate `python3` with the version installed by Homebrew. The path it returns is `{/path/from/the/terminal}`. What should I do to associate the `python3` command with the Python version installed by Homebrew?**_

   Ensure you fill in your specific operating system and the path returned by the command `which python3` in the prompt.

   You may also reach out to the instructor and TA for support.
   :::