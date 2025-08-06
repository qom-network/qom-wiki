---
title: GitHub Guide For Beginners (With GitHub SSH Setup)
type: docs
prev: 
next: 
sidebar:
  open: true
---


This guide will walk you through:

1. Creating a GitHub account
    
2. Hiding your email
    
3. Creating an SSH key and connecting it to GitHub
    
4. Forking someone else's repository
    
5. Cloning it to your `Desktop` folder on your local machine
    

---

## 📝 Step 1: Create a GitHub Account

1. Go to [https://github.com](https://github.com)
    
2. Click on **Sign up**
    
3. Enter the required info:
    
    - **Username**
        
    - **Email address**
        
    - **Password**
        
4. Confirm your email via the link sent to you
    

---

## 🔒 Step 2: Make Your Email Private on GitHub

1. Click your profile picture → **Settings**
    
2. Go to **Emails** in the sidebar
    
3. Check these options:
    
    - ✅ **Keep my email address private**
        - Store your email address "123456789+YourUserName@users.noreply.github.com"
        
    - ✅ **Block command line pushes that expose my email**
    

---

## 💻 Step 3: Install Git (if not already installed)

- **macOS**: Open Terminal and run:
```bash
git --version
```
- If not installed, you’ll be prompted to install Git.
    
- **Windows**: Download and install Git from [https://git-scm.com](https://git-scm.com)


---

## 🔐 Step 4: Generate SSH Key and Register with GitHub

### ① Open Terminal or Git Bash and run:

```bash
ssh-keygen -t ed25519 -C "123456789+YourUserName@users.noreply.github.com"
```

- Replace `123456789+YourUserName@users.noreply.github.com` with the email you used for GitHub
    
- Press Enter to accept default file location
    
- You can press Enter to skip passphrase (optional)


### ② View and copy the public key:

```bash
cat ~/.ssh/id_ed25519.pub
```

- Copy the full output.

### ③ Add SSH key to GitHub:

1. Go to GitHub → **Settings** → **SSH and GPG keys**
    
2. Click **New SSH key**
    
3. Title: e.g. “My Laptop”
    
4. Paste your copied key
    
5. Click **Add SSH key**


---

## ⚙️ Step 5: Configure Your Git User Info

```bash
git config --global user.name "Your GitHub Username" 
git config --global user.email "123456789+YourUserName@users.noreply.github.com"
```

> Tip: If your email is private, use your `123456789+YourUserName@users.noreply.github.com` GitHub-provided email (See Step2)

---

## 🔁 Step 6: Fork a Repository on GitHub

1. Find the repository you want to fork
    
2. Click the **Fork** button (top-right)
    
3. It will create a copy under your GitHub account


---

## 📥 Step 7: Clone Your Fork to Your Desktop (Using SSH)

### ① Go to your forked repository on GitHub

### ② Click the **Code** button → Choose **SSH** → Copy the SSH URL

Example: `git@github.com:yourusername/reponame.git`

### ③ Open Terminal and run:

```bash
cd desktop
git clone git@github.com:yourusername/reponame.git
```

**If you initially cloned using HTTPS and want to switch to SSH later, please follow the steps below to make the change.**


#### 🔄 Change the GitHub Repository Remote URL from HTTPS to SSH

✅ **Check Your Current Remote URL**
First, confirm whether your current remote URL is using HTTPS:


```bash
git remote -v


#Example output (if using HTTPS):
origin  https://github.com/your-username/your-repo.git (fetch)
origin  https://github.com/your-username/your-repo.git (push)
```

🔁 **Change Remote URL to SSH**
If you're using HTTPS, switch to SSH by running the following command:

```bash
git remote set-url origin git@github.com:your-username/your-repo.git
```

Replace `your-username` and `your-repo` with your actual GitHub username and repository name.

For example, if your username is BabelFish and the repository is hello-world, you would run:

```bash
git remote set-url origin git@github.com:BabelFish/hello-world.git
```

✅ **Verify the Change**
To make sure the change was successful, run:

```bash
git remote -v

#You should see something like:
origin  git@github.com:BabelFish/hello-world.git (fetch)
origin  git@github.com:BabelFish/hello-world.git (push)
```

---

## ✅ Done!

You now have:

- GitHub account ✔️
    
- Email privacy set ✔️
    
- SSH key authentication set up ✔️
    
- A fork of the repo under your account ✔️
    
- The repo cloned to your Desktop ✔️
