# restaurant-website-group7
##  Our Team

| Name | Role | GitHub Profile |
| :--- | :--- | :--- |
| **Marym Fouda** | Owner| [@marymfouda](https://github.com/marymfouda) |
| **Mahmoud Ammar** | Developer-1 | [@mahmoud-3mmar](https://github.com/mahmoud-3mmar)|
| **Mahmoud kamal** | Developer-2 | [@Mahmoud-Kama1](https://github.com/Mahmoud-Kama1) |

---
# 📌 Git & GitHub 

Welcome! If you are looking to master the art of version control and collaboration, you are in the right place. This is a simple, hands-on project designed to help beginners practice the core Git workflow.

##💡 Project Goals
The main objective is to understand how developers work together using:
* **Branching:** Working on features without breaking the main code.
* **Pull Requests (PR):** Suggesting changes for review.
* **Merging:** Integrating new updates into the final project.

---

## Core Concepts

### 1. What is Git & GitHub?
* **Git:** A version control system that tracks every change you make to your files.
* **GitHub:** A cloud-based platform where we host Git repositories to collaborate with others.

### 2. Pull Request (PR)
A PR is a way to notify others that you've completed a feature or fixed a bug. It allows the team to review your code before it becomes part of the main project.

### 3. Merging
Merging is the process of taking the history and changes from one branch and joining them into another (usually the `main` branch).

---
```bash
git clone [https://github.com/YOUR_USERNAME/learning-git-task.git](https://github.com/YOUR_USERNAME/learning-git-task.git)
```
---
Never work directly on the main branch. Create a new one for your changes:
```bash
git checkout -b add-my-profile
```
---
## ⚠️ Handling Merge Conflicts

### What is a Merge Conflict?
A conflict happens when two people edit the **same line** in the **same file**, or when one person deletes a file that another person is modifying. Git gets confused and asks you: *"Which version should I keep?"*

### How to Fix It (The Easy Way)
Don't panic! If Git tells you there is a conflict during a merge:

1. **Locate the Conflict:** Open the file mentioned by Git. You will see these markers:
   ```text
   <<<<<<< HEAD
   Your changes (the ones currently on the main branch)
   =======
   Their changes (the ones you are trying to pull/merge)
   >>>>>>> branch-name
   ```
   Should remove unkown character
   That is a great addition! Dealing with a **Merge Conflict** is usually the scariest part for beginners, but explaining it simply makes it much less intimidating.

Here is a new section you can add to your **README.md** that explains what a conflict is and how to fix it:

---

markdown
## ⚠️ Handling Merge Conflicts

### What is a Merge Conflict?
A conflict happens when two people edit the **same line** in the **same file**, or when one person deletes a file that another person is modifying. Git gets confused and asks you: *"Which version should I keep?"*

### How to Fix It (The Easy Way)
Don't panic! If Git tells you there is a conflict during a merge:

1. **Locate the Conflict:** Open the file mentioned by Git. You will see these markers:
   ```text
   <<<<<<< HEAD
   Your changes (the ones currently on the main branch)
   =======
   Their changes (the ones you are trying to pull/merge)
   >>>>>>> branch-name

```

2. **Choose the Winner:** Delete the markers (`<<<<<<<`, `=======`, `>>>>>>>`) and keep the code you actually want. You can keep one side, the other, or combine both!
3. **Finalize the Fix:**
* Save the file.
* Stage the fix: `git add <file-name>`
* Complete the merge: `git commit -m "Fix merge conflict"`



