
### Commands for Key Concepts

#### 1. Initial Git Configuration

- **Set user name and email**:
  ```bash
  git config --global user.name "Your Name"
  git config --global user.email "youremail@example.com"
  ```
  
- **View current configuration**:
  ```bash
  git config --list
  ```

#### 2. Local vs. Remote Repositories

- **Clone a remote repository to local**:
  ```bash
  git clone <repository_url>
  ```

- **Check linked remote repository**:
  ```bash
  git remote -v
  ```

#### 3. Basic Git Architecture

- **Stage changes**:
  ```bash
  git add <file_name>
  ```

- **Commit staged changes**:
  ```bash
  git commit -m "Commit message"
  ```

- **Push commits to the remote repository**:
  ```bash
  git push origin main
  ```

#### 4. Connecting with Remote Repositories

- **Add a new remote repository**:
  ```bash
  git remote add origin <repository_url>
  ```

- **Push to a new remote repository**:
  ```bash
  git push -u origin main
  ```

- **Pull updates from a remote repository**:
  ```bash
  git pull origin main
  ```