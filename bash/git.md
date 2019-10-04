# Git Cheat Sheet

* Changes
* Config
* Branches
* Initialize
* Review
* Refactor
* Redo
* Suppress
* Synchronize
* Fragments

---

### Changes

```bash
# List All Modified or Staged Files
$ git status

# Modified Files not yet Staged
$ git diff

# Add File to Staging
$ git add [file]

# Changes between Staging and Last File Version
$ git diff --staged

# Unstages the File
$ git reset [file]

# Records File Snapshot to Version History
$ git commit -m [message]
```

---

### Config

```bash
# Global Config
$ git config --global [action]

# Name
$ git config user.name "[name]"

# Email
$ git config user.email "[email]"

# Color
$ git config color.ui auto
```

---

### Branches

```bash
# List All Local Branches
$ git branch

# Create New Branch
$ git branch [branch-name]

# Switches to Specified Branch
$ git branch checkout [branch-name]

# Combines Branch History into Current Branch
$ git merge [branch-name]

# Deletes Specified Branch
$ git branch -d [branch-name]
```

---

### Intialize

```bash
# Create a Git Initialized Project Directory
$ git init [project-name]

# Initialize current Directory
$ git init

# Clone Git Repository
$ git clone [url]
```

---

### Review

```bash
# Version history for current Branch
$ git log

# Version history for File
$ git log --follow [file]

# Content Differences between Branches
$ git diff [branch-1]...[branch-2]

# Metadata and Content changes of Commit
$ git show [commit]
```

---

### Refactor

```bash
# Delete File from Working Directory
$ git rm [file]

# Removes File from Version Control
$ git rm --cached [file]

# Changes File locally and prepares for Commit
$ git mv [file-original] [file-renamed]
```

---

### Redo

```bash
# Undo all commits after [commit]
$ git reset [commit]

# Discards all changes after [commit]
$ git reset --hard [commit]
```

---

### Suppress


```bash
# List all Ignored Files
$ git ls-files --other --ignored --exclude-standard
```

---

### Synchronize

```bash
# Downloads all history from Repo Bookmark
$ git fetch [bookmark]

# Combines Bookmark Branch into Local Branch
$ git merge [bookmark]/[branch-name]

# Uploads all Local Commits to Github/Gitlab/BitBucket/etc.
$ git push [alias] [branch]

# Downloads Bookmark History and Incorporate Changes
$ git pull

# List Remote Origins
$ git remote -v

# Add Remote Origin
$ git remote add [remote-name] [url]

# Remove Remote Origin
$ git remote remove [remote-name]
```

---

### Fragments

```bash
# Temporarily Stores all Modified Tracked Files
$ git stash

# Restore the most recent Tracked Files
$ git stash pop

# List all Change Sets
$ git stash list

# Discard most recent Change Set
$ git stash drop
```
