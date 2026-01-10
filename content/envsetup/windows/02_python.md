---
title: Install Python
label: envsetup-windows-python
---

Now you will install Python. Python is the programming language we will use this semester for all our data analytics operations.

Windows does not come with Python installed by default, so you'll need to download and install it from the official Python website.

## Install Python

1. **Download Python from python.org**
   * Open your web browser and navigate to [https://www.python.org/downloads/](https://www.python.org/downloads/)
   * Click the yellow **Download Python 3.x.x** button to download the latest stable version
   * Save the installer file (it will be named something like `python-3.x.x-amd64.exe`)

2. **Run the Python Installer**
   * Locate the downloaded installer file in your **Downloads** folder and double-click it to run it
   * **⚠️ IMPORTANT:** On the first screen, check the box that says **Add python.exe to PATH** at the bottom of the window
      * This is critical! Without this, Python won't work correctly from the command line
   * Click **Install Now** (recommended) or **Customize installation** if you want to change the installation location
   * Wait for the installation to complete
   * Click **Close** when the installation is finished

3. **Verify Installation**
   * Open **PowerShell** by pressing {kbd}`Win` + {kbd}`X` and selecting **Windows PowerShell** (or **Terminal** on Windows 11)
   * Copy the following command:
     ```
     python --version
     ```
   * Paste it into PowerShell and press {kbd}`Enter`
   * The output should show something like `Python 3.12.x` (the exact version number may vary)
   * Copy the following command to verify the Python path:
     ```
     where python
     ```
   * Paste it into PowerShell and press {kbd}`Enter`
   * The output should show a path similar to `C:\Users\YourUsername\AppData\Local\Programs\Python\Python3xx\python.exe`

   :::{note}
   If the `python --version` command doesn't work, you may need to close and reopen PowerShell, or restart your computer. If it still doesn't work, you may need to manually add Python to your PATH environment variable. Ask your favorite AI tool for support with this specific error message, or reach out to the instructor or TA.
   :::
