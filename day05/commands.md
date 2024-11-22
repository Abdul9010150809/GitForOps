
### Day 05: Collaboration & Pull Requests

#### Pull Requests

1. **Fork a Repository** (via GitHub UI).

2. **Clone a Forked Repository**:
   ```bash
   git clone <forked_repository_url>
   ```

3. **Add an Upstream Remote**:
   ```bash
   git remote add upstream <original_repository_url>
   ```

4. **Create a New Branch**:
   ```bash
   git checkout -b <branch_name>
   ```

5. **Push Changes to Your Branch**:
   ```bash
   git push origin <branch_name>
   ```

6. **Open a Pull Request**:
   - Navigate to **Pull Requests** on the original repository and click **New Pull Request**.

7. **Sync Fork with Upstream Changes**:
   ```bash
   git fetch upstream
   git checkout main
   git merge upstream/main
   ```

---

#### Issues and Discussions

1. **Open a New Issue** (via GitHub UI):
   - Navigate to the **Issues** tab and click **New Issue**.

2. **Comment on an Existing Issue**:
   - Use the GitHub UI to add comments or solutions.

3. **Start a Discussion** (via GitHub UI):
   - Go to the **Discussions** tab and click **New Discussion**.

---

#### Code Reviews and Contributions

1. **Review a Pull Request** (via GitHub UI):
   - Navigate to the PR and leave inline comments or approve the changes.

2. **Check Out a Pull Request Locally**:
   ```bash
   git fetch origin pull/<PR_number>/head:<local_branch_name>
   git checkout <local_branch_name>
   ```

3. **Resolve Merge Conflicts**:
   ```bash
   git merge <conflicting_branch>
   # Resolve conflicts in files manually.
   git add <resolved_file>
   git commit
   ```

---
