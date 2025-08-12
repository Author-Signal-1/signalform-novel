\# GitHub Git Bash Commands Reference

\## Top 10 Essential Commands for Your Novel Repository



---



\## 1. CHECK STATUS

```bash

git status

```

\*\*What it does:\*\* Shows which files have been changed, added, or need to be committed  

\*\*When to use:\*\* Before making commits to see what changes you have  

\*\*Example output:\*\* Lists modified files, new files, files ready to commit



---



\## 2. COPY FILES TO REPOSITORY

```bash

cp "/c/Users/info/OneDrive/Desktop/temp-chapters/filename.md" "chapters/Target-Name.md"

```

\*\*What it does:\*\* Copies files from your temp folder to the repository  

\*\*When to use:\*\* When you have new chapter content to upload  

\*\*Your pattern:\*\* `signalform\_chapter\_XX.md` → `Chapter-XX.md`



---



\## 3. ADD FILES TO GIT TRACKING

```bash

git add chapters/Chapter-01.md

```

\*\*What it does:\*\* Tells Git to track changes to specific files  

\*\*When to use:\*\* After copying new content, before committing  

\*\*Bulk version:\*\* `git add chapters/` (adds all files in chapters folder)



---



\## 4. COMMIT CHANGES

```bash

git commit -m "Your descriptive message here"

```

\*\*What it does:\*\* Saves your changes with a description  

\*\*When to use:\*\* After adding files, before pushing to GitHub  

\*\*Good messages:\*\* "Add Chapter 8", "Update oracle guide", "Revise Chapter 1-3"



---



\## 5. PUSH TO GITHUB

```bash

git push origin main

```

\*\*What it does:\*\* Uploads your committed changes to GitHub  

\*\*When to use:\*\* After committing, to make changes live online  

\*\*Result:\*\* Your files become visible on github.com



---



\## 6. BULK ADD AND COMMIT

```bash

git add chapters/ \&\& git commit -m "Bulk update: Chapters 1-7" \&\& git push origin main

```

\*\*What it does:\*\* Adds all chapter files, commits them, and pushes in one command  

\*\*When to use:\*\* When updating multiple chapters at once  

\*\*Time saver:\*\* Combines steps 3, 4, and 5



---



\## 7. LIST FILES AND DIRECTORIES

```bash

ls /c/Users/info/OneDrive/Desktop/temp-chapters/\*.md

```

\*\*What it does:\*\* Shows all .md files in your temp folder  

\*\*When to use:\*\* To see what chapter files you have ready to upload  

\*\*Also useful:\*\* `ls chapters/` (see what's in your repository)



---



\## 8. NAVIGATE TO REPOSITORY

```bash

cd ~/signalform-novel

```

\*\*What it does:\*\* Changes to your repository directory  

\*\*When to use:\*\* At the start of every session  

\*\*Essential:\*\* Must be in this folder for Git commands to work  

\*\*Alternative:\*\* `cd /c/Users/info/signalform-novel`



---



\## 9. VIEW RECENT COMMITS

```bash

git log --oneline -10

```

\*\*What it does:\*\* Shows your last 10 commits with messages  

\*\*When to use:\*\* To see what changes you've made recently  

\*\*Output:\*\* Short list of commit messages and IDs



---



\## 10. VIEW FILE CONTENTS

```bash

cat filename.md

```

\*\*What it does:\*\* Displays file contents in the terminal  

\*\*When to use:\*\* To quickly check file contents without opening an editor  

\*\*Page by page:\*\* Use `less filename.md` for longer files (press 'q' to quit)



---



\## TYPICAL WORKFLOW SEQUENCE:

```bash

\# 1. Navigate to repository

cd ~/signalform-novel



\# 2. Check current status

git status



\# 3. Copy new chapter

cp "/c/Users/info/OneDrive/Desktop/temp-chapters/signalform\_chapter\_08.md" "chapters/Chapter-08.md"



\# 4. Add, commit, and push

git add chapters/Chapter-08.md

git commit -m "Add Chapter 8: \[Chapter Title]"

git push origin main

```



---



\## BULK UPLOAD MULTIPLE CHAPTERS:

```bash

\# Copy multiple files (one at a time)

cp "/c/Users/info/OneDrive/Desktop/temp-chapters/signalform\_chapter\_08.md" "chapters/Chapter-08.md"

cp "/c/Users/info/OneDrive/Desktop/temp-chapters/signalform\_chapter\_09.md" "chapters/Chapter-09.md"

cp "/c/Users/info/OneDrive/Desktop/temp-chapters/signalform\_chapter\_10.md" "chapters/Chapter-10.md"



\# Add all chapters, commit, and push

git add chapters/

git commit -m "Bulk upload: Chapters 8-10"

git push origin main

```



---



\## USEFUL GIT BASH SHORTCUTS:

\- \*\*Paste:\*\* `Shift + Insert`

\- \*\*Copy:\*\* `Ctrl + Shift + C` (select text first)

\- \*\*Clear screen:\*\* `Ctrl + L`

\- \*\*Cancel command:\*\* `Ctrl + C`

\- \*\*Auto-complete:\*\* `Tab` (type partial filename and press Tab)



---



\## GIT BASH FILE PATHS:

\- \*\*Windows style:\*\* `C:\\Users\\info\\OneDrive\\Desktop\\temp-chapters\\`

\- \*\*Git Bash style:\*\* `/c/Users/info/OneDrive/Desktop/temp-chapters/`

\- \*\*Home directory:\*\* `~/` = `/c/Users/info/`

\- \*\*Current directory:\*\* `./`



---



\## TROUBLESHOOTING:

\- \*\*"not a git repository"\*\* → Run: `cd ~/signalform-novel`

\- \*\*"nothing to commit"\*\* → You forgot to `git add` your files

\- \*\*"failed to push"\*\* → Run `git pull origin main` first, then push again

\- \*\*File not found\*\* → Check file paths - use forward slashes `/` in Git Bash

\- \*\*Permission denied\*\* → Make sure you're in the right directory



---



\## USEFUL FILE OPERATIONS:

```bash

\# Create directory

mkdir new-folder



\# Remove file

rm filename.md



\# Move/rename file

mv oldname.md newname.md



\# Show current directory

pwd



\# Go back one directory

cd ..



\# Show file sizes

ls -la

```



---



\## YOUR REPOSITORY STRUCTURE:

```

~/signalform-novel/

├── chapters/

│   ├── Chapter-01.md

│   ├── Chapter-02.md

│   └── ...

├── notes/

│   ├── oracle-guide.md

│   └── character-notes.md

├── README.md

└── github-commands-reference.md

```



---



\*Save this file as: github-gitbash-commands-reference.md\*  

\*Keep it handy for quick reference during your writing sessions!\*  

\*Use `cat github-gitbash-commands-reference.md` to view it anytime!\*

