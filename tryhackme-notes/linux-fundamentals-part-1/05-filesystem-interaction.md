# Task 5: Interacting With the Filesystem!

## What This Task Covers

Now that you’ve seen how to list directories and check where you are, this task dives deeper into navigating the Linux filesystem, creating and removing files and folders, and organizing data from the terminal.

---

## Key Commands

### 1. `cd` – Change Directory

```bash
cd foldername

    Moves you into the specified folder.

Special variations:

cd ..        # Go back one directory
cd /         # Go to root
cd ~         # Go to your home directory

2. touch – Create a File

touch file.txt

    Creates an empty file.

3. mkdir – Make a Directory

mkdir new_folder

    Creates a new folder.

4. file – Check File Type

file file.txt

    Tells you the type of content inside a file (e.g., text, binary, image, etc.)

5. cp – Copy Files or Folders

cp file1.txt copy.txt

    Copies file1.txt into copy.txt.

Copying folders:

cp -r folder1 folder2

    The -r flag means "recursive" (needed for folders).

6. mv – Move or Rename Files

mv oldname.txt newname.txt

    Renames a file or moves it to a new location.

7. rm – Remove Files

rm file.txt

    Deletes a file.

To delete a folder and everything inside:

rm -r foldername

⚠️ Use this with caution — there’s no “undo” in the terminal.
Bonus: Absolute vs Relative Paths

    Relative path: From your current directory (cd foldername)

    Absolute path: Full path from root (cd /home/user/folder)

My Notes

This was the most hands-on part so far. Moving around the system, creating and deleting files — it finally feels like I’m using Linux for real. These commands are going to be essential later when working with scripts, logs, or CTF challenges.
