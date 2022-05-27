# Developing With WSL2 (Windows) Guide

## What is WSL and why would I want to use it?

In web development, the Windows operating system is notorious for causing issues. That's why it is
recommended that all Windows users who are developing on Thoth Tech web repositories use Windows
Subsystem for Linux. Windows Subsystem for Linux (WSL) allows Linux distributions to run within the
Windows OS. This greatly simplifies development, and it is luckily very easy to set up!

## Step 1: Set up WSL2

To quickly
[set up WSL2 with Ubuntu](https://ubuntu.com/tutorials/install-ubuntu-on-wsl2-on-windows-10#1-overview):

1. Run Windows PowerShell as administrator (search "Powershell" in the windows search bar and
   right-click 'run as administrator') and use the following command:

   ```powershell
   wsl --install -d ubuntu
   ```

   This will set up WSL2 and the Ubuntu distribution.

2. Restart your computer.

3. Open Ubuntu (search "Ubuntu" in the windows search bar) and follow the first time setup
   instructions to create a username and password.

   **NOTE: If you experience errors during this step, it may be because virtualization is disabled
   in your BIOS. To fix this will be different depending on your computer/CPU.**

4. To make sure you have the latest updates for Ubuntu, use the following commands:
   ```shell
   sudo apt update
   ```
   then
   ```shell
   sudo apt upgrade
   ```
   You now have a Linux distribution running within Windows!

## Step 2: If your project requires Docker, it is best to download and install Docker Desktop now (ignore this step if not using Docker)

Docker Desktop is a software that is used to simplify the development of Doubtfire/OnTrack and other
Thoth Tech projects. Docker removes the need to install native tools used within the project.

1. Download Docker Desktop from the
   [Docker website](https://docs.docker.com/desktop/windows/install/).

## Step 3: Create a directory for Thoth Tech development

Open up your Ubuntu WSL2 terminal and create a directory to organise your Thoth Tech projects. In
this case we could create a directory for all Thoth Tech repositories

```shell
mkdir thoth-tech
```

Then, cd into the newly created directory

```shell
cd thoth-tech
```

Now we can clone a Thoth Tech repository in this directory. If we were working on OnTrack, we can
now use `git clone` to download a local version of the repository. Follow the
[OnTrack contributing guide]() for more information.

## Step 4. Developing using Visual Studio Code

Developing in WSL2 is extremely easy using Visual Studio Code. After creating a new branch for your
project (following the [Thoth Tech git contribution guide]()), it is as simple as typing

```shell
code .
```

This will open Visual Studio Code in the directory that you are currently in. If prompted to install
any recommended extensions (for example, "WSL - Remote"), you should do so.

Once VS Code is open, you will have access to the full codebase of the project and be able to make
changes.

Once you are happy with your changes, you can refer again to Thoth Tech git contribution guide for
creating a pull request to merge with the main project.
