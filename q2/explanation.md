# Q2 Explanation

- `mkdir -p` created the secure project directory tree in one step without failing if any parent folder already existed.
- `touch` created the empty planning, application, and log files so the workspace had the expected structure.
- `ls -ld` before and after `chmod` showed the permission change from an open directory state to a restricted 750 layout.
- `chmod 640` on the files kept them readable for the owner and prevented write access from others, which is appropriate for project content.
- `umask` returned `0022`, which explains why newly created files start with standard non-executable permissions.
