
### Day03: Undoing Changes, Stashing, and Reviewing Changes

In **Day03**, we cover essential Git functionalities for managing and reviewing changes effectively:

1. **Undoing Changes**: Safely revert or discard changes in different scenarios.
2. **Stashing**: Temporarily save your work to switch context without committing.
3. **Reviewing Changes**: Analyze uncommitted changes and track the history of commits.

---

#### 1. Undoing Changes

Undoing changes is a critical part of Git workflows. Common scenarios include:

- **Discarding untracked changes**: Revert edits to untracked files.
- **Unstaging files**: Remove files from the staging area.
- **Reverting commits**: Undo a previous commit safely.
- **Resetting branches**: Roll back to a clean state.

##### **Example Scenarios**

1. **Revert to Last Commit for a File**:
   - **Scenario**: You edited `file.txt`, but want to discard the changes and restore the last committed version.
   - **Command**: `git checkout -- file.txt`

2. **Unstage a File**:
   - **Scenario**: You staged `file.txt` but realized it's not ready for commit.
   - **Command**: `git reset file.txt`

3. **Undo the Last Commit (Keep Changes)**:
   - **Scenario**: You made a commit but want to amend it after fixing an issue.
   - **Command**: `git reset --soft HEAD~1`

4. **Undo the Last Commit (Discard Changes)**:
   - **Scenario**: You mistakenly committed broken code and want to discard it entirely.
   - **Command**: `git reset --hard HEAD~1`

5. **Revert a Commit Without Losing History**:
   - **Scenario**: A bug was introduced in commit `abc123`. Revert it without removing other changes.
   - **Command**: `git revert abc123`

---

#### 2. Stashing Changes

Stashing is useful when you need to save unfinished work temporarily without committing.

##### **Example Scenarios**

1. **Save Current Changes**:
   - **Scenario**: You are in the middle of editing files but need to switch to another branch.
   - **Command**: `git stash`

2. **Apply Stashed Changes**:
   - **Scenario**: After switching back to your original branch, you want to continue working on the stashed changes.
   - **Command**: `git stash apply`

3. **Stash Specific Files**:
   - **Scenario**: Only save changes in `file1.txt` and `file2.txt` for later use.
   - **Command**: `git stash push -m "Partial work" file1.txt file2.txt`

4. **Remove Stashed Changes After Applying**:
   - **Scenario**: To keep the stash list clean, drop the applied stash.
   - **Command**: `git stash drop`

5. **Pop and Apply the Latest Stash**:
   - **Scenario**: Apply and delete the stash in one step.
   - **Command**: `git stash pop`

---

#### 3. Reviewing Changes

Reviewing changes helps track progress and history.

##### **Example Scenarios**

1. **View Uncommitted Changes**:
   - **Scenario**: Check what’s modified before committing.
   - **Command**: `git diff`

2. **View Staged Changes**:
   - **Scenario**: Check what’s added to the staging area.
   - **Command**: `git diff --staged`

3. **Show Commit History**:
   - **Scenario**: Review the list of commits with details.
   - **Command**: `git log --oneline`

4. **Compare Two Commits**:
   - **Scenario**: Analyze the differences between two specific commits `abc123` and `def456`.
   - **Command**: `git diff abc123 def456`

---
