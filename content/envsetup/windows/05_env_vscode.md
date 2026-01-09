---
title: Integrate Environment & VS Code
label: envsetup-windows-vscode
---

Now you will create your virtual environment and configure your Visual Studio Code installation to use it.

1. **(If not already done) Install Visual Studio Code**
   * Download the **VS Code User Installer for Windows** from the [official VS Code website](https://code.visualstudio.com/)
   * Run the installer and accept the license agreement
   * On the **Select Additional Tasks** screen, ensure **Add "Open with Code" action to Windows Explorer directory context menu** is checked
   * Click {kbd}`Install` and then {kbd}`Finish` to launch the application

2. **Install the Python Extension in VS Code**
   * Open VS Code
   * Click the **Extensions** icon on the left sidebar (or press {kbd}`Ctrl` + {kbd}`Shift` + {kbd}`X`)
   * Search for and install the **Python** extension provided by Microsoft

3. **Create the Analytics Environment**
   * Open the **Anaconda Prompt (miniconda3)** from your Start Menu
   * Copy the following command:
     ```
     mamba create -n analytics_env python=3.11 pandas numpy matplotlib jupyterlab -y
     ```
   * Paste it into the Anaconda prompt and press {kbd}`Enter`
   * Wait for Mamba to solve the environment and download the packages into your `C:\conda_envs` directory

4. **Activate and Verify the Environment**
   * Copy the following command:
     ```
     conda activate analytics_env
     ```
   * Paste it into the Anaconda prompt and press {kbd}`Enter`
   * Confirm that the text in the parentheses at the start of your command prompt has changed from `(base)` to `(analytics_env)`
   * Copy the following command to check the location of your environment:
     ```
     conda info --envs
     ```
   * Paste it into the prompt and press {kbd}`Enter` to verify the path points to `C:\conda_envs\analytics_env`

   5. **Select the Python Interpreter in VS Code**
   * Open **Visual Studio Code**
   * Open your course folder by going to **File** > **Open Folder...** and selecting the `mgmt47800` directory you created on your computer
   * Open the **Command Palette** by pressing {kbd}`Ctrl` + {kbd}`Shift` + {kbd}`P`
   * Type `Python: Select Interpreter` and select it from the list
   * Look for the entry labeled **Python 3.11 (analytics_env)** located at `C:\conda_envs\analytics_env\python.exe`
   * Click this entry to set it as your default for this workspace
   * **Verify:** Create a new file ( {kbd}`Ctrl` + {kbd}`N` ), save it as `test.py`, and look at the bottom right corner of the window to confirm it displays **analytics_env**