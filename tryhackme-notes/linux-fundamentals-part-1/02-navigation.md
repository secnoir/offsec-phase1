# 02 - Navigating the Linux File System

## Understanding the Linux File System

Linux has a very structured and organized file system. Everything starts from the **root directory**, represented as a single forward slash `/`. From there, all other files and directories branch out like a tree.

Some important directories:

- `/home` – contains personal folders for each user.
- `/etc` – contains configuration files.
- `/bin` – essential binary files (basic system commands).
- `/var` – log files and variable data.
- `/tmp` – temporary files.
- `/root` – the root user’s home directory.

---

## Basic Navigation Commands

Here's a breakdown of the most common commands for moving around:

- `pwd` — **Print Working Directory**  
  Shows the full path of your current directory.
  ```bash
  pwd

    ls — List Directory Contents
    Lists files and folders in the current directory.

ls           # Simple list
ls -l        # Long listing format
ls -a        # Show hidden files

cd — Change Directory
Moves you into a different directory.

    cd /etc           # Go to /etc
    cd ~              # Go to your home directory
    cd ..             # Go up one level
    cd ../../         # Go up two levels

    clear — Clears the terminal screen for better readability.

Useful Shortcuts

    ~ — refers to the current user's home directory.

    . — refers to the current directory.

    .. — refers to the parent directory.

These shortcuts make moving around a lot quicker once you’re comfortable with the structure.
Absolute vs Relative Paths

    Absolute path starts from the root /

        Example: /home/irfan/Desktop

    Relative path starts from your current directory

        Example: ../Documents

Understanding both is crucial — especially in scripts and automation.
My Thoughts

At first, I kept getting confused between cd and where I actually was. But once I understood how everything branches out from /, it made a lot more sense. Using pwd and ls frequently helped me get more comfortable.

This section was all about learning to navigate, and it’s a skill I’ll need constantly in ethical hacking — whether I’m looking through logs, jumping into config files, or exploring a target machine.
