---
title: Install Conda & Python
label: envsetup-windows-conda-python
---

Now you'll install **Miniconda** and **Python** on your computer.

**Miniconda** is a lightweight, industry-standard distribution that provides the essential engine for Python data analytics, allowing you to create isolated environments and manage the specific libraries required for complex financial modeling and data-driven decision-making.

:::{note}
**Miniconda** is a lightweight version of a software named **Anaconda**. You'll see it referred to as "Miniconda", "Anaconda", and just "Conda" throughout the course. For our purposes, they all refer to the package manager on your computer.
:::

**Python** is the programming language that we will use to perform our analytics operations in this course.

## Install Python

1. **Install Python via Miniconda**
   * Download the **Miniconda Windows 64-bit installer** from the [official Anaconda site](https://docs.anaconda.com/miniconda/)
   * Open the downloaded `.exe` file to start the installation wizard
   * Click {kbd}`Next` and then {kbd}`I Agree` after reviewing the license terms
   * Select **Just Me (recommended)** and click {kbd}`Next`
   * Keep the default installation destination (usually `C:\Users\Username\miniconda3`)
   * Under **Advanced Installation Options**, ensure **Register Miniconda3 as my default Python 3.x** is checked
   * Click {kbd}`Install` and wait for the process to finish
   * Click {kbd}`Next` and then {kbd}`Finish` to close the installer

2. **Verify the Python Installation**
   * Open the **Start Menu** and type "Anaconda Prompt"
   * Click on **Anaconda Prompt (miniconda3)** to open the terminal
   * Type `python --version` and press {kbd}`Enter`
   * Confirm the output displays a version number (e.g., `Python 3.12.x`)
   * Type `where python` and press {kbd}`Enter` to confirm the path points to your Miniconda folder