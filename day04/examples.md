
### Day 04: Branching and Merging

In this session, we will dive deep into the following concepts:

1. **Understanding Branches and Their Importance**
   - Branching allows developers to work on features, bug fixes, or experiments in isolation.
   - Common scenarios include feature development, testing, and creating backups.

2. **Merging Branches and Resolving Conflicts**
   - Merging integrates changes from one branch into another, often involving conflict resolution.

3. **Undoing Merge Changes**
   - Revert a merge commit or reset the branch to a pre-merge state.

---

#### 1. Understanding Branches

Branches allow parallel development without affecting the `main` branch or other branches. They are lightweight, starting from a specific commit and evolving independently.

##### **Example Scenarios**

1. **Creating a New Branch**:
   - **Scenario**: Start working on a feature called "new-feature."
   - **Command**: `git branch new-feature`

2. **Switching to a Branch**:
   - **Scenario**: Move to the "new-feature" branch.
   - **Command**: `git checkout new-feature` (or `git switch new-feature`)

3. **Viewing All Branches**:
   - **Scenario**: Check available branches.
   - **Command**: `git branch`

---

#### 2. Merging Branches and Resolving Conflicts

Merging integrates changes from one branch into another. 

##### **Example Scenarios**

1. **Merging Without Conflicts**:
   - **Scenario**: Merge `new-feature` into `main` after finishing the work.
   - **Commands**:
     ```bash
     git checkout main
     git merge new-feature
     ```

2. **Merging With Conflicts**:
   - **Scenario**: Conflicts arise when the same lines of code are edited in both branches.
   - **Steps**:
     - Git highlights conflicting files during the merge.
     - Open the files, resolve the conflicts manually, and mark them as resolved:
       ```bash
       git add <file_name>
       git commit
       ```

---

#### 3. Undoing Merge Changes

Undoing merges helps recover from unintended merges or issues introduced by a merge.

##### **Example Scenarios**

1. **Revert a Merge Commit**:
   - **Scenario**: Undo a problematic merge but keep the branch history.
   - **Command**:
     ```bash
     git revert -m 1 <merge_commit_hash>
     ```

2. **Reset to Pre-Merge State**:
   - **Scenario**: Discard the merge completely.
   - **Command**:
     ```bash
     git reset --hard <commit_before_merge>
     ```

---

#### Example Workflow

1. Create and switch to a feature branch:
   ```bash
   git branch new-feature
   git checkout new-feature
   ```

2. Make changes, add them, and commit:
   ```bash
   git add .
   git commit -m "Implemented feature X"
   ```

3. Merge the feature branch into `main`:
   ```bash
   git checkout main
   git merge new-feature
   ```

4. Handle conflicts if they arise:
   - Edit conflicting files manually.
   - Stage the resolved files:
     ```bash
     git add <file_name>
     ```
   - Commit the resolved merge:
     ```bash
     git commit
     ```

5. Undo a merge if necessary:
   ```bash
   git revert -m 1 <merge_commit_hash>
   ```
---
