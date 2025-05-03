# new-project

## Step-by-step: Setting up a new Git repository with a development branch

### 1. Create a new GitHub repository

Go to [GitHub](https://github.com/) and click on **"New Repository"**.

- Repository name: `new-project`
- Set it to **Private** or **Public**, as needed.
- Initialize with a README (optional, can skip if doing it locally)

---

### 2. Clone the repository locally

```bash
git clone https://github.com/your-org-or-username/new-project.git
cd new-project
```

### 3. Create a development branch

```bash
git checkout -b development
```

### 4. Make your changes

```bash
echo "# new-project" > README.md
echo -e "\nThis project is under development." >> README.md
```

### 5. Stage and commit your changes

```bash
git add README.md
git commit -m "Added README with setup instructions"
```

### 6. Push the development branch to GitHub

```bash
git push origin development
```

### 7. Create a Pull Request to merge into main

Go to your `repo` on [GitHub](https://github.com/) → **Pull Requests** → **New Pull Request**

-- Base: `main`
-- Compare: `development`
-- Submit PR and merge

### 8. Sync local main branch (optional)

```bash
git checkout main
git pull origin main
```