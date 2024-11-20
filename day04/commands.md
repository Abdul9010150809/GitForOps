
### Day 04: Branching and Merging

#### Branching

1. **Create a New Branch**:
   ```bash
   git branch <branch_name>
   ```

2. **Switch to a Branch**:
   ```bash
   git checkout <branch_name>  # Older style
   git switch <branch_name>    # Modern style
   ```

3. **View All Branches**:
   ```bash
   git branch
   ```

4. **Delete a Branch**:
   ```bash
   git branch -d <branch_name>   # Safe delete
   git branch -D <branch_name>   # Force delete
   ```

---

#### Merging

1. **Merge a Branch**:
   ```bash
   git checkout <target_branch>
   git merge <source_branch>
   ```

2. **View Merge Conflicts**:
   ```bash
   git status
   ```

3. **Mark Conflict as Resolved**:
   ```bash
   git add <file_name>
   git commit
   ```

4. **Abort a Merge**:
   ```bash
   git merge --abort
   ```

---

#### Undoing Merge Changes

1. **Revert a Merge Commit**:
   ```bash
   git revert -m 1 <merge_commit_hash>
   ```

2. **Reset to Pre-Merge State**:
   ```bash
   git reset --hard <commit_before_merge>
   ```

3. **Restore Deleted Branch After a Merge**:
   ```bash
   git checkout -b <branch_name> <commit_hash>
   ```

---