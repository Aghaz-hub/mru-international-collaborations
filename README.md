# MRU International Collaborations Tracker

**Manav Rachna International Institute of Research and Studies, Faridabad**  
Office of International Affairs & Collaborations

A web-based admin portal to track MoUs, Partner Universities, Academic Arrangements, Global Classrooms, International Mobility and Activities.

---

## Default Admin Login

| Field        | Value            |
|--------------|------------------|
| **Username** | `admin`          |
| **Password** | `mru@oiac2026`   |

> Change these credentials later in `index.html` (search for `ADMIN_USER` and `ADMIN_PASS`).

---

## Project Structure

```
mru-collaborations/
├── index.html          ← Login page (start here)
├── app.html            ← Main Dashboard + all modules
├── README.md           ← This file
├── css/                ← (reserved for future styles)
├── js/                 ← (reserved for future scripts)
└── assets/             ← (put logo or images here if needed)
```

---

## Step-by-Step: Upload to GitHub & Host

### Step 1: Create a new GitHub Repository

1. Go to [https://github.com/new](https://github.com/new)
2. Repository name example: `mru-international-collaborations`
3. Keep it **Public** (required for free GitHub Pages) or Private (if you have GitHub Pro)
4. **Do not** initialize with README (we already have one)
5. Click **Create repository**

### Step 2: Upload the files

**Option A – Using GitHub Website (Easiest)**

1. On the new repository page, click **uploading an existing file**
2. Drag & drop **all files and folders** from the `mru-collaborations` folder
3. Commit message: `Initial commit - MRU Collaborations Tracker`
4. Click **Commit changes**

**Option B – Using Git Command Line**

```bash
cd mru-collaborations
git init
git add .
git commit -m "Initial commit - MRU International Collaborations Tracker"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/mru-international-collaborations.git
git push -u origin main
```

### Step 3: Enable GitHub Pages (Free Hosting)

1. Go to your repository on GitHub
2. Click **Settings** → **Pages** (left sidebar)
3. Under **Source**, select:
   - Branch: `main`
   - Folder: `/ (root)`
4. Click **Save**
5. Wait 1–2 minutes
6. Your site will be live at:

```
https://YOUR-USERNAME.github.io/mru-international-collaborations/
```

### Step 4: Share with Admin

Give the Admin this link + the login credentials:

- **URL**: `https://YOUR-USERNAME.github.io/mru-international-collaborations/`
- **Username**: `admin`
- **Password**: `mru@oiac2026`

---

## How Admin Uses the System

1. Open the website → Login page appears
2. Enter username & password → Click **Sign In**
3. Dashboard opens with:
   - Summary cards (clickable)
   - World map (hover for partner counts)
   - MoUs, Partners, Academic Arrangements, Global Classrooms, Mobility, Activities
4. Use the left sidebar to switch modules
5. Click **Logout** (bottom-right) when finished

---

## Changing Admin Password

1. Open `index.html` in any text editor
2. Find these two lines near the bottom:

```js
const ADMIN_USER = "admin";
const ADMIN_PASS = "mru@oiac2026";
```

3. Change the values
4. Save and re-upload / commit the file to GitHub

---

## Important Notes

- This version stores the **login session** in the browser (localStorage).
- Data currently comes from the embedded Excel data (hard-coded).
- For permanent online data editing (add/edit/delete MoUs by multiple users), a backend (Firebase / Supabase / university server) is recommended later.
- The current system is perfect for **demo, internal review, and single-admin use**.

---

## Next Possible Upgrades

| Feature                        | Difficulty | Notes                          |
|--------------------------------|------------|--------------------------------|
| Real database + multi-user     | Medium     | Use Firebase or Supabase       |
| Upload MoU PDFs                | Medium     | Needs cloud storage            |
| Email alerts for expiring MoUs | Medium     | Needs email service            |
| Role-based access (Viewer/Editor) | Medium  | Extend login system            |
| Mobile responsive improvements | Easy       | Already partially responsive   |

---

## Support

For any changes or new modules, contact the development team / Office of International Affairs.

**© 2026 Manav Rachna International Institute of Research and Studies**
