### Day 06: Best Practices & Review

#### Best Practices

1. **Create a `.gitignore` File**:
   ```bash
   touch .gitignore
   echo "node_modules/" >> .gitignore
   ```

2. **Check for Sensitive Data in History**:
   ```bash
   git log -S <keyword>
   ```

3. **Use Rebase to Clean Commit History**:
   ```bash
   git checkout feature-branch
   git rebase main
   ```

4. **Tagging a Release**:
   ```bash
   git tag -a v1.0 -m "Version 1.0 release"
   git push origin v1.0
   ```

---

#### Clean Workflows

1. **Feature Branch Creation**:
   ```bash
   git checkout -b <feature_branch>
   ```

2. **Pull Latest Changes from `main`**:
   ```bash
   git checkout main
   git pull origin main
   ```

3. **Rebase with Main Branch**:
   ```bash
   git checkout <feature_branch>
   git rebase main
   ```

4. **Merge Feature Branch**:
   ```bash
   git checkout main
   git merge <feature_branch>
   ```

---