# 📚 GitHub Beginner's Guide Repository

This repository is a hands-on sandbox for anyone learning how to use Git and GitHub. Whether you're just starting out or need structured practice, this will walk you through everything from cloning to making pull requests. The goal: **make you comfortable with version control and collaborating on open-source platforms.**

---

## 🧠 What You'll Learn

- Basic Git commands
- Setting up Git
- Forking and cloning repositories
- Working with branches
- Committing and pushing changes
- Creating pull requests
- Resolving merge conflicts
- Collaborating with others

---

## 🔧 Setup Instructions

### 1. Install Git

Check if Git is already installed:

```bash
git --version
```

If not, download from [https://git-scm.com/downloads](https://git-scm.com/downloads)

### 2. Configure Git

```bash
git config --global user.name "Your Name"
git config --global user.email "youremail@example.com"
```

---

## 🚀 Workflow Summary

```
FORK → CLONE → BRANCH → COMMIT → PUSH → PULL REQUEST → MERGE
```

---

## 🛠️ Step-by-Step Instructions

### ✅ Fork the Repository

1. Go to the repo page on GitHub
2. Click the **Fork** button on the top-right
3. The repo is now copied to your account

---

### ✅ Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/this-repo.git
cd this-repo
```

---

### ✅ Create a Branch

```bash
git checkout -b your-branch-name
```

Use a meaningful branch name:  
Example: `git checkout -b add-naveen-file`

---

### ✅ Make a Change

Create a new file:

```bash
echo "Hello, I'm Naveen!" > contributions/naveen.txt
```

Or edit an existing file:

```bash
nano examples/sample.txt
```

---

### ✅ Stage and Commit

```bash
git add .
git commit -m "Add naveen.txt with introduction"
```

Use clear commit messages.

---

### ✅ Push to Your Fork

```bash
git push origin your-branch-name
```

---

### ✅ Open a Pull Request (PR)

1. Go to your forked repo on GitHub
2. Click **Compare & pull request**
3. Add a title and description
4. Submit the PR to the original repo

---

## 🔄 Syncing with Upstream

If the original repo updates, sync your local copy:

```bash
git remote add upstream https://github.com/ORIGINAL_OWNER/this-repo.git
git fetch upstream
git checkout main
git merge upstream/main
```

To push updates to your fork:

```bash
git push origin main
```

---

## 🔀 Resolving Merge Conflicts

If there's a conflict:

```bash
git pull origin main
# Fix conflicts in files manually
git add conflicted-file
git commit
```

Then push again:

```bash
git push origin your-branch-name
```

---

## 📁 Recommended Directory Layout

```
this-repo/
├── README.md
├── examples/
│   ├── sample.txt
├── contributions/
│   ├── your-name.txt
├── .gitignore
├── LICENSE
```

---

## 🧪 Suggested Exercises

| Task                             | File Path                | Difficulty |
|----------------------------------|---------------------------|------------|
| Add your name                   | `contributions/`          | Easy       |
| Edit a line in `sample.txt`     | `examples/sample.txt`     | Easy       |
| Create a new folder             | `examples/<your-name>/`   | Medium     |
| Delete a file                   | `rm contributions/temp.txt` | Medium     |
| Resolve a merge conflict        | Any file                  | Hard       |

---

## 🧹 Best Practices

- Commit often, with clear messages
- Keep your branches focused on one task
- Never commit secrets (e.g. passwords, API keys)
- Pull before pushing
- Review your code before submitting PRs

---

## 📚 Additional Learning Resources

- [Pro Git Book](https://git-scm.com/book/en/v2)
- [GitHub Docs](https://docs.github.com/en)
- [Git Cheatsheet](https://education.github.com/git-cheat-sheet-education.pdf)
- [Learn Git Branching](https://learngitbranching.js.org/)

---

## 🧑‍💻 Contribute to This Repo

You are encouraged to:

- Add your name to the `contributors` list
- Improve this README
- Create sample projects in the repo
- Help others in issues or PRs

---

## 🙌 Contributors

| Name            | Secret                      |
|-----------------|-----------------------------------|
| Naveen Srinivas | I like reading fantasy novels and hate romance |
| Aadarsh Mahesh K| |

To add your name:

```bash
echo "- Your Name | What You Did" >> CONTRIBUTORS.md
```

Then commit and push.

---

## 📜 License

MIT License. Use freely with attribution.