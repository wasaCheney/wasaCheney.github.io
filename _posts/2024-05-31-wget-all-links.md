# Get all links (only the address rather than downloading the content) and write to a file
`wget --no-directories --mirror --spider https://utw.me/file/scripts/ 2>&1 | tee log.txt`

# Then check the written file, and delete what unnecessary

# Then downloads one by one
`cat log.txt | shuf | xargs -n10 -P4 wget --continue`
