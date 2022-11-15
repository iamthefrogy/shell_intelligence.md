# Collection of my Linux Command List
I often Google and Stakeoverflow silly things. I was tired one day and created this list so I don't have to Google everytime.

Find all types of files using some extension and move them to the parent folder from any recursive folder.
```sh
find . -name '*.yaml' -type f -exec mv {} . \;
```

Find a specific text in any file within the recursive folder and output the file name with the proper location.
```sh
grep -iRl "severity: info"
```

Remove only folders from the working directory but untouched any files.
```sh
rm -r */
```

Remove all files containing specific text within folder.
```sh
grep -lrIZ "severity: medium" | xargs -0 rm -f --
```

Display file content with line numbers.
```sh
cat -n script.sh
```
