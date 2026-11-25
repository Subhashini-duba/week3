# DEVOPS LAB – WEEK 3
## Git and GitHub Practical Experiments

**Subject:** DevOps Lab  
**Week:** 3  
**Experiments:** Program 2 and Program 3

---

## PROGRAM 2: Git Basic Commands and Repository Management

### Aim
To understand Git configuration, repository creation, file tracking, committing and viewing commit history.

### Description
Git is a distributed version control system used to track changes in source code. It helps developers manage different versions of their projects.

### Commands Executed

**1. Configure Git**
```bash
git config --global user.name "Student"
git config --global user.email "student@example.com"
git config --list
```

**2. Create a repository**
```bash
mkdir program2
cd program2
git init
```

**3. Create a file**
```bash
echo "Welcome to DevOps Lab" > index.txt
```

**4. Check repository status**
```bash
git status
```

**5. Add and commit files**
```bash
git add index.txt
git commit -m "First commit"
```

**6. View commit history**
```bash
git log --oneline
```

### Result
Successfully created a Git repository, configured Git, tracked files and saved changes using commits.

---

## PROGRAM 3: Git Remote Repository, Branching, Merging and Recovery

### Aim
To perform remote repository operations, branching, merging and recovery using Git commands.

### Description
GitHub is an online platform used to host Git repositories. Branching allows developers to work on separate features, while merging combines their changes.

### Commands Executed

**1. Connect remote repository**
```bash
git remote add origin https://github.com/YOUR-USERNAME/devops-week3.git
git remote -v
```

**2. Push code to GitHub**
```bash
git branch -M main
git push -u origin main
```

**3. Create and switch branches**
```bash
git branch feature
git switch feature
```

**4. Create and commit a feature**
```bash
echo "This is my feature branch" > feature.txt
git add .
git commit -m "Added feature"
```

**5. Merge branches**
```bash
git switch main
git merge feature
```

**6. Push changes**
```bash
git push origin main
git push origin feature
```

**7. Restore file changes**
```bash
echo "Original content" > sample.txt
git add sample.txt
git commit -m "Add sample file"

echo "Changed content" > sample.txt
git restore sample.txt
cat sample.txt
```

**8. Revert a commit**
```bash
git log --oneline
git revert COMMIT_ID
```
Replace `COMMIT_ID` with the actual commit ID of the commit you want to undo.

### Result
Successfully connected a local Git repository to GitHub, pushed files, created branches, merged changes and practiced recovery commands.

---

## Tools Used
- Git
- GitHub
- GitHub Codespaces
- Online Linux Terminal

## Conclusion
Through these experiments, I learned how to manage source code using Git and GitHub. I practiced repository initialization, file tracking, commits, remote operations, branching, merging and recovery commands.

## Screenshots
Add your practical execution screenshots below:

1. Git configuration and initialization
2. Git status and commit
3. Git log
4. GitHub remote connection
5. Successful push
6. Branch creation
7. Branch merging
8. Git restore
9. Git revert

---

**End of Week 3 DevOps Lab Experiments**
