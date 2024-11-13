
# Git Installation Guide

Follow these steps to install Git on your local system.

---

## Windows

1. **Download Git**:
   - Visit the [Git for Windows](https://gitforwindows.org/) website.
   - Download the latest Git installer for Windows.

2. **Run the Installer**:
   - Open the downloaded `.exe` file.
   - Go through the installation steps, selecting default options unless you have specific preferences.

3. **Configure Git**:
   - After installation, open the Command Prompt or Git Bash.
   - Set up your username and email:
     ```bash
     git config --global user.name "Your Name"
     git config --global user.email "you@example.com"
     ```
   - Verify the installation:
     ```bash
     git --version
     ```

---

## macOS

1. **Using Homebrew** (recommended):
   - If you have Homebrew installed, open the Terminal and run:
     ```bash
     brew install git
     ```

2. **Using Xcode Command Line Tools**:
   - If you prefer not to use Homebrew, you can install Git through Xcode Command Line Tools by running:
     ```bash
     xcode-select --install
     ```

3. **Verify Installation**:
   - Run the following to check Git version:
     ```bash
     git --version
     ```

---

## Linux

1. **Debian/Ubuntu**:
   - Open the Terminal and update your package list:
     ```bash
     sudo apt update
     ```
   - Install Git:
     ```bash
     sudo apt install git
     ```

2. **Fedora**:
   - Open the Terminal and run:
     ```bash
     sudo dnf install git
     ```

3. **Verify Installation**:
   - Check the Git version by running:
     ```bash
     git --version
     ```

---

These steps will install Git on your system. After installation, be sure to configure your Git username and email to start using it effectively.