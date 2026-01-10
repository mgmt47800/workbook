---
title: Install the Package Manager
label: envsetup-windows-pkgmgr
---

You've installed Python – the programming language used in this course. However, Python has several support packages that _it_ needs to perform all the analytic functions. To help you maintain those, we will use **Poetry**, which is a _Python_ package manager.

1. **Install Poetry Using PowerShell**
   * Open **PowerShell** by pressing {kbd}`Win` + {kbd}`X` and selecting **Windows PowerShell** (or **Terminal** on Windows 11)
   * Copy the following command:
     ```
     (Invoke-WebRequest -Uri https://install.python-poetry.org -UseBasicParsing).Content | python -
     ```
   * Paste it into PowerShell and press {kbd}`Enter`
   * The installer will download and install Poetry
   * When the installation completes, you'll see a message about adding Poetry to your PATH
   * **Close and reopen PowerShell** for the changes to take effect

2. **Verify Installation**
   * Ensure you have opened a _new_ **PowerShell** window
   * Copy the following command to check your Poetry installation:
     ```
     poetry --version
     ```
   * Paste it into PowerShell and press {kbd}`Enter`
   * Confirm the output displays something similar to `Poetry (version 2.2.1)` (any version number of 2.2 or greater is fine!)

   :::{note}
   If the `poetry --version` command doesn't work after reopening PowerShell, you may need to manually add Poetry to your PATH. The installer typically adds Poetry to:
   
   `C:\Users\YourUsername\AppData\Roaming\Python\Scripts`
   
   If you need help adding this to your PATH, ask your favorite AI tool for support, or reach out to the instructor or TA.
   :::
