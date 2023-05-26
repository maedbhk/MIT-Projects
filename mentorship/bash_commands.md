---
title: Useful bash commands
---

[Useful linux commands](https://man7.org/linux/man-pages/dir_section_1.html)

> list all txt files
	* $ ls ~/<folder_name>/*.txt | wc -l

> list all files that are not txt files
	* $ ls ~/<folder_name> | grep ".*[^txt)]$"

> get size of folder
	* $ du -sh ~/<folder_name>

> inspect the first two lines of a text file
	* $ head -n 2 <file_name>.txt


for f in $(ls *.txt); do awk -F'\t' 'NR<=2 {data[NR]=$0} END {split(data[1], cols, "\t"); split(data[2], desc, "\t"); for(i=1; i<=NF; i++) {print cols[i] "\t" desc[i]}}' $f >> output; done && cat output | awk -F'\t' '{print $1 $2}' | sort | uniq >> elements_list.txt && rm output
