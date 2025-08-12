# GitHub PowerShell Commands Reference
## Top 10 Essential Commands for Your Novel Repository

---

## 1. CHECK STATUS
```powershell
git status
```
**What it does:** Shows which files have been changed, added, or need to be committed  
**When to use:** Before making commits to see what changes you have  
**Example output:** Lists modified files, new files, files ready to commit

---

## 2. COPY FILES TO REPOSITORY
```powershell
copy "C:\Users\info\OneDrive\Desktop\temp-chapters\filename.md" "chapters\Target-Name.md"
```
**What it does:** Copies files from your temp folder to the repository  
**When to use:** When you have new chapter content to upload  
**Your pattern:** `signalform_chapter_XX.md` → `Chapter-XX.md` (or `chapter-XX.md`)

---

## 3. ADD FILES TO GIT TRACKING
```powershell
git add chapters/Chapter-01.md
```
**What it does:** Tells Git to track changes to specific files  
**When to use:** After copying new content, before committing  
**Bulk version:** `git add chapters/` (adds all files in chapters folder)

---

## 4. COMMIT CHANGES
```powershell
git commit -m "Your descriptive message here"
```
**What it does:** Saves your changes with a description  
**When to use:** After adding files, before pushing to GitHub  
**Good messages:** "Add Chapter 8", "Update oracle guide", "Revise Chapter 1-3"

---

## 5. PUSH TO GITHUB
```powershell
git push origin main
```
**What it does:** Uploads your committed changes to GitHub  
**When to use:** After committing, to make changes live online  
**Result:** Your files become visible on github.com

---

## 6. BULK ADD AND COMMIT
```powershell
git add chapters/ && git commit -m "Bulk update: Chapters 1-7" && git push origin main
```
**What it does:** Adds all chapter files, commits them, and pushes in one command  
**When to use:** When updating multiple chapters at once  
**Time saver:** Combines steps 3, 4, and 5

---

## 7. LIST FILES IN DIRECTORY
```powershell
dir "C:\Users\info\OneDrive\Desktop\temp-chapters\*.md"
```
**What it does:** Shows all .md files in your temp folder  
**When to use:** To see what chapter files you have ready to upload  
**Also useful:** `dir chapters\` (see what's in your repository)

---

## 8. NAVIGATE TO REPOSITORY
```powershell
cd C:\Users\info\signalform-novel
```
**What it does:** Changes to your repository directory  
**When to use:** At the start of every session  
**Essential:** Must be in this folder for Git commands to work

---

## 9. VIEW RECENT COMMITS
```powershell
git log --oneline -10
```
**What it does:** Shows your last 10 commits with messages  
**When to use:** To see what changes you've made recently  
**Output:** Short list of commit messages and IDs

---

## 10. FORCE OVERWRITE FILES
```powershell
copy "source\file.md" "destination\file.md" /Y
```
**What it does:** Copies and overwrites without asking for confirmation  
**When to use:** When updating existing chapters with revised versions  
**The /Y flag:** Automatically says "yes" to overwrite prompts

---

## TYPICAL WORKFLOW SEQUENCE:
```powershell
# 1. Navigate to repository
cd C:\Users\info\signalform-novel

# 2. Check current status

# 4. Add, commit, and push
```

---

## BULK UPLOAD MULTIPLE CHAPTERS:
```powershell
# Copy multiple files
copy "C:\Users\info\OneDrive\Desktop\temp-chapters\signalform_chapter_*.md" "chapters\"

# Add all chapters, commit, and push
git add chapters/
git commit -m "Bulk upload: Chapters X-Y"
git push origin main
```

---

## TROUBLESHOOTING:
- **"not a git repository"** → Run: `cd C:\Users\info\signalform-novel`
- **"nothing to commit"** → You forgot to `git add` your files
- **"failed to push"** → Run `git pull origin main` first, then push again
- **File not found** → Check file paths and spelling carefully

---

## YOUR REPOSITORY STRUCTURE:
```
signalform-novel/
├── chapters/
│   ├── Chapter-01.md (or chapter-01.md)
│   ├── Chapter-02.md
│   └── ...
├── notes/
│   ├── oracle-guide.md
│   └── character-notes.md
└── README.md
```

---

*Save this file as: github-commands-reference.txt*  
*Keep it handy for quick reference during your writing sessions!*git add chapters/Chapter-08.md
git commit -m "Add Chapter 8: [Chapter Title]"
git push origin main

# 3. Copy new chapter(s)
copy "C:\Users\info\OneDrive\Desktop\temp-chapters\signalform_chapter_08.md" "chapters\Chapter-08.md"

