---
title: Install Conda & Python
label: envsetup-windows-conda-python
---

Now you'll install **Miniforge** and **Python** on your computer.

## What is Miniforge?

**Miniforge** is a free, open-source distribution that provides Conda package management without any licensing restrictions. It's community-maintained and uses the **conda-forge** repository by default, which is completely free for all users including universities and businesses.

**Miniforge vs. Anaconda/Miniconda:**
- **Anaconda** and **Miniconda** default to Anaconda's commercial package repository, which requires a paid license for organizations with more than 200 employees (like Purdue)
- **Miniforge** uses the community-maintained **conda-forge** repository instead, which has no licensing restrictions
- Miniforge provides the same core functionality as Miniconda (Conda + Python) but is 100% free and open-source for everyone

:::{note}
Throughout this course, when we refer to "Conda" or "Anaconda," we're talking about the **package management system**, not the commercial product. Miniforge gives you full Conda functionality without any licensing concerns.
:::

**Python** is the programming language that we will use to perform our analytics operations in this course.

## Install Python

1. **Install Python via Miniforge**
   * Download the **Miniforge Windows installer** from the [official Miniforge GitHub page](https://github.com/conda-forge/miniforge)
   * Look for **Miniforge3-Windows-x86_64.exe** and download it
   * Open the downloaded `.exe` file to start the installation wizard
   * Click {kbd}`Next` and then {kbd}`I Agree` after reviewing the license terms
   * Select **Just Me (recommended)** and click {kbd}`Next`
   * Keep the default installation destination (usually `C:\Users\Username\miniforge3`)
   * Under **Advanced Installation Options**, ensure **Add Miniforge3 to my PATH environment variable** is checked
   * Also ensure **Register Miniforge3 as my default Python 3.x** is checked
   * Click {kbd}`Install` and wait for the process to finish
   * Click {kbd}`Next` and then {kbd}`Finish` to close the installer

2. **Verify the Python Installation**
   * Open the **Start Menu** and type "Miniforge Prompt"
   * Click on **Miniforge Prompt** to open the terminal
   * Type `python --version` and press {kbd}`Enter`
   * Confirm the output displays a version number (e.g., `Python 3.12.x`)
   * Type `where python` and press {kbd}`Enter` to confirm the path points to your Miniforge folder
