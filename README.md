# Comprehensive Git and Pull Request Tutorial (Xplore)

This interactive tutorial will guide you through the process of using Git commands and making a pull request to contribute to this project. We'll cover basic Git operations and troubleshooting tips. Follow the steps carefully and don't hesitate to ask for clarification if you encounter any issues.

## Getting Started

1. **Fork this repository** to your GitHub account by clicking the "Fork" button in the top-right corner of the repository page.
![Forking a Repository](https://github.com/SharanRP/Xplore/assets/136159249/caaa1619-d5c7-4108-b60b-16de8d26884f)

2. **Clone the forked repository** to your local machine:
```bash
git clone https://github.com/YOUR_USERNAME/Xplore.git
```
Replace `YOUR_USERNAME` with your actual GitHub username.

3. **Navigate to the project directory**:
```bash
cd Xplore
```

4. **Create a new branch** for your changes:
```bash
git checkout -b feature/your-feature-name
```
Replace `your-feature-name` with a descriptive name for your feature or change.

<hr>
🚨 **Potential Issue:** If you encounter an error saying `fatal: not a git repository`, it means you're not in the correct directory. Navigate to the `Xplore` directory and try again.
<hr>

## Basic Git Commands

### Checking Status
To see the current status of your repository:
```bash
git status
```

### Viewing Branches
To see all branches and identify the current branch:
```bash
git branch
```

### Switching Branches
To switch to an existing branch:
```bash
git checkout branch-name
```

To create a new branch and switch to it:
```bash
git checkout -b new-branch-name
```

### Stashing Changes
To temporarily store your changes without committing:
```bash
git stash
```

To apply the most recent stash:
```bash
git stash pop
```

To list all stashes:
```bash
git stash list
```

To apply a specific stash:
```bash
git stash apply stash@{n}
```
Replace `n` with the stash number.

### Resetting Changes
To unstage changes (but keep them in your working directory):
```bash
git reset HEAD file-name
```

To discard changes in your working directory:
```bash
git checkout -- file-name
```

To reset to a specific commit:
```bash
git reset --hard commit-hash
```
Be cautious with `--hard` as it discards all changes!

## Making Changes

5. Make your desired changes to the codebase using your favorite code editor.

6. **Stage your changes**:
```bash
git add .
```
This command stages all the changes you've made.

To stage specific files:
```bash
git add file-name1 file-name2
```

7. **Commit your changes** with a descriptive message:
```bash
git commit -m "Add feature xyz"
```
Replace `"Add feature xyz"` with a concise description of your changes.

<hr>
🚨 **Potential Issue:** If you encounter an error saying `nothing added to commit but untracked files present`, it means you have new files that haven't been staged. Run `git add .` again and then commit your changes.
<hr>

## Pushing Changes

8. **Push your changes** to your forked repository:
```bash
git push origin feature/your-feature-name
```
Replace `your-feature-name` with the name of your branch.

<hr>
🚨 **Potential Issue:** If you encounter an error saying `remote origin already exists`, you may need to set the upstream repository by running:
```bash
git remote add upstream https://github.com/SharanRP/Xplore.git
```
Then try pushing your changes again.
<hr>

## Creating a Pull Request

9. Visit your forked repository on GitHub.

10. Switch to the branch you just pushed by clicking on the "Branch" dropdown and selecting your branch.
![Switching Branches](https://github.com/SharanRP/Xplore/assets/136159249/f96a022d-721a-433b-9c31-dbaa7d26748f)

11. Click on the "New Pull Request" button.
![New Pull Request](https://github.com/SharanRP/Xplore/assets/136159249/4f76b5bc-859c-4546-a1c7-af0a528800c5)

12. Provide a descriptive title and description for your pull request, explaining the changes you've made and their purpose.

13. Click on the "Create Pull Request" button to submit your pull request.
![Create Pull Request](https://github.com/SharanRP/Xplore/assets/136159249/d0c7383e-9dae-436d-af27-f5728ec90e6d)

<hr>
🎉 Congratulations! You've successfully created a pull request. The project maintainers will review your changes and provide feedback or merge them into the main repository.
<hr>

## Additional Git Commands

### Viewing Commit History
To see the commit history:
```bash
git log
```

For a more concise view:
```bash
git log --oneline
```

### Fetching Updates
To fetch updates from the remote repository without merging:
```bash
git fetch origin
```

### Merging Changes
To merge changes from another branch into your current branch:
```bash
git merge branch-name
```

### Resolving Conflicts
If you encounter merge conflicts, Git will mark the conflicting areas in your files. Manually resolve these conflicts, then:
```bash
git add .
git commit -m "Resolve merge conflicts"
```

### Pulling Changes
To fetch and merge changes from the remote repository:
```bash
git pull origin main
```
Replace `main` with the branch name you want to pull from.

## Adding Your Information
Please add your name and registration number below:
- Name: [Your Name]
- Registration Number: [Your Registration Number]

Remember, practice makes perfect! Don't be afraid to experiment with these Git commands in a test repository to get more comfortable with them.
