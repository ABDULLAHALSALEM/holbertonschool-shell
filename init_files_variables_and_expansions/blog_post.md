# What happens when you type `ls *.c`?

When you type `ls *.c` in your shell and hit Enter, here is what happens step by step:

1. The shell reads your command.
2. It identifies `ls` as the command to execute.
3. It sees `*.c`. The `*` is a **wildcard**, which means "match any number of characters."
4. The shell expands `*.c` to all files in the current directory ending with `.c`.
   - Example: if your folder contains `main.c`, `test.c`, and `hello.txt`, the pattern `*.c` becomes `main.c test.c`.
5. The command now looks like this:
   ```bash
   ls main.c test.c
