# Q3 Explanation

- `echo` created a sample file so the link behavior could be tested against real file data.
- `ln` created a hard link that shared the same inode as the original file, which means both names pointed to the same content.
- `ln -s` created a symbolic link that stored only the pathname of the original file.
- `ls -li` and `stat` exposed inode numbers, link counts, and file types, which are the key metadata for link analysis.
- After deleting `original.txt`, the hard link still worked because the inode still existed, while the symlink failed because its target path no longer existed.
