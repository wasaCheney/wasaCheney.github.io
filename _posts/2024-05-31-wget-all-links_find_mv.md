# Get all links (only the address rather than downloading the content) and write to a file
`wget --no-directories --mirror --spider https://utw.me/file/scripts/ 2>&1 | tee log.txt`

# Then check the written file, and delete what unnecessary

# Then downloads one by one
`cat log.txt | shuf | xargs -n10 -P4 wget --continue`

================
# Find required files and mv to another dir
`find ~/Linux/Old -maxdepth 1 -mindepth 1 -not -name Tux.png -print0 | xargs -0 mv -t ~/Linux/New`
- `-maxdepth 1` makes it not search recursively
- If you only care about files, you can say `-type f`
- `-mindepth 1` makes it not include the ~/Linux/Old path itself into the result
