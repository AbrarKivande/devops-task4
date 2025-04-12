# DevOps Internship – Task 4 Documentation

## Objective
To manage a DevOps project using Git and GitHub best practices including:
- Branching strategies
- Pull requests
- Tagging
- Documentation

---

## Step-by-Step Workflow

### 🔸 Step 1: Initialized Git
```bash
git init

🔸 Step 2: Created GitHub Repo and Linked It
bash
Copy
Edit
git remote add origin https://github.com/<your-username>/devops-task4.git

🔸 Step 3: Created README.md and .gitignore
bash
Copy
Edit
echo "# DevOps Task 4" > README.md
echo "node_modules/" > .gitignore

🔸 Step 4: First Commit to main
bash
Copy
Edit
git add .
git commit -m "Initial commit"
git branch -M main
git push -u origin main

🔸 Step 5: Created dev and feature/login Branches
bash
Copy
Edit
git checkout -b dev
git push -u origin dev

git checkout -b feature/login
git push -u origin feature/login

🔸 Step 6: Added Feature File
bash
Copy
Edit
echo "console.log('Login feature')" > login.js
git add login.js
git commit -m "Add login feature"
git push

🔸 Step 7: Pull Request from feature/login → dev
Created pull request and merged it via GitHub UI.

🔸 Step 8: Created Git Tag
bash
Copy
Edit
git checkout dev
git tag -a v1.0 -m "First dev release"
git push origin v1.0

🔸 Step 9: Merged dev into main
Another pull request was created from dev to main.

