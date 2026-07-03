# Q4 Explanation

- `echo` created a simple log file to use as the target for file-descriptor testing.
- `lsof` listed currently open files, and `lsof -p $$` narrowed that view to the current shell process.
- `exec 3<app.log` opened the file on descriptor 3, which is why `/proc/$$/fd` later showed a matching entry.
- The redirection commands demonstrated the difference between standard output and standard error, and the combined form captured both streams together.
- `ulimit -a` reported the shell resource limits, including the large open-file limit that supports many concurrent descriptors.
