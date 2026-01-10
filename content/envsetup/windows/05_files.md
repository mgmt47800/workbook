---
title: Download Files
label: envsetup-windows-files
---

**Almost finished!** Let's install Visual Studio Code – the recommended integrated development environment (IDE) for this course – and download some files we'll use to test the environment.

## Install VS Code

1. **(If not already done) Install Visual Studio Code**
   * Download the **VS Code User Installer for Windows** from the [official VS Code website](https://code.visualstudio.com/)
   * Run the installer and accept the license agreement
   * On the **Select Additional Tasks** screen, ensure **Add "Open with Code" action to Windows Explorer directory context menu** is checked
   * Click {kbd}`Install` and then {kbd}`Finish` to launch the application

2. **Install the Python Extension in VS Code**
   * Open VS Code
   * Click the **Extensions** icon on the left sidebar (or press {kbd}`Ctrl` + {kbd}`Shift` + {kbd}`X`)
   * Search for and install the **Python** extension provided by Microsoft

## Create a Project Directory on Your Computer

3. **Create the Project Directory**
   * Open **File Explorer** by pressing {kbd}`Win` + {kbd}`E`
   * Navigate to your local root directory named `mgmt47800` (likely in `My Documents` or `OneDrive`, wherever you created it)
   * Right-click in the empty space, select **New** > **Folder**, and name it `getting_started`

## Download the Getting Started Files

4. **Download and Move the Getting Started Notebook and Associated Files**
   * Download the [`getting_started.zip`](https://purdue0-my.sharepoint.com/:u:/g/personal/ree_purdue_edu/IQB2T1t5uizDQrN-0gteZKdEAVBnbgCedHtSl3qXCQ7OylA) file linked here
   * Extract the files by right-clicking the `.zip` file and selecting **Extract All...**
   * Locate the extracted folder in your **Downloads** folder
      * You should see the following three files:
         * `getting_started.ipynb`
         * `pyproject.toml`
         * `README.md`
   * **MOVE ALL THREE FILES INTO YOUR** `mgmt47800\getting_started` folder

   Your directory structure should now look like this:
   ```
   My Documents\
   ├── mgmt47800\
   │   ├── getting_started\
   │       └── getting_started.ipynb
   │       └── pyproject.toml
   │       └── README.md
   ```
