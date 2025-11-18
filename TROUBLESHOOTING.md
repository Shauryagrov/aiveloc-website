# Troubleshooting: Website Not Updating

## Quick Fixes

### 1. Clear Browser Cache (Most Common Issue)

**Chrome/Edge:**
- Press `Ctrl+Shift+Delete` (Windows) or `Cmd+Shift+Delete` (Mac)
- Select "Cached images and files"
- Time range: "All time"
- Click "Clear data"

**Safari:**
- Press `Cmd+Option+E` to clear cache
- Or: Safari → Preferences → Advanced → "Show Develop menu"
- Then: Develop → Empty Caches

**Firefox:**
- Press `Ctrl+Shift+Delete` (Windows) or `Cmd+Shift+Delete` (Mac)
- Select "Cache"
- Click "Clear Now"

### 2. Hard Refresh (Force Reload)

**Windows:**
- `Ctrl + F5` or `Ctrl + Shift + R`

**Mac:**
- `Cmd + Shift + R` or `Cmd + Option + R`

### 3. Check GitHub Pages Status

1. Go to: https://github.com/Shauryagrov/aiveloc-website/settings/pages
2. Verify:
   - Source: `main` branch, `/ (root)` folder
   - Status shows "Your site is live at..."
   - If not enabled, enable it and wait 2-3 minutes

### 4. Check if Files Are on GitHub

1. Go to: https://github.com/Shauryagrov/aiveloc-website
2. Verify `index.html` shows the new content (Aiveloc company site)
3. If it shows old content, files weren't pushed correctly

### 5. Force GitHub Pages to Rebuild

**Method 1: Make a small change**
- Edit any file (add a space)
- Commit and push
- This triggers a rebuild

**Method 2: Check Actions tab**
- Go to: https://github.com/Shauryagrov/aiveloc-website/actions
- See if there are any build errors

### 6. Check DNS/URL

**If using GitHub Pages URL:**
- Visit: `https://shauryagrov.github.io/aiveloc-website/`
- Add `?v=2` to force refresh: `https://shauryagrov.github.io/aiveloc-website/?v=2`

**If using custom domain (aiveloc.com):**
- DNS might be cached
- Try: `https://aiveloc.com/?v=2`
- Wait 5-30 minutes for DNS propagation

### 7. Verify Files Are Correct

Check that `index.html` on GitHub contains:
- "Aiveloc" (not "DivinePrayers")
- "AI-Powered Apps. Human Expertise."
- Apps section with all 3 apps

If it doesn't, the files weren't pushed correctly.

## Still Not Working?

1. **Check GitHub repository directly:**
   - https://github.com/Shauryagrov/aiveloc-website/blob/main/index.html
   - Does it show the new content?

2. **Try incognito/private window:**
   - This bypasses cache completely
   - If it works in incognito, it's a cache issue

3. **Check GitHub Pages build:**
   - Settings → Pages → Check "View deployment" or "Visit site"
   - This shows the actual deployed version

4. **Wait a few minutes:**
   - GitHub Pages can take 1-5 minutes to update
   - After enabling, wait and try again

