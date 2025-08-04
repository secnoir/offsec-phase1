 Task 7: An Introduction to Shell Operators

## What This Task Covers

This task introduces shell operators — tools that help you combine or manipulate commands and their outputs. They're small symbols with powerful effects.

---

## 1. `>` – Redirect Output (Overwrite)

```bash
echo Hello > file.txt

    Sends the output of echo Hello into file.txt

    If file.txt exists, it will be overwritten

2. >> – Redirect Output (Append)

echo World >> file.txt

    Appends to the end of file.txt instead of overwriting it

3. < – Input Redirection

command < file.txt

    Feeds the contents of file.txt as input to the command

This isn’t used as often in basic tasks, but it’s good to know for scripts and automation.
4. | – Pipe

ls -l | grep ".txt"

    Takes the output from the first command and “pipes” it into the second

    In this case: ls -l output is filtered through grep to show only .txt files

Pipes are super useful for chaining commands together.
5. && – Run Commands Only If Previous One Succeeds

mkdir test && cd test

    cd test will only run if mkdir test was successful

This is great for scripting or automating a flow of commands that rely on each other.
6. ; – Run Commands One After Another

mkdir test; cd test

    Runs both commands regardless of whether the first one succeeds

Summary Table
Operator	Function
>	Redirect and overwrite output
>>	Redirect and append output
<	Feed input from a file
`	`
&&	Run next command only if success
;	Run next command regardless
My Notes

Shell operators are like shortcuts to doing more with less. I already used | with grep, and I can see how && will be useful in scripts or when chaining setup commands. These are small details that make the terminal much more powerful.
