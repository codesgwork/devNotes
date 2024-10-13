To set global user settings for Git, you need to configure your username and email address, which will be associated with your commits. Here’s how you can set these global configurations:

## Steps to Set Global Git User Settings:

#### 1. **Open Git Bash** or any terminal on your system.

#### 2. Use the following commands to set your username and email globally. Replace `"Your Name"` and `"youremail@example.com"` with your actual details:

- Set global username:

  ```bash
  git config --global user.name "Your Name"
  ```

- Set global email:
  ```bash
  git config --global user.email "youremail@example.com"
  ```

#### 3. You can check if the settings have been applied correctly by running:

```bash
git config --global --list
```

This command will display the global configurations, including your username and email.

Of course! Here's a **summary note** for your reference on troubleshooting and setting up SSH keys for GitHub:

---

## **Summary: SSH Key Setup and Troubleshooting for GitHub**

#### 1. **Generate an SSH Key (if not already generated):**

```bash
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```

- Press **Enter** to save the key in the default location (`~/.ssh/id_rsa`).
- Optionally, set a passphrase for added security.

#### **Add SSH Key to SSH Agent:**

- Start the SSH agent:
  ```bash
  eval "$(ssh-agent -s)"
  ```
- Add your SSH private key to the agent:
  ```bash
  ssh-add ~/.ssh/id_rsa
  ```

#### **Add SSH Key to GitHub:**

- Copy your public SSH key:
  ```bash
  cat ~/.ssh/id_rsa.pub
  ```
- Go to **GitHub** > **Settings** > **SSH and GPG keys** > **New SSH key**.
- Paste the copied key and save.

#### **Configure SSH for GitHub (for multiple git account):**

- Edit `~/.ssh/config` (create if it doesn't exist):
  ```bash
  Host github.com
    HostName github.com
    User git
    IdentityFile ~/.ssh/id_rsa
  ```

#### **Test the SSH Connection:**

- Run the following command to test:
  ```bash
  ssh -T git@github.com
  ```
- Expected output (if successful):
  ```bash
  Hi your-username! You've successfully authenticated, but GitHub does not provide shell access.
  ```

#### **Cloning a GitHub Repository Using SSH:**

- Use the correct SSH URL format:
  ```bash
  git clone git@github.com:your-username/repository.git
  ```

#### **Verbose SSH Debugging (If Needed):**

- For troubleshooting SSH connection issues, use the verbose flag:
  ```bash
  ssh -vT git@github.com
  ```

---

This should cover all the necessary steps for setting up and troubleshooting SSH keys with GitHub. You can keep this for future reference to quickly resolve any similar issues.

Let me know if you need anything else!
