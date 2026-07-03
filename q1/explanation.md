# Q1 Explanation

- `whoami` confirmed the logged-in Linux user so the report could identify the current account.
- `id` showed the UID, primary GID, and supplementary groups, which is the most complete way to verify account membership.
- `echo "$SHELL"` confirmed the interactive shell is Bash, and `pwd` showed the session started in `/`.
- `ls -ls` displayed the contents of the current directory with permissions and sizes, giving a quick view of the workspace state.
- `curl` to Google verified network access because it returned successfully within the timeout and printed the reachable message.
