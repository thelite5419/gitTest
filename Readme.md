## **Git Commands and Configuration Guide**

### **Initializing a Repository**

To create a new Git repository locally:

```plaintext
git init
```

This will create an empty Git repository in your directory.

### **Adding Changes**

To stage changes for a particular file or directory:

```plaintext
git add [file path / directory path]
```

To add all changes in the current directory:

```plaintext
git add .
```

This will stage the modified or new files for the next commit.

### **Committing Changes**

To save the changes you made in the repository, use:

```plaintext
git commit -m "[commit message]"
```

The commit message should briefly describe the changes.

### **Pushing Changes to GitHub**

Once you have committed your changes, you can push them to GitHub using:

```plaintext
git push -u origin main
```

Make sure you have set the remote repository by adding its URL with the command:

```plaintext
git remote add origin [repository URL]
```

The `push` command uploads the local commits to GitHub.

### **Pulling Changes**

To pull the latest changes from a remote repository:

```plaintext
git pull
```

This will fetch and integrate the latest changes from the remote repository into your local branch.

## **If you are connecting to a pre-existing repository that has a different history, use:** `**bash git pull origin main --allow-unrelated-histories**`

### **Cloning a Repository**

To clone an existing repository from GitHub:

```plaintext
git clone [repository URL]
```

This command downloads the repository to your local machine, preserving the entire version history.

### **Viewing Commit Logs**

To see the history of commits, use:

```plaintext
git log
```

This command displays commit messages, dates, and authors.

### **Email Configuration**

Before making commits, configure your Git with your name and email. To set these globally:

```plaintext
git config --global user.email "your-email@example.com"
git config --global user.name "your-username"
```

To verify the configuration:

```plaintext
git config --list --global
```

### **Branching in Git**

Branches allow you to work on different parts of a project independently.

To list all branches:

To create a new branch:

To switch to another branch:

To merge a branch into the current branch:

To handle switching between branches:

```plaintext
git checkout [branch-name]
```

This command moves you between branches, allowing you to work on different versions of the code.

### **Handling Merge Conflicts**

When working on the same files, merge conflicts can occur. To abort a conflicted merge:

```plaintext
git merge --abort
```

This will stop the merge process and revert back to the previous state.

### **Force Push Command**

To forcefully push your changes to the remote repository, use:

```plaintext
git push <remote> --force
```

This should be used with caution as it overwrites the remote history. You can copy this markdown file to your project and save it as `README.md` for a clean, structured guide to using Git commands.

```plaintext
git merge [branch-name]
```

```plaintext
git switch [branch-name]
```

```plaintext
git branch [branch-name]
```

```plaintext
git branch
```