# 🧠 SPS @ COC GitHub Guide  
Welcome to our shared workspace:  
👉 https://github.com/sps-coc

This is where we keep everything organized so we don’t lose files, overwrite each other’s work, or rely on “who has the latest version?”

If it’s official, it lives here.

---

# 🏗 How This Works (Super Simple)

- The `main` branch = the official version of everything  
- Nobody edits `main` directly  
- All changes go through a **Pull Request (PR)**  
- A Maintainer reviews it  
- Then it gets merged  

That’s it.

Think of `main` like the official binder — you don’t write in it directly, you submit changes.

---

# 👥 Roles (What You Can Do)

### 👀 Readers
- View and download files
- Cannot make changes

### ✍️ Contributors
- Can make changes using branches
- Can open Pull Requests
- Cannot merge into `main`

### 🛠 Maintainers
- Review Pull Requests
- Approve and merge changes

### 👑 Owners
- Manage permissions and settings

Most people will be Contributors or Readers.

---

# 📦 Getting Files (Easiest Way)

If you just want access to files:

1. Go to the repo
2. Click the green **Code** button
3. Click **Download ZIP**

Done.

---

# 💻 Making Changes (Recommended Ways)

You have two good options:

---

## ✅ Option A — Use GitHub Website (Easiest)

Best for quick edits like:
- Fixing typos
- Updating minutes
- Adding simple files

### Steps:

1. Go to the file you want to edit  
2. Click the ✏️ (edit) button  
3. Make your changes  
4. At the bottom:
   - Select **“Create a new branch”**  
5. Click **Propose changes**  
6. Click **Create Pull Request**  

Done.

---

## 💻 Option B — Use Git (More Control)

### Step 1 — Install Git

Download: https://git-scm.com/downloads

---

### Step 2 — Clone the repo (one time)

```bash
git clone https://github.com/sps-coc/REPO_NAME.git
cd REPO_NAME
```

### Step 3 - Get latest version

```bash
git pull origin main
```

Always do this before starting work.

### Step 4 - Create a branch

```bash
git checkout -b short-description
```

Example:

```bash
git checkout -b update-meeting-minutes
```

### Step 5 - Make changes

Edit files normally.

### Step 6 - Save changes

```bash
git add .
git commit -m "Updated meeting minutes"
```

### Step 7 - Push your branch

```bash
git push origin short-description
```

### Step 8 - Open a Pull Request

- Go to GitHub
- Click Compare & pull request
- Add a short description
- Submit

### 🔁 What Happens Next?
- A Maintainer reviews your PR
- If everything looks good, it gets approved
- It gets merged into `main`
- Your changes are now official

### ⚠️ Important Rules
- ❌ Do **NOT** edit `main` directly
- ✅ Always use a branch + PR
- ✅ Keep changes small and focused
- ✅ Use clear commit messages

### 🧩 Common Situations
**"I'm out of date"**

Run:
```bash
git pull origin main
```

**"Someone changed the same file as me"**

Yout might get a merge conflict.

This just means Git needs help deciding which version to keep.

Don't panic--ask a Maintainer if unsure.

**"Can I just upload files?"**

Yes.
- Go to repo
- Click **Add file** → **Upload files**
- Commit to a new branch
- Open PR

### 🔐 Public Repo Note

This repository is public, which means:
- Anyone can view it
- Anyone can download it

But:
- Only club members can make changes

🚨 **Do NOT upload sensitive info**

Never put:
- Phone numbers
- Personal emails
- Financial details
- Private documents

Those go in a separate private repo.

### 🧑‍🎓 Officer Transition Rule
When leadership changes:
1. New officers are added
2. Given proper roles
3. Old offiers removed after confirmation
4. Never leave only one Owner

### 🆘 Need Help?
Ask in the club discord or contact a Maintainer.

Everyone starts somewhere--Git feels weird at first, then it clicks.

### 🏁 TL;DR
- Don't touch `main`
- Make a branch
- Open a PR
- Get approval
- Done
