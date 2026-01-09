---
title: Verify Installation & Versions
label: envsetup-windows-verify
---

Finally, you will test your environment setup with a file provided to you.

1. **Create the Project Subdirectory**
   * Open **File Explorer** by pressing {kbd}`Win` + {kbd}`E`
   * Navigate to your local root directory you created earlier named `\mgmt47800`
   * Right-click in the empty space, select **New** > **Folder**, and name it `getting_started`

2. **Download and Move the Verification Notebook**
   * Download the [`verification_test.ipynb.zip`](https://purdue0-my.sharepoint.com/:u:/r/personal/ree_purdue_edu/Documents/Course%20Documentation/MGMT%2047800%20-%20Experiential%20Projects%20in%20Analytics/student_files/getting_started/verification_test.ipynb.zip?csf=1&web=1&e=KgwMDH) file here and extract it from the .zip file
   * Locate the unzipped file in your **Downloads** folder
   * Copy the file and paste it into `\mgmt47800\getting_started`

Your directory structure should now look like this:
```
Documents/
├── mgmt47800/
│   ├── getting_started
│       └── verification_test.ipynb
```

3. **Open the Project in VS Code**
   * Open **Visual Studio Code**
   * Go to **File** > **Open Folder...**
   * Navigate to your LRD (`mgmt47800`) and enter it
   * Select the `getting_started` directory and open it
      * You should now see the `verification_test.ipynb` file in the file explorer in VS Code
   * Double-click `verification_test.ipynb` to open the notebook

4. **Execute and Verify**
   * Look at the top-right corner of the notebook editor; if it says "Select Kernel," click it and choose **Python Environments...** > **analytics_env**
   * Locate the first code cell in the notebook
   * Click the **Run Cell** icon (the "Play" triangle) to the left of the cell or press {kbd}`Shift` + {kbd}`Enter`
   * **Verification:** Ensure the output confirms that Python is executing from `C:\conda_envs\analytics_env` and that the Pandas library loads successfully