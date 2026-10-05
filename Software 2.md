---
Date & Time: 29-09-2026 11:05
Lecturer:
  - Gretchen Hallett
Course Name:
  - COMS10012
Lecture Name:
---
## Introduction
```Bash
$ ls -l --human-readbale /
```
Prompt: $
Command: ls
Flags: -l .....
Arguments: / (actually empty)

### Pipes
```Bash
ls | grep .md
```

### Splices
```Bash
$ for f in $(find . -name \*.md);
	do 
		echo "$(f)";
	done

./README.md
./lab/permission.md
```
- Link output of the shell to a new one

```Bash
if test "${x}" -gt 3; then echo 'x > 3'; fi

# Or like this
if [ "$[x]" -gt 3 ]; then echo still true; fi
# Don't forget spaces between square brackets
```

```Shell
x = 5
cat ${x}
```

---
#Incomplete
Add pipe operators table