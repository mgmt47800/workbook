---
title: Create an External Environments Directory
label: envsetup-windows-eed
---

You will create a Python virtual environment to use in this course. This environment will store all the Python packages that are installed throughout the course so that you can easily uninstall them all later if needed.

Because Python packages contain 1000s of small files, it's best to create this virtual environment **outside** of any directories that are synced (via OneDrive, for example). We'll create it at the root of your `C:` drive.

1. **Create the Folder via File Explorer**
   * Open **File Explorer** by pressing {kbd}`Win` + {kbd}`E`
   * Navigate to **This PC** > **Local Disk (C:)**
   * Right-click in the empty space and select **New** > **Folder**
   * Name the folder `conda_envs`

2. **Exclude Folder from Cloud Sync (OneDrive/Dropbox)**
   * Locate your new `C:\conda_envs` folder
   * If you see sync icons (blue clouds or green checks), right-click the folder
   * Select **Always keep on this device** to ensure the files remain local and do not waste bandwidth or trigger sync conflicts
   * If using Dropbox or Google Drive, enter the application settings to "uncheck" or "ignore" this specific directory

3. **Configure Folder Permissions**
   * Right-click the `conda_envs` folder and select **Properties**
   * Click on the **Security** tab, then click the {kbd}`Edit...` button
   * Select **Users** from the "Group or user names" list
   * In the "Permissions for Users" section, check the box for **Full control** under the **Allow** column
   * Click {kbd}`Apply`, then {kbd}`OK` on both windows to save the changes