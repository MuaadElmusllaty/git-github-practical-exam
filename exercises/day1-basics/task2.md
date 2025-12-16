

```markdown
# Day 1 - Task 2: File Management (20 points)

## 🎯 Objective: 
Practice adding, modifying, and viewing file changes.

## 📝 Steps to Complete:

### Step 1: Create Multiple Files
```bash
# Create 3 new files in day1-tasks/ folder:
# - notes.txt (with some text)
# - practice.md (with "# Practice" as content)  
# - temp-file.tmp (empty)
# Write the commands you used:(I'm powershell guy) so inside day1-tasks/ folder:
    "some text">notes.txt
    "# Practice">practice.md
    "">temp-file.tmp

```

### Step 2: Stage and Commit Selectively
```bash
# Stage ONLY notes.txt and practice.md (not temp-file.tmp)
# Commit with message: "feat: add practice files"
# Write the commands:
git add notes.txt practice.md
git commit -m "feat: add practice files"

```

### Step 3: Create .gitignore
```bash
# Create a .gitignore file in the root folder
# Make it ignore ALL .tmp files
# Write the content of your .gitignore here:
"*.tmp" > .gitignore
```




