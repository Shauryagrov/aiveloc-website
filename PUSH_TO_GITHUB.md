# Push Website to GitHub

## After Creating Repository on GitHub

Run these commands in the `website/` folder:

```bash
cd /Users/madhurgrover/DivinePrayers/website
git remote add origin https://github.com/YOUR_USERNAME/aiveloc-website.git
git push -u origin main
```

**Replace `YOUR_USERNAME` with your actual GitHub username!**

## If You Get Authentication Error

GitHub may ask for authentication. Options:

1. **Use GitHub CLI** (if installed):
   ```bash
   gh auth login
   ```

2. **Use Personal Access Token**:
   - Go to GitHub → Settings → Developer settings → Personal access tokens
   - Generate new token with `repo` permissions
   - Use token as password when pushing

3. **Use SSH** (if you have SSH keys set up):
   ```bash
   git remote set-url origin git@github.com:YOUR_USERNAME/aiveloc-website.git
   git push -u origin main
   ```

