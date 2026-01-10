---
title: Create and Test Your Virtual Environment
label: envsetup-mac-env-test
---

Now it's time to bring it all together! You will use Visual Studio Code to create a virtual environment and run a Jupyter Notebook containing Python code.

:::{tip}
When using Python on your local computer, you should **always** create and use a virtual environment. This is important for a number of reasons:

1. The virtual environment settings can be shared so that you can easily recreate the environment on another computer OR share the configuration with a teammate so that you are working with exactly the same tools and versions
2. The virtual environment is isolated from other projects, in case you need to work on multiple projects with different settings for each
3. The virtual environment is isolated from the rest of the files on your computer so it's easy to clean up and remove files when they are no longer necessary
:::

## About the Files
In the previous step, you downloaded and stored three files on your computer.

- `getting_started.ipynb` is a **Jupyter Notebook** file that contains Python code. You will do _most_ of the work in this course in Jupyter notebooks, which we will discuss in class
- `pyproject.toml` is a **Poetry configuration file**. Think of this as the "recipe and instructions" to create your virtual environment
- `README.md` is an information file written in Markdown that describes the contents of the other files in the directory and provides instructions and references to others who are working on the project with you. If you are familiar with repositories on GitHub, the README file supplies the content for the "home page" of the repository

## Create a Virtual Environment for Python

1. **Open the Project Subdirectory in VS Code**
   * Open **Visual Studio Code**
   * Go to **File** > **Open Folder...**
   * Navigate to your LRD (`mgmt47800`) and enter it
   * Double-click the `getting_started` directory and click the "Open" button
      * You should now see the three files (`getting_started.ipynb`, `pyproject.toml`, and `README.md`) in the file explorer in VS Code
   * Double-click `getting_started.ipynb` to open the notebook for editing

2. **Open VS Code's Built-In Terminal**
   VS Code has a command line built into its user interface. You will use that to configure your virtual environment.
   * Open the Terminal: Use the keyboard shortcut {kbd}`Ctrl` + **`** (backtick) or navigate to the top menu and select **Terminal** > **New Terminal**.
   * Identify the Shell: Look at the terminal dropdown menu in the top-right area of the terminal panel. It should display **zsh**.
   * Verify via Command: Type the following command into the terminal and press {kbd}`Enter`:
    ```zsh
    echo $SHELL
    ```
   :::{note}
   The output should be `/bin/zsh`. If it is not, click the **down arrow** next to the {kbd}`+` icon in the terminal window and select **zsh**.
   :::

3. **Create the Virtual Environment**
   * In the Terminal _within VS Code_, type the following command and press {kbd}`Enter`:
   ```zsh
   poetry install
   ```
      * This will tell Poetry to "read" the `pyproject.toml` file, create your virtual environment, and install the necessary software to run your code

4. **Execute and Verify**
   * Look at the top-right corner of the notebook editor; if it says "Select Kernel," click it and choose **Python Environments...**
   * Review the list of environments. You should see one that starts with `getting_started...` Select that environment
   * Locate the first code cell in the notebook
   * Click the **Run Cell** icon (the "Play" triangle) to the left of the cell or press {kbd}`Shift` + {kbd}`Enter`
   * The Python output that appears below the cell should say:
   "✅ SUCCESS: Your environment is running locally."
      * If you see the SUCCESS message, 🎉 CONGRATULATIONS! 🎉 You are ready to proceed
      * If you do not see the success message, consult an AI tool or the instructor/TA