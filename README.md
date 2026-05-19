# Dr. Chetankumar Patel — Personal Academic Website

## Files in this folder

```
index.html                          ← Main homepage (activities + projects)
patent-portfolio.html               ← Full patent portfolio page (rename your existing index.html)
Patent_Portfolio_UAE_with_Images.docx ← DOCX portfolio (link in site)
projects/
  spine-mobilizer.html              ← Example project page (TEMPLATE)
  breathing-device.html             ← (create by copying template)
  tractor-trolley.html              ← (create by copying template)
  ... one file per project
imgs/
  p1.png, p2.jpg ... p12.png        ← CAD images for patent cards
```

---

## How to publish on GitHub Pages (step by step)

### Step 1 — Create a GitHub account
1. Go to https://github.com
2. Click **Sign up**
3. Enter your email, create a password, choose a username
   - Suggested username: `chetankumarpatel` or `drchetan-patel`
   - Your website will be at: `https://[username].github.io`
4. Verify your email address

### Step 2 — Create a new repository
1. After logging in, click the **+** button (top right) → **New repository**
2. Repository name: type exactly `[yourusername].github.io`
   - Example: if your username is `chetankumarpatel`, name it `chetankumarpatel.github.io`
   - This special name makes it your main GitHub Pages site
3. Set visibility to **Public** (required for free GitHub Pages)
4. Check **Add a README file**
5. Click **Create repository**

### Step 3 — Upload your files
1. In your new repository, click **Add file** → **Upload files**
2. Drag and drop ALL files:
   - `index.html`
   - `patent-portfolio.html`
   - `Patent_Portfolio_UAE_with_Images.docx`
   - The entire `projects/` folder
   - The entire `imgs/` folder
3. Scroll down, type a commit message: `Initial website upload`
4. Click **Commit changes**

   > Note: GitHub does not let you drag a whole folder in one go on some browsers.
   > For folders, click "Add file" → "Upload files" for each folder separately,
   > OR use the GitHub Desktop app (see Step 3b below).

### Step 3b — Upload folders easily (GitHub Desktop)
If you have trouble uploading folders:
1. Download GitHub Desktop from https://desktop.github.com
2. Sign in with your GitHub account
3. Click **Clone a repository** → find your repository → choose a folder on your computer
4. Copy all your website files into that folder
5. In GitHub Desktop you will see all files listed
6. Type a commit message → click **Commit to main** → click **Push origin**

### Step 4 — Enable GitHub Pages
1. In your repository, click **Settings** (top menu)
2. In the left sidebar, click **Pages**
3. Under **Source**, select **Deploy from a branch**
4. Under **Branch**, select **main** and folder **/ (root)**
5. Click **Save**

### Step 5 — Visit your live website
1. Wait 2–5 minutes
2. Go to: `https://[yourusername].github.io`
3. Your website is live!

GitHub will show you the URL in the Pages settings once it's ready.

---

## How to add a new activity (no coding required)

Open `index.html` in any text editor (Notepad, TextEdit, VS Code).

Find this line:
```
const activities = [
```

Add your new activity at the TOP of the list (it will appear first):
```javascript
{ date:'2026-05-18', cat:'workshop', title:'Kids Robotics Workshop — Saturday Session',
  desc:'Describe what happened in 2-3 sentences.',
  location:'RK University Innovation Lab', participants:'25 students',
  tags:['Robotics','Arduino','STEM'] },
```

**Categories available:**
- `workshop` — purple
- `talk` — teal
- `industry` — blue
- `counselling` — green
- `event` — gold
- `research` — red
- `other` — grey

Save the file, then upload it to GitHub (same way as Step 3).
Your website updates automatically within 2–3 minutes.

---

## How to create a new project page

1. Copy `projects/spine-mobilizer.html`
2. Rename it: `projects/your-project-name.html`
3. Open it in a text editor and replace:
   - The `<title>` tag
   - The category pill text
   - The `<h1>` project name
   - The subtitle text
   - The meta chips (patent number, status, etc.)
   - All section content (Problem, Innovation, Methodology, Outcomes, UAE Relevance)
   - The sidebar details (patent number, funding, team)
   - The image paths
   - The project navigation links at the bottom
4. Upload to GitHub

Then add the project to the `projects` array in `index.html` so it shows as a card on the homepage.

---

## Personalise these placeholders

Search and replace in `index.html`:
- `[+91-XXXXXXXXXX]` → your actual phone number
- `[your-profile]` in the LinkedIn link → your LinkedIn username
- `[your-orcid]` → your ORCID number
- `chetanpatel@rku.ac.in` → keep or update your email

---

## Custom domain (optional, later)

If you want `www.drchetan.com` instead of `chetankumarpatel.github.io`:
1. Buy a domain from GoDaddy, Namecheap, or Google Domains (~$10-15/year)
2. In GitHub Pages settings → Custom domain → enter your domain
3. Follow the DNS setup instructions shown

This is completely optional — the `.github.io` address works perfectly.
