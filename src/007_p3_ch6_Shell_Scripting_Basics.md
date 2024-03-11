# Shell Scripting Basics

Shell scripting is a method to automate tasks in UNIX-like operating systems using shell scripts, which are text files containing a series of commands. `bash` (Bourne Again SHell) and `ksh` (Korn SHell) are two popular shells that support scripting, each with its own set of features, though they share many syntax and functionality similarities. Both shells provide programming constructs that allow conditional execution, loops, and functions, making them powerful tools for automation. Here, we'll cover some basics of shell scripting with a focus on similarities and key differences between `bash` and `ksh`.

### Shebang

Both `bash` and `ksh` scripts typically start with a "shebang" line that specifies the interpreter to be used:

```bash
#!/bin/bash
```

```ksh
#!/bin/ksh
```

This line tells the system to execute the script with `bash` or `ksh` respectively.

### Variables

Variables in both shells are assigned without spaces, and their values are accessed using a dollar sign (`$`):

```bash
name="world"
echo "Hello, $name"
```

Both shells support local and environment variables, though their syntax for advanced features like arrays can differ slightly.

### Conditional Statements

Both `bash` and `ksh` support `if-else` statements, though there are differences in how they handle certain test conditions and modern syntax extensions like `[[ ]]` for testing.

```bash
if [ "$name" == "world" ]; then
  echo "Hello, $name"
else
  echo "Unknown"
fi
```

### Loops

Both shells support `for`, `while`, and `until` loops. The syntax is generally the same across both shells:

```bash
for i in 1 2 3; do
  echo "Number $i"
done
```

### Functions

Functions in both shells are defined and used similarly:

```bash
greet() {
  echo "Hello, $1"
}
greet "world"
```
