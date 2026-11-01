# Deployment Guide: Suon Lysorng's GitHub Pages & Profile

This guide explains how to publish your personal academic & industry website to **GitHub Pages** (just like `https://luboshanus.github.io/`) and set up your **GitHub Profile README**.

---

## Part 1: Deploying Your Personal Website (`lysorngsuon.github.io`)

Your website is located in this folder:
`C:\02 DASLY\Finance Learning\Cambodia SME Financial Intelligence\Lysorngsuon\lysorngsuon.github.io`

### Step 1: Create the GitHub Repository
1. Log in to your GitHub account: **[github.com/Lysorngsuon](https://github.com/Lysorngsuon)**.
2. Click the **`+`** icon in the top right corner and select **New repository**.
3. Name the repository exactly:
   ```
   Lysorngsuon.github.io
   ```
   *(GitHub specifically recognizes this naming convention to host your personal user website at `https://lysorngsuon.github.io/`).*
4. Ensure the repository is set to **Public**.
5. Do **not** initialize with a README, .gitignore, or license (we already have all files ready).
6. Click **Create repository**.

### Step 2: Push Your Website Files to GitHub
Open your terminal (PowerShell or Command Prompt) and run:

```powershell
# 1. Navigate to the website folder
cd "C:\02 DASLY\Finance Learning\Cambodia SME Financial Intelligence\Lysorngsuon\lysorngsuon.github.io"

# 2. Initialize git repository
git init

# 3. Add all files
git add .

# 4. Commit files
git commit -m "Initial release of personal academic and industry website"

# 5. Set main branch and link to GitHub
git branch -M main
git remote add origin https://github.com/Lysorngsuon/Lysorngsuon.github.io.git

# 6. Push to GitHub
git push -u origin main
```

### Step 3: Verify GitHub Pages Settings
1. Go to your repository on GitHub: `https://github.com/Lysorngsuon/Lysorngsuon.github.io`.
2. Click **Settings** (tab at the top) &rarr; **Pages** (in the left sidebar).
3. Under **Build and deployment**:
   - **Source**: `Deploy from a branch`
   - **Branch**: `main` / `/ (root)`
4. Click **Save**.
5. Within 1 to 2 minutes, your website will be live at:
   👉 **`https://lysorngsuon.github.io/`**

---

## Part 2: Setting Up Your GitHub Profile README (`github.com/Lysorngsuon`)

GitHub allows you to showcase a customized profile on your main GitHub landing page (`https://github.com/Lysorngsuon`).

### Step 1: Create the Special Profile Repository
1. On GitHub, create a new repository named exactly:
   ```
   Lysorngsuon
   ```
   *(GitHub displays a special banner: "✨ You found a secret! Lysorngsuon/Lysorngsuon is a special repository...").*
2. Set it to **Public**.
3. Check the box **Add a README file**.
4. Click **Create repository**.

### Step 2: Copy the Profile README
1. Open the file `github-profile-README.md` located in this folder:
   `C:\02 DASLY\Finance Learning\Cambodia SME Financial Intelligence\Lysorngsuon\lysorngsuon.github.io\github-profile-README.md`
2. Copy its entire contents.
3. In your new `Lysorngsuon` repository on GitHub, edit `README.md`, paste the content, and click **Commit changes**.
4. Your main GitHub profile page at `https://github.com/Lysorngsuon` will now display your professional bio, tech badges, publications, and direct links to your live website!

---

## Part 3: Previewing the Website Locally
You can preview the website immediately on your computer before publishing:
1. Double-click `index.html` inside `C:\02 DASLY\Finance Learning\Cambodia SME Financial Intelligence\Lysorngsuon\lysorngsuon.github.io\index.html`.
2. It will open in your default browser (Chrome, Edge, etc.) with all styling, photos, and features active.

