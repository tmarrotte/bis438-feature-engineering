# BIS 438 Feature Engineering Lab - Setup Guide

**Course:** BIS 438
**Lab:** Part 1 - Customer Churn Feature Engineering  
**Duration:** 60 minutes  
**Difficulty:** Beginner-friendly (no coding experience required!)

---

## What You'll Do

In this lab, you'll learn how to prepare raw customer data for machine learning by:
- Cleaning messy data
- Handling missing values
- Creating new features
- Encoding categories for ML models

**All instructions are in the notebook** - this guide just helps you get set up!

---

## ⚠️ IMPORTANT: First-Time Setup Tips

**Before you start:**

1. **Be Patient:** First-time setup takes 2-3 minutes. Wait for "Codespace ready" before doing anything!

2. **Free Tier Limits:** GitHub gives you 120 FREE hours/month of Codespaces (plenty for this 60-minute lab)
   - Your Codespace auto-stops after 30 minutes of inactivity
   - You can manually stop/delete it when done to save hours
   - See "Troubleshooting" section below for instructions

3. **Your Work is Saved:** Codespaces auto-saves everything in the cloud
   - Close the browser anytime - your progress is preserved
   - Come back later by reopening your Codespace from GitHub

4. **Each Student Gets Their Own:** You have your own isolated environment
   - Your instructor cannot see or access your Codespace
   - You cannot share a Codespace with classmates
   - Each person must create their own

**Ready?** Follow the steps below to get started!

---

## Setup Instructions

### Prerequisites
- A GitHub account (free) - [Sign up here](https://github.com/signup) if needed

---

## Step 1: Access the Lab Repository

Your instructor has provided a GitHub repository link. It should look like:
```
https://github.com/[instructor-username]/bis438-feature-engineering-lab
```

Click the link to open the repository.

---

## Step 2: Launch GitHub Codespaces

GitHub Codespaces creates a cloud-based coding environment that runs in your browser. Everything is pre-configured!

### Instructions:

1. **Click the green `<> Code` button** at the top right of the repository page

2. **Select the "Codespaces" tab** (next to "Local")

3. **Click "Create codespace on main"**
   - If you see an existing Codespace listed, click on it to reopen
   - First-time setup takes 2-3 minutes (be patient!)

4. **⚠️ WAIT for the environment to fully load** (this is important!)
   - You'll see a VS Code interface in your browser
   - Look at the **bottom-right corner** for status messages:
     - "Setting up Codespace..." 
     - "Installing Python packages..."
     - "Codespace ready" ✅
   - **Do NOT open the notebook or run any cells until you see "Codespace ready"**
   - This usually takes 2-3 minutes on first launch

### What's Happening?
Codespaces is:
- Creating a virtual computer in the cloud (15 seconds)
- Installing Python 3.13 (30 seconds)
- Installing all required libraries: pandas, numpy, matplotlib, etc. (90 seconds)
- Loading your lab files (10 seconds)
- Setting up Jupyter notebook support (15 seconds)

**Total:** ~2-3 minutes. Grab a coffee! ☕

### How do I know it's ready?
- ✅ Bottom-right says "Codespace ready" or shows no installation messages
- ✅ You can see files in the left sidebar
- ✅ No loading spinners in the status bar

---

## Step 3: Open the Lab Notebook

Once Codespaces is ready:

1. **Look at the file explorer** on the left sidebar

2. **Find and click on:** `feature_engineering_lab.ipynb`
   - This is your interactive lab notebook
   - It contains all instructions and code

3. **Wait for the notebook to open**
   - You'll see cells with text and code
   - May take 10-15 seconds on first open

4. **Select a Python kernel** (you'll be prompted automatically):
   - Click "Select Kernel" in the top right (or it may pop up automatically)
   - Choose **"Python 3.13.x"** from the list
   - Look for the option that shows **/usr/local/bin/python**
   - This connects your notebook to Python so it can run code

**✅ Kernel Selected?** You should see "Python 3.13.x" in the top-right corner of the notebook.

### What is a "Kernel"?
Think of it as the "engine" that runs your Python code. You're selecting which version of Python to use. We're using Python 3.13 for this lab.

---

## Step 4: Start the Lab!

You're ready to begin!

### How to Use the Notebook:

- **Read the markdown cells** (text explanations) carefully
- **Run code cells** by clicking on them and pressing **Shift + Enter**
- **Run cells in order** from top to bottom (later cells depend on earlier ones)
- **Complete the "YOUR TURN" exercises** as you go

### First Action:
1. Click on the **first code cell** (imports libraries)
2. Press **Shift + Enter** to run it
3. You should see: "Libraries loaded successfully!"

If you see that message, you're all set!

---

## What's in This Repository?

```
Repository Contents
├── README.md ← You are here (setup guide)
├── feature_engineering_lab.ipynb ← START HERE (your lab)
├── customer_data.csv (customer data - don't open directly)
├── requirements.txt (Python packages - auto-installed)
└── .devcontainer/ (Codespaces config - ignore this)
```

**You only need to work with:** `feature_engineering_lab.ipynb`

Everything else happens automatically!


---

## Troubleshooting

### ⚠️ IMPORTANT: Wait for Setup to Complete!

When you first create a Codespace, **wait 2-3 minutes** for the setup to complete:
- Look at the **bottom-right corner** for status messages
- You'll see "Setting up Codespace..." then "Installing Python packages..."
- **Do not run any notebook cells** until you see "Codespace ready"
- If you try to run cells too early, you may get "ipykernel not found" errors

### Issue: "Codespace failed to create"
**Solution:** 
- Refresh the page and try again
- Make sure you're logged into GitHub
- Check if you have available Codespace hours (free tier: 120 hours/month)
- Try clearing your browser cache and restarting

### Issue: "Kernel not found" or "ipykernel not available"
**Solution - Method 1 (Preferred):**
1. **Wait!** Codespaces may still be installing packages (check bottom status bar)
2. Once setup is complete, click "Select Kernel" in the top right of the notebook
3. Choose **"Python 3.13.x"** (should match your environment)
4. Look for the option with **/usr/local/bin/python** in the path
5. Click it and wait for the kernel to connect

**Solution - Method 2 (If Method 1 doesn't work):**
1. Close the notebook file
2. Open a new terminal: `Terminal` → `New Terminal` from the top menu
3. Run: `pip install ipykernel jupyter`
4. Wait for installation to complete (30-60 seconds)
5. Reopen the notebook: click `feature_engineering_lab.ipynb` in the file explorer
6. Select the Python 3.13 kernel when prompted

### Issue: "Module not found" error when running code (e.g., pandas, numpy)
**Cause:** Python packages didn't install automatically, or you selected the wrong kernel.

**Solution:**
1. Check which kernel is selected (look at top-right of notebook)
   - Should say "Python 3.13.x" or similar
   - If it says something else, click it and select the Python 3.13 option
2. Open a new terminal: `Terminal` → `New Terminal` from the top menu
3. Verify Python version: `python --version` (should be 3.13.x)
4. Reinstall packages: `pip install --no-cache-dir -r requirements.txt`
5. Wait for installation to complete (1-2 minutes)
6. Restart the kernel: Click the ↻ icon at the top of the notebook
7. Try running the first cell again

### Issue: Code cells won't run / nothing happens when I press Shift+Enter
**Solution:**
1. Check if kernel is connected (top-right should show "Python 3.13.x")
2. If disconnected, click "Select Kernel" and choose Python 3.13
3. If kernel is busy (spinning icon), wait for current cell to finish
4. Try restarting the kernel: Click ↻ icon at top of notebook

### Issue: Lost your work?
**Don't worry!** Codespaces automatically saves your changes. Your work is stored in the cloud.
- Every time you edit and run cells, changes are saved automatically
- Your `.pkl` files are saved in your Codespace storage
- Close the browser anytime - your work persists

### Issue: Need to pause and come back later?
**No problem!** 
- Codespaces auto-saves your work continuously
- Just close the browser tab - your Codespace will auto-stop after 30 minutes of inactivity
- To resume: Go back to the GitHub repository → Code → Codespaces → Click your existing Codespace
- Your progress will be exactly where you left off (notebook outputs, variables, `.pkl` files all preserved)

### Issue: How do I stop/delete my Codespace to save hours?

**To Stop (Pause) Your Codespace:**
1. Go to https://github.com/codespaces
2. Find your `bis438-feature-engineering-lab` Codespace
3. Click the **three dots (...)** on the right
4. Select **"Stop codespace"**
5. Your work is saved - you can restart it later

**To Delete Your Codespace (after lab is complete):**
1. Go to https://github.com/codespaces
2. Find your `bis438-feature-engineering-lab` Codespace
3. Click the **three dots (...)** on the right
4. Select **"Delete"**
5. ⚠️ **Warning:** This permanently deletes all your work! Only do this if you've submitted your lab.

**Managing Your Free Hours:**
- Free tier: 120 hours/month (plenty for this lab!)
- This lab takes ~60 minutes to complete
- Codespaces auto-stop after 30 minutes of inactivity (doesn't waste your hours)
- Check remaining hours: https://github.com/settings/billing

### Issue: Notebook outputs disappeared when I reopened
**Cause:** This is normal! Notebook outputs are not saved in your Codespace by default.

**Solution:**
- Run the cells again to regenerate outputs
- Your saved `.pkl` files are still there (run the loading cells to restore your work)
- To preserve outputs: Use "Export" → "Export as PDF/HTML" from the `...` menu in notebook toolbar

### Issue: Can I work on this from multiple computers?
**Yes!** Your Codespace lives in the cloud:
1. Open the GitHub repository from any computer
2. Go to Code → Codespaces → Click your existing Codespace
3. Continue where you left off
4. All your work, packages, and files are preserved

---

## Tips for Success

### Do's
- **Read carefully** - Instructions are in the notebook
- **Run cells in order** - Top to bottom, don't skip
- **Experiment** - Try changing values and see what happens
- **Ask questions** - Raise your hand if stuck
- **Save frequently** - Use `Ctrl+S` (Windows) or `Cmd+S` (Mac)

### Don'ts
- Don't skip cells - they build on each other
- Don't edit the CSV file directly - work in the notebook
- Don't worry about making mistakes - you can always restart!

---

## Time Expectations

- **Environment setup:** 2-3 minutes (one time)
- **Lab completion:** 60 minutes
- **Total:** ~65 minutes

The lab is designed to be completed in one class period.

---

## What Happens Next?

### During the Lab:
1. Complete all code cells in the notebook
2. Answer embedded questions as you go
3. Take note of interesting findings

### After the Lab:
- Your instructor will provide reflection questions
- You may be asked to submit your completed notebook
- Part 2 (Model Training) will build on this work

---

## Getting Help

**If you're stuck:**
1. Read the markdown text above the cell carefully
2. Check the hints in code comments (lines starting with `#`)
3. Ask a classmate sitting near you
4. Raise your hand for instructor help
5. Check the troubleshooting section above

**Remember:** Everyone gets stuck sometimes. That's part of learning!

---

## Ready to Begin?

1. GitHub account created
2. Codespace launched successfully  
3. Notebook opened: `feature_engineering_lab.ipynb`
4. First cell runs without errors

**If all checked, you're ready!**

Open the notebook and follow the instructions inside. Good luck!

---

## Additional Resources

- **GitHub Codespaces Help:** https://docs.github.com/codespaces
- **Jupyter Notebook Basics:** Press `Shift + Enter` to run cells
- **Keyboard Shortcuts:** Click the keyboard icon in the notebook toolbar
- **Manage Your Codespaces:** https://github.com/codespaces

---

## Quick Reference: Common Tasks

### Running Code in the Notebook
- **Run current cell:** `Shift + Enter`
- **Run all cells:** Click ▶▶ icon at top of notebook
- **Stop running code:** Click ⏹ (square) icon at top

### Kernel Management
- **Select kernel:** Top-right corner → "Select Kernel" → Choose Python 3.13.x
- **Restart kernel:** Click ↻ icon at top of notebook
- **Clear outputs:** Edit menu → Clear All Outputs

### Codespace Management
- **Stop Codespace:** https://github.com/codespaces → ... menu → Stop
- **Delete Codespace:** https://github.com/codespaces → ... menu → Delete (⚠️ permanent!)
- **Check usage:** https://github.com/settings/billing

### Saving Your Work
- **Auto-save:** Happens automatically (every few seconds)
- **Manual save:** `Ctrl+S` (Windows/Linux) or `Cmd+S` (Mac)
- **Export notebook:** ... menu in notebook toolbar → Export as PDF/HTML

### Getting Unstuck
1. Read error messages carefully (they often tell you what's wrong!)
2. Check if kernel is connected (top-right should show Python 3.13.x)
3. Try restarting the kernel (↻ icon)
4. Check the Troubleshooting section above
5. Ask your instructor for help

---

**Questions before starting?** Ask your instructor!

**Ready to start?** Open `feature_engineering_lab.ipynb` now!
