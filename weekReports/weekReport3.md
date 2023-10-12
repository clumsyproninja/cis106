---
name: Andeivi Mejia Taveras
semester: Spring 23
course: cis106
---

# Week Report 3

## Summary of presentations:

### Introduction to Linux
1. What is an operating system?
An operating system is essential for a computer as it offers fundamental software functions, allowing you to utilize the computer's hardware and providing the basic tools for its functionality.

2. Aside from a kernel, what other parts make an operating system?
- Command-Line Shells
  - Primary way of using computers before Graphical Interface was invented. They work by typing commands in a shell. In Linux, the entire system can be controlled through the command line.
- Graphical User Interfaces
  - GUIs depend on icons, menus, and a mouse pointer to facilitate user interactions. Linux, on the other hand utilizes the X Window System in conjunction with desktop environment software suites to provide its GUI.
- Utility and Productivity Programs
  - These tools include web browsers, document processors, and text editors
- Libraries
  - Libraries are sets of programming functions usable in many programs

3. What is a Linux distribution?
A complete Linux system package is called a Linux Distribution. The following elements make up a Linux Distribution:
- A Linux Kernel
- Core Unix Tools
- Supplemental Software
- Startup Scripts
- An installer

4. What is Ubuntu?
Ubuntu is a Linux Distribution, freely available with both community and professional support.

5. Define the following terms: Open Source, Closed Source, Free Software
- Open Source:
  - Software that can be distributed for free or for a fee. Source code is provided with the software.
- Closed Source:
  - Software not distributed with source code. User is restricted from modifying it
- Free Software:
  - Software is distributed with source code. Software can be free of charge or by fee.

1. What are the 4 freedoms defined by the free software foundation?
- Freedom 0: Use software for any purpose
- Freedom 1: Examine and modify source code
- Freedom 2: Redistribute the software
- Freedom 3: Redistribute your modified software

### The basics of Virtualization
1. What is Virtualization?
Virtualization is defined as creating virtual versions of something. It is often used to let multiple Oss run on one physical machine at the same time.

2. List 3 benefits of Virtualization.
- Allows running multiple Oss on one machine without dual booting.
- Reduces costs by decreasing the physical hardware that must be purchased for a network
- Offers ability to save the state of a machine at any time and roll back or forwards

3. What is a Hypervisor?
A hypervisor is a software or hardware in charge of creating, managing, and running virtual machines

4. What is Virtualbox?
Virtualbox is a powerful virtualization product for enterprise as well as home use. It is freely available as Open Source Software.

### Exploring Desktop Environments
1. What is a desktop environment? (3 examples)
A desktop environment (DE) is a collection of software running on top of a computer operating system that provides a common graphical user interface (GUI), sometimes described as a graphical shell. For example:
- GNOME
- Cinnamon
- MATE

2. List 4 common elements of desktop environments.
- Display Manager
- File Manager
- Icons
- Panels 

3. What is Ubuntu's default desktop environments?
GNOME 3. And the official GUI for GNOME 3 is called GNOME Shell.

4. What are the official flavors of Ubuntu?
- Edubuntu
- Kubuntu
- Lubuntu
- Ubuntu Budgie
- Ubuntu Cinnamon
- Ubuntu Kylin
- Ubuntu MATE
- Ubuntu Studio
- Ubuntu Unity
- Xubuntu

### What is a shell?
1. What is Bash?
Bash is a command processor that runs in a text window where the user types commands that cause actions. It can also read and execute commands from a file called a shell script.

2. How do you access the Linux CLI?
- Terminal Emulator
- Linux Console

3. What is a console terminal?
A virtual console is a terminal session that runs in Linux system memory. Instead of having several terminals connected to the computer, most Linux distributions start five or six virtual consoles so you access them from a single keyboard and monitor.

4. What is a terminal emulator?
A program that allows you to access the Linux CLI. Most of the time you use a terminal emulator if you have a GUI installed.

5. Provide 3 examples of Linux commands
- !!, runs last command
- ls, lists directory contents
- sudo, execute commands as the superuser

### Managing Software
1. Which command is used for updating Ubuntu?
sudo apt update

2. Which command is used for installing software? (Provide an example)
sudo apt install firefox

3. Which command is used for removing software? (Provide an example)
sudo apt remove firefox

4. Which command is used for searching for software? (Provide an example)
sudo apt search "web browser"

5. Definition of the following terms:
- Package
  - Archives that contain binaries of software, configuration files, and information about dependencies
- Library
  - Reuseable code that can be used by more than one function or program
- Repository
  - Large collection of software available for download
