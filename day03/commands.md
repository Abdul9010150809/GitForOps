
### Day03: Undoing Changes, Stashing, and Reviewing Changes

#### Undoing Changes

1. **Revert a File to the Last Committed State**:
   ```bash
   git checkout -- <file_name>
   ```

2. **Unstage a Staged File**:
   ```bash
   git reset <file_name>
   ```

3. **Undo the Last Commit (Keep Changes)**:
   ```bash
   git reset --soft HEAD~1
   ```

4. **Undo the Last Commit (Discard Changes)**:
   ```bash
   git reset --hard HEAD~1
   ```

5. **Revert a Specific Commit**:
   ```bash
   git revert <commit_hash>
   ```

6. **Reset a Branch to a Specific Commit**:
   ```bash
   git reset --hard <commit_hash>
   ```

#### Stashing Changes

1. **Save All Current Changes**:
   ```bash
   git stash
   ```

2. **List All Stashes**:
   ```bash
   git stash list
   ```

3. **Apply the Latest Stash**:
   ```bash
   git stash apply
   ```

4. **Stash Specific Files**:
   ```bash
   git stash push -m "Message" <file1> <file2>
   ```

5. **Pop the Latest Stash**:
   ```bash
   git stash pop
   ```

6. **Drop a Specific Stash**:
   ```bash
   git stash drop stash@{0}
   ```

#### Reviewing Changes

1. **Show Uncommitted Changes**:
   ```bash
   git diff
   ```

2. **Show Staged Changes**:
   ```bash
   git diff --staged
   ```

3. **View Commit History**:
   ```bash
   git log
   ```

4. **Show a Specific Commit**:
   ```bash
   git show <commit_hash>
   ```

5. **Compare Two Commits**:
   ```bash
   git diff <commit_hash_1> <commit_hash_2>
   ```

6. **View a File's History**:
   ```bash
   git log -- <file_name>
   ```

---