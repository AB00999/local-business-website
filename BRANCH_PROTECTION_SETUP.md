# Branch Protection Setup Guide

## Quick Setup Instructions

Your GitHub repository needs branch protection to prevent accidental force pushes and deletions. Follow these steps:

### Step 1: Navigate to Repository Settings
1. Go to: https://github.com/AB00999/local-business-website/settings/rules
2. Click the **"New branch ruleset"** button

### Step 2: Configure Ruleset Name
- **Ruleset name:** `Protect main branch`
- **Description:** `Protects the main branch from force pushes and requires pull requests before merging`
- **Enforcement:** `Active`

### Step 3: Set Target Branches
1. Click on "Branch targeting criteria"
2. Select "Include by pattern"
3. Enter: `main`
4. Click "Add pattern"

### Step 4: Enable Protection Rules
Check/Enable the following rules:

✅ **Restrict creations**
   - Only allow users with bypass permission to create matching refs

✅ **Restrict updates**
   - Only allow users with bypass permission to update matching refs

✅ **Restrict deletions**
   - Only allow users with bypass permissions to delete matching refs

✅ **Block force pushes**
   - Prevent users with push access from force pushing to refs

✅ **Require a pull request before merging**
   - Require all commits be made to a non-target branch and submitted via a pull request before they can be merged
   - Set to 1 (require at least 1 pull request review)

### Step 5: Save
Click the **"Create"** button to save the ruleset.

## What This Protects

- ✅ Prevents accidental deletions of the main branch
- ✅ Prevents force pushes that could lose commit history
- ✅ Requires pull requests for all code changes
- ✅ Maintains code quality and review process
- ✅ Protects your production deployment

## Done!

Once saved, your main branch will be protected. All future commits must be:
1. Made on a separate branch
2. Submitted as a pull request
3. Reviewed before merging (if you enable code review)

This keeps your main branch stable and your website safe! 🚀
