# Differences Between Git Merge and Git Rebase
## 1. Core Logical Differences
- **Git merge**: Merges commits from two branches and creates a brand-new "merge commit". It fully preserves the commit history of all branches with diverged tracks, featuring excellent traceability.
- **Git rebase**: Moves all commits of the current branch to follow the latest commit of the target branch. No new merge commit is generated, resulting in a clean linear commit history.

## 2. Differences in Commit History Display
- **merge**: Complete history records are retained, clearly showing the whole process of branch divergence and merging, with every development step well-documented.
- **rebase**: Presents concise linear commit history without divergence traces, ideal for sorting commits on personal branches.

## 3. Differences in Conflict Resolution
- **merge**: Conflicts only need to be resolved once during merging, which is simple and less error-prone.
- **rebase**: If conflicts exist in multiple commits, users have to fix conflicts commit by commit, leading to more complicated operations.

## 4. Applicable Scenarios
- **merge**: Team collaboration, merging public main branches, and scenarios requiring complete preservation of development history.
- **rebase**: Sorting commits on personal development branches and synchronizing personal branches with the latest main branch.
