# SplashKit

## What is SplashKit?

The SplashKit website is accessible here: [SplashKit - Home](https://SplashKit.io/)

SplashKit is an open-source Software Development Kit (SDK) created with the purpose of reducing the
overhead required for truly technical coding.

SplashKit includes a large library of methods that a user may experiment with and apply. A function
is a piece of code that accomplishes a purpose by calling other lines of code, it's much simpler to
use pre-defined functions rather than creating all the code yourself when creating a game.

Although SplashKit is a large library, capabilities may always be improved or added to expand its
realism and complexity. This enables users to include more sophisticated elements into their
SplashKit projects more easily and quickly.

### Where is it used?

Currently, SplashKit is primarily used within Deakin University, with the intention of growing into
a larger Educational Toolkit.

The students at Deakin University, studying Introduction to Programming have been the most exposed
to this product. They are the ideal consumers of this product – within the first 12 weeks of using
SplashKit in Introduction to Programming, students can code 2D games with unrestricted creativity
and have a grounded knowledge of C++.

### What does this mean for Thoth Tech?

Here at Thoth Tech, our aim is to improve both functionality, experience and support for upon the
current library of the SplashKit SDK. Allowing users to create more realistic gameplay and games. We
also wish to build a solution capable of highlighting the achievements of the SplashKit users to
ensure exposure of the product and capability as an educational tool.

## What are the goals for SplashKit?

This is entirely up to the team’s expertise, interest, and vision. However, the direction previously
discussed includes:

- Fix incompatibility of SplashKit with Python version 3.8.x
- Building upon the menu framework
- Data visualisation
- Audio mixing
- Machine learning
- Creating an Arcade Machine and game database
- Ease the installation process

## Understanding SplashKit

### Getting Started

The following steps will provide the reader with a basic understanding of SplashKit.

1. Become familiar with SplashKit

   - Visit the SplashKit.io website - here you can read documentation and articles about the
     SplashKit functions.
   - Explore the SplashKit Source Code.
   - Read through the User Guides created by previous developers in the Background Docs Folder.

2. Install SplashKit SDK into your machine

   - Watch provided video (“Windows SplashKit Installation – with audio”)

3. How to run the code

   - Watch the provided video (“how_to_test_code”)

4. How to test you code
   - Run this command line in msys2 64bit for installing cmake
     ```shell
     pacman -S git mingw-w64-x86_64-cmake mingw-w64-x86_64-toolchain mingw-w64-x86_64-ninja
     ```
   - Install option 3
   - Enter this command line in your msys2
     ```shell
     git clone --recursive -j2 https://github.com/SplashKit/SplashKit.git
     ```
   - It will copy SplashKit file to your choosen folder.
   - Use the `cd` command to find the find where the `Cmakelist.txt` is.
     ```shell
     cd /c/SplashKit/projects/cmake
     ```
   - Enter this command, generate files
     ```shell
     cmake -G "Ninja"
     ```
   - and then enter this command line
     ```shell
     ninja
     ```

### Installation

SplashKit requires some software to set up:

- MSYS2 Terminal
- Visual Studio Code
- G++ language tools

As SplashKit is aimed at beginners, Visual Studio Code is the optimal choice due to its simplicity
and ease of use.

A written installation guide for all Operating Systems (OS) can be found
[here](https://splashkit.io/articles/installation/)

A video installation guide for Windows OS can be found
[here](https://deakin365.sharepoint.com/:v:/s/ThothTech2/EXWvjZKY61RGjgewzgySCS0BXQVagohU70wRH3hh2cl_0g?e=tgMpiP)

### Source Code

GitHub: [SplashKit](https://github.com/splashkit)

SplashKit comprises of 4 sections:

- SplashKit Manager (SKM)
- SplashKit-Core
- SplashKit.io
- SplashKit translator

**SplashKit Manager** or SKM is the CLI/App tool for installing and managing SplashKit, as well as
creating, building, and running SplashKit projects. SKM is highly editable through including folders
and bash code into the SplashKit directory / GitHub.

**SplashKit Core** is the code for SplashKit, it is what makes up the all-purpose SDK. All direction
to SplashKit comprised of creating or building upon the core code. Each component was referred to as
a module.

**SplashKit.io** is the website, which is referred to throughout this document.

**SplashKit translator** is responsible for the translation of the SplashKit C++ source into another
language.

### SplashKit on your device

SplashKit duplicates a version of the Source Code onto your device. This is accessed here:

```shell
C:\msys64\home\<user>\.SplashKit
```

This is how SplashKit Manager (SKM) can create projects with preconfigured files. For C++ projects,
these can be accessed here:

```shell
C:\msys64\home\<user>\.SplashKit\new\c++\files
```

SplashKit is a library which includes a variety of functionality detailed on the website. Each file
is referred to as a module, which groups the functions by use. The function code and headers of
SplashKit can be accessed here:

```shell
C:\msys64\home\<user>\.SplashKit\source
```

## Product Lifecycle

TBA
