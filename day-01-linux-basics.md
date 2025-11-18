1.pwd
Shows the current working directory (your present location in the filesystem).

2.ls -la / ls -lrtha

ls -la — Lists all files (including hidden files) with detailed information (permissions, owner, size, date).

ls -lrtha — Lists files with details, long format, reverse sort, time sort (newest first normally), human-readable sizes, all (include hidden).
(Flags can be combined in any order, e.g. ls -alh.)

3.cd ~ / cd /

cd ~ — Move to your home directory.

cd / — Move to the root directory.

4.mkdir practice week1 / mkdir -p practice/week1

mkdir practice week1 — Create two directories named practice and week1.

mkdir -p practice/week1 — Create the practice directory and the week1 subdirectory inside it; -p creates parent directories as needed and won’t error if they already exist.

5.touch notes.txt
Creates an empty file named notes.txt (or updates its timestamp if it already exists).

6.echo "hello" > hello.txt
Writes hello into hello.txt (creates the file if it doesn't exist). Note: > overwrites; use >> to append.

7.cat hello.txt
Displays the full contents of hello.txt.

8.head -n 5 /etc/passwd
Shows the first 5 lines of /etc/passwd.

9.tail -n 10 /var/log/syslog
Shows the last 10 lines of /var/log/syslog (may require sudo on some systems).

10.man ls
Opens the manual (help) page for the ls command.

11.which bash
Shows the full path to the bash executable (e.g. /bin/bash) — useful to confirm which shell binary is installed.

12.find ~ -type f -size +1M -maxdepth 3
Searches your home directory (~) for files (-type f) larger than 1 MiB (-size +1M), searching up to 3 directory levels deep (-maxdepth 3).