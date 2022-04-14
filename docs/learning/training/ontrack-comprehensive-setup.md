# Ontrack Comprehensive Setup Guide

## Windows (using WSL2)
### Set up WSL2 
The first step in setting up your development environment will be to set up Windows Subsystem for Linux (WSL) and Ubuntu. WSL allows Linux distributions to run within the Windows OS. Visit this [website](https://docs.microsoft.com/en-us/windows/wsl/install) for more information.

To quickly set up WSL2 with Ubuntu, follow the tutorial on [ubuntu.com](https://ubuntu.com/tutorials/install-ubuntu-on-wsl2-on-windows-10#1-overview), OR (to paraphrase):

1. Run Windows PowerShell as administrator and use the following command:
   ```powershell
   wsl --install -d ubuntu
   ```
   This will set up WSL2 and ubuntu.

2. Restart your computer.

3. Open Ubuntu (search for the app on your computer) and follow the first time setup instructions to create a username and password.

   **NOTE: If you experience errors during this step, it may be because virtualization is disabled in your BIOS. To fix this will be different depending on your computer/CPU.**

4. To make sure you have the latest updates for Ubuntu, use the following commands:
   ```sh
   sudo apt update
   ```
   then
   ```sh
   sudo apt upgrade
   ```

### Download and install Docker Desktop
...wip

### Set up the OnTrack repository (following [CONTRIBUTING.md]())

On github, fork [doubtfire-deploy](), [doubtfire-api](), and [doubtfire-web](https://github.com/thoth-tech/doubtfire-web).
Make sure to fork the THOTH TECH branch.

#### note: Should we still be following the fork workflow?

Open your Ubuntu terminal and create a directory for Doubtfire.
   ```sh
   mkdir Doubtfire
   ```

cd into this directory
   ```sh
   cd Doubtfire
   ```

clone your doubtfire-deploy
   ```sh
   git clone --recurse-submodules https://github.com/YOUR_USERNAME/doubtfire-deploy
   ```

### How to checkout a branch

...wip

### Developing
Once the previous steps have been completed
code

code .
