
### Key Concepts

#### 1. Local vs. Remote Repositories

A **local repository** is stored on your machine, containing files and commits you’ve created locally. A **remote repository** is hosted on a server like GitHub or GitLab, allowing for backup, sharing, and collaboration.

**Example Workflow**:
- Clone a remote repository to local.
- Make changes in the local repository, commit them, and push to the remote repository to synchronize updates.

#### 2. Basic Git Architecture

Git’s architecture includes four main areas:

- **Working Directory**: Where you modify files.
- **Staging Area**: Where changes are staged before committing.
- **Local Repository**: Stores committed changes on your machine.
- **Remote Repository**: Stores the shared version of your code on a server.

**Example Workflow**:
1. Make changes in the working directory.
2. Stage files using `git add`.
3. Commit changes with `git commit`.
4. Push changes to the remote repository with `git push`.

---

### Detailed Git Architecture

```
                     ┌──────────────────────────────────────────┐
                     │          Remote Repository               │
                     │  (e.g., GitHub, GitLab, Bitbucket)       │
                     └──────────────────────────────────────────┘
                                       ▲
                                       │
                           git push     │     git pull
                                       │
                     ┌──────────────────────────────────────────┐
                     │          Local Repository                │
                     │ (Your committed changes, all versions)   │
                     └──────────────────────────────────────────┘
                                       ▲
                                       │
                          git commit   │    git reset
                                       │
                     ┌──────────────────────────────────────────┐
                     │           Staging Area                  │
                     │ (Files prepared for commit, snapshots)  │
                     └──────────────────────────────────────────┘
                                       ▲
                                       │
                          git add      │    git reset
                                       │
                     ┌──────────────────────────────────────────┐
                     │          Working Directory              │
                     │ (Your local files and current changes)  │
                     └──────────────────────────────────────────┘
```
