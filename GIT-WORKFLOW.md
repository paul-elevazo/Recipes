# Git Workflow Guide for Recipe Repository

This guide provides simple steps for managing your recipe repository with Git.

## 🚀 Simple Git Workflow

### **Daily Recipe Management:**

#### **1. Check Status**
```bash
git status
```
*Shows what files have changed, what's staged, and current branch status*

#### **2. Add Changes**
```bash
git add .
```
*Adds all new/modified files to staging*

**Or add specific files:**
```bash
git add path/to/specific-recipe.md
```

#### **3. Commit Changes**
```bash
git commit -m "Add [recipe name] or Update [recipe name]"
```

**Example commit messages:**
- `"Add slow cooker chicken tikka masala recipe"`
- `"Update beef stew recipe with new cooking times"`
- `"Add vegetarian lasagna to oven-baked section"`

#### **4. Push to GitHub**
```bash
git push
```
*That's it! Your changes are now live on GitHub*

## 📋 Complete Example Workflow

```bash
# 1. Check what's changed
git status

# 2. Add all changes
git add .

# 3. Commit with descriptive message
git commit -m "Add grilled salmon with herb butter recipe"

# 4. Push to GitHub
git push
```

## 🔍 Useful Commands

### **Check Repository Status:**
```bash
git status          # See current changes
git log --oneline   # View recent commits
git branch -vv      # Check branch tracking
```

### **Before Making Changes:**
```bash
git pull           # Get latest changes from GitHub (if working on multiple devices)
```

### **If You Make a Mistake:**
```bash
git reset HEAD~1   # Undo last commit (keeps file changes)
git checkout .     # Discard all uncommitted changes
```

## 🎯 Best Practices

### **Commit Messages:**
- **Be descriptive**: "Add Thai green curry recipe" vs "new recipe"
- **Use action words**: Add, Update, Fix, Remove
- **Include recipe name** when possible

### **When to Commit:**
- ✅ **After adding a new recipe**
- ✅ **After updating cooking times or ingredients**
- ✅ **After organizing/moving recipes**
- ✅ **After fixing typos or formatting**

### **File Organization:**
- Place recipes in appropriate cooking method folders
- Use descriptive filenames: `beef-bourguignon.md` not `recipe1.md`
- Keep consistent formatting using the template in README.md

## 🚨 Troubleshooting

### **If `git push` doesn't work:**
Try the specific push command:
```bash
git push origin main:master
```

### **If you see merge conflicts:**
```bash
git pull           # Pull latest changes first
# Resolve conflicts in files
git add .
git commit -m "Resolve merge conflicts"
git push
```

### **If you accidentally commit the wrong files:**
```bash
git reset --soft HEAD~1    # Undo commit, keep changes staged
git reset HEAD filename    # Unstage specific file
git commit -m "Correct commit message"
```

## 📱 Working Across Multiple Devices

### **Starting work on a new device:**
```bash
git pull    # Get latest recipes from GitHub
```

### **Before adding new recipes:**
```bash
git pull    # Make sure you have latest version
# Add your new recipes
git add .
git commit -m "Add new recipes from [device/location]"
git push
```

---

**Remember:** The repository is set up so `git push` works simply. No complex commands needed for daily use! 🎉
