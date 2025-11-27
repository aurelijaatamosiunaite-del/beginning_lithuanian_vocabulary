# Step-by-Step Guide: Setting Up PWA Version on GitHub

## STEP 1: Download the PWA Files

You should have these files:
- index.html
- manifest.json
- service-worker.js
- icon-192.png
- icon-512.png
- README.md

## STEP 2: Create a New Branch in Your Existing Repository

### Option A: Using GitHub Website (EASIER)

1. Go to your repository: `https://github.com/YOUR-USERNAME/YOUR-REPO-NAME`

2. Click the branch dropdown (says "main" or "master")

3. Type a new branch name: `pwa-version`

4. Click "Create branch: pwa-version"

5. You're now on the new branch!

6. Click "Add file" → "Upload files"

7. Drag and drop ALL the PWA files (or click to select them)

8. Scroll down, add commit message: "Add PWA version"

9. Click "Commit changes"

### Option B: Using Git Command Line (if you're comfortable)

```bash
# Clone your repository (if not already)
git clone https://github.com/YOUR-USERNAME/YOUR-REPO-NAME
cd YOUR-REPO-NAME

# Create new branch
git checkout -b pwa-version

# Copy the PWA files to this folder

# Add files
git add .

# Commit
git commit -m "Add PWA version"

# Push to GitHub
git push origin pwa-version
```

## STEP 3: Enable GitHub Pages for the PWA Branch

1. Go to your repository on GitHub

2. Click "Settings" (top right)

3. Scroll down to "Pages" in the left sidebar

4. Under "Source":
   - Branch: Select `pwa-version`
   - Folder: Select `/ (root)`

5. Click "Save"

6. Wait 1-2 minutes

7. Your PWA will be live at:
   `https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/`

## STEP 4: Test the PWA

### On Your Phone:

1. Open the URL in your phone's browser

2. **Android (Chrome):**
   - Look for "Add to Home screen" popup
   - Or tap menu (⋮) → "Add to Home screen"

3. **iPhone (Safari):**
   - Tap Share button (⬆️)
   - Scroll down, tap "Add to Home Screen"

4. Tap the new icon on your home screen - it should open like a real app!

### On Desktop:

1. Open the URL in Chrome or Edge

2. Look for install icon in address bar

3. Click it to install

## STEP 5: Keep Both Versions!

Now you have:
- **main branch**: Your original HTML version (safe backup!)
- **pwa-version branch**: New PWA version to test

You can switch between them on GitHub by clicking the branch dropdown.

## STEP 6: Share with Students

Give students this link:
`https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/`

Tell them:
1. Open the link
2. When prompted, tap "Add to Home Screen" or "Install"
3. Use the app icon on their home screen

## Updating the PWA Later

When you want to update:

1. Switch to `pwa-version` branch on GitHub
2. Edit the files you want to change
3. Commit the changes
4. GitHub Pages will auto-update (takes 1-2 minutes)
5. Students just need to refresh or close/reopen the app

## Troubleshooting

**"I don't see the install prompt!"**
- Make sure you're using HTTPS (GitHub Pages does this automatically)
- Try visiting the page 2-3 times
- Try a different browser

**"The app won't update!"**
- In service-worker.js, change `v1` to `v2` in CACHE_NAME
- This forces all devices to download the new version

**"I want to go back to the HTML version!"**
- Just switch to the `main` branch on GitHub
- Or delete the `pwa-version` branch entirely (safe - your main branch is untouched)

## Safety Notes

✅ Your original code in `main` branch is NEVER touched
✅ You can delete the `pwa-version` branch anytime
✅ You can keep both versions running simultaneously at different URLs
✅ Students can use whichever version they prefer

---

## Quick Reference: GitHub Pages URLs

If you keep both:
- HTML version: `https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/` (from main branch)
- PWA version: Create a separate repo OR use subfolders

**Better approach for 2 versions:**
Keep them in SEPARATE repositories:
- Repo 1: `lithuanian-vocab-html` (main branch only)
- Repo 2: `lithuanian-vocab-pwa` (pwa version)

This way each has its own URL and they don't interfere!
