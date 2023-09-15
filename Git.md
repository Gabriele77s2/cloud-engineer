# Git

1. **Git:** Git is a distributed version control system that allows developers to track changes in their codebase, collaborate with others, and manage software development projects efficiently.

2. **Repository (Repo):** A repository is a storage location where all the files and version history for a Git project are stored. It can be local or remote.

3. **Commit:** A commit is a snapshot of the project's files at a specific point in time. Developers create commits to save changes made to their codebase.

4. **Branch:** A branch is a separate line of development in Git. Developers can create branches to work on new features, bug fixes, or experimental changes without affecting the main codebase.

5. **Master/Main Branch:** The default branch in Git, often called "master" or "main," is the primary branch where the stable and production-ready code is kept.

6. **Clone:** Cloning is the process of creating a copy of a remote repository on a local machine. This allows developers to work on the code locally.

7. **Push:** Pushing is the act of uploading local commits to a remote repository. This makes changes available to other collaborators.

8. **Pull:** Pulling is the process of downloading changes from a remote repository to a local repository. It's used to update a local branch with changes made by others.

9. **Merge:** Merging is the process of combining the changes from one branch into another. It's typically used to integrate feature branches into the main branch.

10. **Pull Request (PR):** A pull request is a way for developers to propose changes to a repository. It allows others to review the changes before they are merged.

11. **Fork:** Forking is the act of creating a copy of someone else's repository under your own account. It's often used when you want to contribute to a project.

12. **Merge Conflict:** A merge conflict occurs when Git cannot automatically merge two sets of changes due to conflicting edits in the same part of a file. Resolving conflicts requires manual intervention.

13. **Checkout:** Checking out is the process of switching between different branches or commits in Git. It allows developers to work on different parts of the project.

14. **Tag:** A tag is a reference to a specific commit, often used to mark important milestones or releases in a repository.

15. **Remote:** A remote is a reference to a repository hosted on a server, usually on platforms like GitHub, GitLab, or Bitbucket.

16. **Stash:** Stashing is the act of temporarily saving changes that are not ready to be committed so that you can switch branches or perform other operations.

17. **Gitignore:** A .gitignore file specifies which files or directories should be ignored by Git. It's used to prevent unneeded files from being tracked.

18. **Version Control:** Version control is a system that manages changes to files over time, allowing you to track and control different versions of your codebase.

19. **Git Client:** A Git client is a software tool or application that provides a user interface for interacting with Git repositories. Examples include Git command-line, Git GUI tools, and integrated development environments (IDEs) with Git support.

20. **SHA-1:** SHA-1 (Secure Hash Algorithm 1) is a cryptographic hash function used by Git to generate unique identifiers (hashes) for commits, tags, and other objects in the repository.

21. **Rebase:** Rebasing is a Git operation used to combine or integrate changes from one branch onto another by moving, or "replaying," the commits from one branch onto another. It can be used to maintain a cleaner and linear commit history.

22. **Cherry-Pick:** Cherry-picking is the process of selecting specific commits from one branch and applying them to another. It's useful when you only want to incorporate specific changes rather than merging an entire branch.

23. **Conflict Resolution Tool:** A conflict resolution tool is a tool or editor that helps developers resolve merge conflicts by highlighting and allowing them to manually edit conflicting sections of code.

24. **HEAD:** HEAD is a special pointer in Git that always points to the latest commit in the currently checked-out branch. It represents the current working directory state.

25. **Submodule:** A submodule is a Git repository embedded within another Git repository. Submodules allow you to include external repositories as dependencies in your project.

26. **Pull (Fetch and Merge):** The pull operation in Git combines the fetch and merge steps. It first fetches changes from a remote repository and then automatically merges them into the current branch.

27. **Remote Tracking Branch:** A remote tracking branch is a local reference that keeps track of the state of a branch in a remote repository. It allows you to see how the remote branch has changed without merging the changes into your local branch.

28. **Bare Repository:** A bare repository is a special type of Git repository that does not have a working directory. It is typically used on servers for centralized collaboration and does not contain the actual project files.

29. **Ancestor and Descendant Commits:** In Git, commits can be categorized as ancestors and descendants. Ancestor commits are those that came before the current commit, while descendant commits are those that come after the current commit in the commit history.

30. **Interactive Rebase:** Interactive rebase is a rebase operation that allows you to interactively choose which commits to include, reorder commits, edit commit messages, or squash multiple commits into one.

31. **Git Hooks:** Git hooks are scripts or executables that can be run automatically at various points in the Git workflow, such as before or after commits, pushes, or merges. They are used for customizing Git's behavior.

32. **Reflog:** The reflog is a Git command that maintains a log of all references' changes in the repository. It's useful for recovering lost commits or branches.

33. **Patch:** A patch is a text file that represents the differences between two sets of code changes. It's often used for sharing changes with others or applying changes to a different branch.

34. **Git Workflows:** Git workflows are predefined processes or strategies for how changes are managed, reviewed, and integrated into a project. Popular workflows include GitFlow, GitHub Flow, and GitLab Flow.

35. **Git LFS (Large File Storage):** Git LFS is an extension for Git that handles large files more efficiently by storing them outside the regular Git repository, reducing repository size.

## Git commands

1. **git init**: Initializes a new Git repository in the current directory.

2. **git clone [repository_url]**: Creates a copy of a remote Git repository on your local machine.

3. **git add [file(s)]**: Stages changes for commit. You can specify individual files or use a wildcard (*) to stage all changes.

4. **git commit -m "[commit_message]"**: Records staged changes in a new commit with a descriptive message.

5. **git status**: Shows the current status of your working directory, including untracked, modified, and staged files.

6. **git log**: Displays a log of all commits in the current branch, showing commit messages, authors, and timestamps.

7. **git branch**: Lists all local branches in the repository and highlights the current branch.

8. **git branch [branch_name]**: Creates a new branch with the specified name.

9. **git checkout [branch_name|commit_hash]**: Switches to the specified branch or commit.

10. **git merge [branch_name]**: Combines changes from the specified branch into the current branch.

11. **git pull**: Fetches changes from a remote repository and merges them into the current branch (equivalent to `git fetch` + `git merge`).

12. **git push**: Pushes your local commits to a remote repository.

13. **git remote -v**: Lists all remote repositories associated with your local repository.

14. **git remote add [name] [repository_url]**: Adds a remote repository with a specified name.

15. **git remote remove [name]**: Removes a remote repository from your configuration.

16. **git diff**: Shows the differences between the working directory and the last commit.

17. **git checkout -b [new_branch_name]**: Creates a new branch and switches to it in one command.

18. **git reset [file(s)]**: Unstages changes for the specified file(s).

19. **git fetch**: Downloads changes from a remote repository but does not merge them into your local branch.

20. **git stash**: Temporarily saves your changes in a "stash" so you can switch branches or perform other operations.

21. **git tag [tag_name]**: Creates a new tag at the current commit, typically used for marking releases.

22. **git rebase [branch_name]**: Replays commits from the current branch on top of the specified branch, creating a linear history.

23. **git cherry-pick [commit_hash]**: Applies the changes from a specific commit onto the current branch.

24. **git clean -n**: Shows which untracked files would be removed by `git clean -f`.

25. **git blame [file]**: Displays the commit history of each line in a file, showing who last modified each line.

26. **git submodule init**: Initializes submodules in your repository.

27. **git submodule update**: Updates submodules to the latest commit in their respective repositories.

28. **git log --graph --oneline --all**: Shows a simplified and graphical representation of the commit history for all branches.
