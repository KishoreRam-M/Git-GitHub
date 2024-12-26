

### 1. **What is Git?**
Git is a **distributed version control system (VCS)** that tracks changes in source code during software development. It allows multiple developers to work on the same project without interfering with each other's work, by providing powerful tools for merging changes, managing branches, and tracking history.

### 2. **Why Use Git?**
- **Version control**: Keeps a history of changes made to files, allowing you to go back to previous versions when necessary.
- **Collaboration**: Supports multiple developers working on the same project simultaneously.
- **Branching & Merging**: Makes it easy to experiment with new features and merge changes seamlessly.
- **Distributed**: Each developer has a full copy of the repository, enabling them to work offline.

---

### 3. **Basic Git Concepts**
- **Repository (Repo)**: A directory that stores all the files and history of a project.
  - **Local Repository**: A Git repository on your own computer.
  - **Remote Repository**: A repository hosted on a server (e.g., GitHub, GitLab, Bitbucket).
  
- **Commit**: A snapshot of changes made to files in the repository at a specific point in time.
  
- **Branch**: A separate line of development that allows developers to work on features or fixes without affecting the main codebase (usually called `main` or `master`).

- **Merge**: The process of combining changes from one branch into another.

- **Clone**: A copy of a repository, typically downloaded from a remote source to work on locally.

---

### 4. **Core Git Commands**

#### 4.1. **Setting Up a Repository**
- **Initialize a new Git repository**:
  ```bash
  git init
  ```
  This creates a new `.git` directory in your project folder to start tracking changes.

- **Clone an existing repository**:
  ```bash
  git clone <repository-url>
  ```
  This creates a copy of the repository from a remote server (e.g., GitHub) to your local machine.

#### 4.2. **Working with Changes**
- **Check the status** of the repository:
  ```bash
  git status
  ```
  This shows which files have been modified, added, or deleted.

- **Add changes** to the staging area:
  ```bash
  git add <file-name>    # Add specific file
  git add .              # Add all changes
  ```

- **Commit changes**:
  ```bash
  git commit -m "Your commit message"
  ```

#### 4.3. **Managing Branches**
- **Create a new branch**:
  ```bash
  git branch <branch-name>
  ```

- **Switch to a branch**:
  ```bash
  git checkout <branch-name>
  ```

- **Create and switch to a new branch**:
  ```bash
  git checkout -b <branch-name>
  ```

- **Merge branches**:
  ```bash
  git merge <branch-name>
  ```

#### 4.4. **Remote Repositories**
- **Add a remote repository**:
  ```bash
  git remote add origin <repository-url>
  ```

- **Push changes** to a remote repository:
  ```bash
  git push origin <branch-name>
  ```

- **Pull changes** from a remote repository:
  ```bash
  git pull origin <branch-name>
  ```

- **Fetch changes** without merging:
  ```bash
  git fetch
  ```

---

### 5. **Advanced Git Concepts**

#### 5.1. **Rebase**
Rebase is a command that allows you to integrate changes from one branch into another. Unlike merge, which creates a new commit, rebase rewrites history by applying changes on top of another branch.

```bash
git rebase <branch-name>
```

#### 5.2. **Stashing Changes**
If you need to switch branches but don’t want to commit your current changes, you can "stash" them.

```bash
git stash
```

Later, you can apply the stashed changes:

```bash
git stash apply
```

#### 5.3. **Tagging**
Git tags are used to mark specific points in history, typically for release versions.

```bash
git tag <tag-name>
```

To push tags to the remote repository:

```bash
git push origin <tag-name>
```

---

# Top Git Prompt

1. **`git init`**  
   Initializes a new Git repository in the current directory.

2. **`git clone <repository>`**  
   Creates a local copy of a remote repository.

3. **`git add <file>`**  
   Stages changes to a file, preparing it for commit.

4. **`git commit -m "<message>"`**  
   Records changes to the repository with a commit message.

5. **`git status`**  
   Displays the current status of the working directory and staging area.

6. **`git log`**  
   Shows the commit history for the current branch.

7. **`git pull`**  
   Fetches and merges changes from the remote repository into the current branch.

8. **`git push`**  
   Uploads local commits to a remote repository.

9. **`git branch`**  
   Lists all branches in the repository. It can also be used to create or delete branches (`git branch <branch-name>`).

10. **`git checkout <branch>`**  
    Switches to a specified branch in the repository.

11. **`git merge <branch>`**  
    Merges changes from another branch into the current branch.

12. **`git remote add <name> <url>`**  
    Adds a remote repository URL to the project.

13. **`git reset`**  
    Undoes changes by resetting the current branch to a previous state.

14. **`git stash`**  
    Temporarily saves changes that are not ready to be committed, allowing you to work on something else.

15. **`git diff`**  
    Shows the differences between the working directory and the index, or between commits.

