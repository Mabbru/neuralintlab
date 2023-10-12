# Week6_lecture_note

## Changesvs.Snapshots

---
![image](https://github.com/Mabbru/neuralintlab/assets/105326662/a3a5075e-9a31-4717-aa85-333442224c97)
---

## Local, Centralized, and Distributed Version control

---
![image](https://github.com/Mabbru/neuralintlab/assets/105326662/c274a636-0273-4aef-91a6-5068c8e8a725)
---

## Three staes in Git
### Modified:
Working Directory ⇒ A
### staged:
staging Area ⇒ B
### comitted:
git directory(Repository) ⇒ C

C → A : Checkout the project // A → B : Stage Fixes // B → C : Commit

## *Git Config*
Git configurations are stored in three levels:
System Level → Global(uesr) Level → Local Level
ex) $ git config --list --shiw-orgin 

- First-time setup
- lnitializing a repository in an existing directory($git -init) Checking repository status($git status)
- Adding a new file to be staged(tracked)($git add [file_name])
- Unstaging a file($git rm-cached[file_name])
- Ignoring a file(.gitignore file)
- Commit($git commit -m "commit message")
- Change branch name
