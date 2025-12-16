# Day 2 - Task 1: Branching & Merging (20 points)

## 🎯 Objective: 
Practice creating branches, merging, and handling conflicts.

## 📝 Steps to Complete:

### Step 1: Create Feature Branch
```bash
# From your exam/name branch, create a new branch:
# Name: feature/contact-page
# Use the MODERN Git command (not checkout)
# Write the command:
git switch -c feature/contact-page
```

### Step 2: Make Changes in Feature Branch
```bash
# In the file `conflict-example.txt` in this folder:
# Change line 5 from "Original text" to "Modified by [Your Name]"
# Commit with: "feat: update contact information"
# Write the commands:
git add conflict-example.txt
git commit -m "feat: update contact information"

```

### Step 3: Create Intentional Conflict
```bash
# First, switch back to your exam/name branch
# In the SAME file (conflict-example.txt):
# Change line 5 from "Original text" to "Main branch version"
# Commit with: "chore: update main branch"

```

### Step 4: Merge and Resolve Conflict
```bash
# Try to merge feature/contact-page into exam/name
# You should get a conflict! 
# Answer these questions:

1. What command shows you which files have conflicts?
Answer: git status

2. Open conflict-example.txt and resolve the conflict.
   Keep BOTH changes (your change AND "Main branch version")
   What does the resolved file look like? Paste it here:

```txt
# Contact Information
# -------------------
# Company: Tech Solutions Inc.
# Email: contact@techsolutions.com
# Phone: +1-555-0123

# This line will cause a conflict:
Main branch version
Modified by Muaad

# Address:
# 123 Main Street
# Tech City, TC 10101

# Leave everything below as is:
This file demonstrates merge conflicts.
Two people might edit the same line.
Git needs help deciding which change to keep.

3. After resolving, what TWO commands do you run to complete the merge?
Answer: 
   a. git add conflict-example.txt
   b. git commit -m "fix: resolve merge conflict between main and feature branch"

```