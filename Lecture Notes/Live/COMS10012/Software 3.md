---
Date & Time: 06-10-2026 11:01
Lecturer:
  - Gretchen Hallett
Course Name:
  - COMS10012
Lecture Name: Regular Expressions
---
## Introduction
- Based on FSMs
- Useful for most text based problems
- Wildly integrated in UNIX tools
- POSIX: Basic & Extended RE
- Perl & Perl Compatible Regular Expressions

## Wildcards
| Operator            | Purpose                                         |
| ------------------- | ----------------------------------------------- |
| `'`                 | Matches any single character                    |
| `^`                 | Matches the start of a line                     |
| `$`                 | Matches the end of the line                     |
| brian               | Find anything starts with *brian*               |
| `[nigel]`           | Matches one of any of the characters in *nigel* |
|                     |                                                 |
| `[a-z0-9]`          | Matches any character in range                  |
| `\[\]`              | Exact matches inside (as a standalone thing)    |
| `\?`                | Matches the thing before it once or zero times  |
| `\+`                | Matches the thing that came before it           |
| `\*`                | Matches at least 0 times                        |
| `squ\[ee\]\+`       | Matches exactly even number of 'e'              |
| `squ\[e\{2\}\]\+`   | Matches multiple of 2 of 'e'                    |
| `squ\[e\{2,3\}\]\+` | Matches multiple of 2, 3 of 'e'                 |

## grep
- Search tool for text documents
- From ed editor command `global /regrexp/ print` -> g/re/p

| Flags    | Purpose                       |
| -------- | ----------------------------- |
| -i       | case sensitive                |
| -E or -P | extended or Perl regexp       |
| -o       | only matching string not line |
| -v       | Inverted matching             |
| -R       | Search folder recursively     |

## Sed
- For filtering & Transforming texts

| Command       | Description                           |
| ------------- | ------------------------------------ |
| `a \ text`    | Append `tex                           |
| `i \ text`    | Insert `te                            |
| `s/ABCD/EFG Match `ABCD` and replace with `EFGH` and  |

---
#Incomplete