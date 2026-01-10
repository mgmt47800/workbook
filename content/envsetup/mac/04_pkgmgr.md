---
title: Install the Package Manager
label: envsetup-mac-pkgmgr
---

You've installed Homebrew, which manages software packages for the Mac.

Then you used Homebrew to install Python – the programming language used in this course. However, Python has several support packages that _it_ needs to perform all the analytic functions. To help you maintain those, we will use **Poetry**, which is a _Python_ package manager.

1. **Use Homebrew to Install Poetry**
   * Open **Terminal** by pressing {kbd}`Cmd` + {kbd}`Space` to open Spotlight, then type "Terminal" and press {kbd}`Enter`
   * Copy the following command:
     ```
     brew install poetry
     ```
   * Paste it into Terminal and press {kbd}`Enter`
   * This will install the latest stable version of Poetry on your computer and associate it with Python

2. **Verify Installation**
   * After Poetry is installed, copy the following command to check your setup:
     ```
     poetry --version
     ```
   * Paste it into Terminal and press {kbd}`Enter`
   * Confirm the output displays something similar to `Poetry (version 2.2.1)` (any version number of 2.2 or greater is fine!)