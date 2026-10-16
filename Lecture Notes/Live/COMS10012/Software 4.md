---
Date & Time: 16-10-2026 11:13
Lecturer:
Course Name:
Lecture Name: Git (1)
---
## Introduction
- Version control program
- Developed by Linus Torvalds in 2005

## Basics
| Command         | Description                                                          |
| --------------- | -------------------------------------------------------------------- |
| `git status`    | Current status of the directory relative to that repository's memory |
| `git init`      | Initialise Git Repo                                                  |
| `git add`       | Add changes                                                          |
| `git add .`     | Add all changes                                                      |
| `git commit`    | Commit changes                                                       |
| `git commit -m` | Commit all changes                                                   |
| `git log`       | Show history of commits                                              |
## Compare & Restore
| Command             | Description                                                                                         |
| ------------------- | --------------------------------------------------------------------------------------------------- |
| `git diff HASH`     | Show difference compared to previous changes                                                        |
| `git restore HASH ` | Restore to most recent version <mark style="background: #FFB86CA6;">(Notated as new changes)</mark> |
| `git checkout HASH` | Return to latest version, but <mark style="background: #FF5582A6;">marked as no changes</mark>      |
|                     |                                                                                                     |

## Git Config
```bash
git config --global user.name "YOURNAME"
git config --global user.email "YOUREMAIL"
```
`.gitignore`: Which file(s) or folders to ignore



---
