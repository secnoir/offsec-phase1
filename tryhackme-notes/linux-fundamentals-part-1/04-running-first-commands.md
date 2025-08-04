# Task 4: Running Your First Few Commands

## What This Task Covers

This section introduces some of the most essential Linux commands. These are the basics that you’ll use constantly — for navigation, checking your location, clearing your screen, and printing information.

---

## Basic Commands to Know

### 1. `whoami`

```bash
whoami

    Shows the user you're currently logged in as.

    Useful when you need to confirm privileges.

2. pwd (Print Working Directory)

pwd

    Displays your current location in the filesystem.

    Useful when navigating deep folder structures.

3. ls (List)

ls

    Lists the contents of the current directory.

Useful variations:

ls -l    # Long format (permissions, owner, size, etc.)
ls -a    # Shows hidden files (those starting with .)

4. clear

clear

    Clears the terminal screen.

    Doesn’t affect anything — just removes visual clutter.

5. echo

echo Hello

    Prints text to the screen.

    Can also be used to output variables or redirect text into files.

Example:

echo "This is a test" > test.txt

6. man (Manual)

man ls

    Shows the manual (help page) for a command.

    Use q to quit the man page.

If you’re unsure how a command works, try man <command>.
My Notes

At first, these commands felt simple, but I can already tell they’re the building blocks of everything else. ls and pwd are like my eyes in the terminal — without them, I’d be lost. man is also something I’ll definitely use a lot while learning new tools.
