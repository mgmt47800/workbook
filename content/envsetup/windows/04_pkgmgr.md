---
title: Configure the Package Manager
label: envsetup-windows-pkgmgr
---

You've established the directory where your virtual environment will be stored (`C:\conda_envs`) and you've installed Miniconda, which helps you create those environments.

Now you will install and configure **Mamba**, which actually manages the files _within_ those virtual environments. Here's an explanation:

## Conda: The Infrastructure Manager
**Conda** acts as a project manager that creates isolated "containers" (virtual environments) for your work. Instead of installing everything in one messy pile on your machine, Conda ensures each project has its own dedicated space. By configuring it to use `C:\conda_envs`, we are building a dedicated, local warehouse for all your software files—keeping them organized and safe from being accidentally corrupted or slowed down by cloud syncing services like OneDrive.

## Mamba: The High-Speed Engine
**Mamba** is a high-performance version of Conda. When you install a complex library like Pandas, the system must solve a "logic puzzle" to ensure all software parts are compatible. While standard Conda can be slow, Mamba uses a faster C++ engine to download and assemble these parts into your `C:\conda_envs` directory in a fraction of the time.

1. **Configure Conda to Use the External Directory**
   * Open the **Anaconda Prompt (miniconda3)** from your Start Menu
   * Copy the following command:
    ```
    conda config --add envs_dirs C:\conda_envs
    ``` 
   * Paste it into the Anaconda prompt and press {kbd}`Enter`
      * (This instruction sets your external environments directory (EED) as the destination for all future library installations)
   * Copy the following command:
    ```
    conda config --set channel_priority strict
    ``` 
   * Paste it into the Anaconda prompt and press {kbd}`Enter` 
      * (This will help your installations move faster)

2. **Verify Path Priority and Configuration**
   * In the Anaconda prompt, type `conda info` and press {kbd}`Enter`
   * Scroll to the **envs directories** section in the output
   * Confirm that `C:\conda_envs` appears as the first (top) entry in the list
   * Verify the configuration by typing `conda config --show envs_dirs` to see the active paths in a simplified format