# Task 6: Searching for Files

## What This Task Covers

This task introduces different ways to locate files on a Linux system. When you're working on larger machines or CTF challenges, knowing how to find things quickly is key.

---

## 1. `find`

Searches for files and directories in real-time by walking the entire filesystem.

### Basic usage:
```bash
find / -name filename.txt

    / tells it to search from the root directory.

    -name is used to match the filename.

You can also use wildcards:

find /home -name "*.log"

This would find all .log files in /home.
2. locate

Faster than find, but relies on an indexed database.

locate filename.txt

    Searches a pre-built index instead of the live filesystem.

    If it doesn’t return anything, try updating the database:

sudo updatedb

    Note: Some systems may not have locate installed by default.

3. grep (Bonus)

Not for finding files, but useful for searching inside them.

grep "keyword" file.txt

    Finds lines that contain "keyword" in file.txt.

Search through multiple files:

grep -r "keyword" /path/to/folder

When to Use What
Command	Best For
find	Real-time, precise file searches
locate	Fast, broad searches from cache
grep	Searching inside file contents
My Notes

I can already tell find and grep will be a big deal in CTFs. Whether it’s locating hidden flags or analyzing log files, knowing where and how to search saves time. locate is super fast, but it needs to be updated first — good to keep in mind.
