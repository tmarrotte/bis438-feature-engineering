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

4. **Wait for the environment to load**
   - You'll see a VS Code interface in your browser
   - Bottom right will show "Setting up Codespace..."
   - When ready, you'll see "Codespace ready"

### What's Happening?
Codespaces is:
- Creating a virtual computer in the cloud
- Installing Python and all required libraries
- Loading your lab files
- Setting up Jupyter notebook support

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

4. **Select a Python kernel** (if prompted):
   - Click "Select Kernel" in the top right
   - Choose "Python 3.x" (any version listed)

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

### Issue: "Codespace failed to create"
**Solution:** 
- Refresh the page and try again
- Make sure you're logged into GitHub
- Check if you have available Codespace hours (free tier: 120 hours/month)

### Issue: "Kernel not found" or notebook won't run
**Solution:**
1. Wait for Codespaces to fully initialize (check bottom status bar)
2. Click "Select Kernel" in the top right of the notebook
3. Choose any "Python 3.x" option
4. If still not working, close and reopen the notebook file

### Issue: "Module not found" error when running code
**Solution:**
1. Open a new terminal: `Terminal` → `New Terminal` from the top menu
2. Run: `pip install -r requirements.txt`
3. Wait for installation to complete
4. Restart the kernel: Click the ↻ icon at the top of the notebook

### Issue: Lost your work?
**Don't worry!** Codespaces automatically saves your changes. Your work is stored in the cloud.

### Issue: Need to pause and come back later?
**No problem!** 
- Codespaces auto-saves your work
- Just close the browser tab
- Return to the GitHub repository and reopen your Codespace
- Your progress will be exactly where you left off

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

---

**Questions before starting?** Ask your instructor!

**Ready to start?** Open `feature_engineering_lab.ipynb` now!
