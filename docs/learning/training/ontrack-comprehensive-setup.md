#### Windows (using WSL2)

1. Set up Windows Subsystem for Linux (WSL) and the Linux distribution. WSL allows Linux distributions to run on the Windows OS. Visit this [website](https://docs.microsoft.com/en-us/windows/wsl/install) for more information.

Follow the instructions here.
https://ubuntu.com/tutorials/install-ubuntu-on-wsl2-on-windows-10#1-overview

(to paraphrase):
Run Windows PowerShell as administrator:

   ```powershell
   wsl --install -d ubuntu
   ```

This will set up WSL2 and ubuntu.
Restart your computer.

Open Ubuntu (search for the app on your computer) and follow the first time setup instructions to create a username and password.
note: if you experience errors here it is most likely because virtualization is disabled in your BIOS.

to make sure you have the latest updates for Ubuntu, use the following commands:

   ```sh
   sudo apt update
   ```

then

   ```sh
   sudo apt upgrade
   ```

2. Download and install Docker Desktop

...

3. Set up the OnTrack repository (following https://github.com/lachfoy/doubtfire-deploy/blob/main/CONTRIBUTING.md)

On github, fork [doubtfire-deploy](), [doubtfire-api](), and [doubtfire-web]().
Make sure to fork the THOTH TECH branch.

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





