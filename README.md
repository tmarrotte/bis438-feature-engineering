# BIS 438 Machine Learning Lab Series - Setup Guide

**Course:** BIS 438  
**Labs:** Two-part series on Customer Churn Prediction  
**Total Duration:** 2 class periods (~60 minutes each)  
**Difficulty:** Beginner-friendly (no coding experience required!)

---

## 📋 Lab Overview

This is a **two-part lab series** where you'll build a complete machine learning solution for TeleConnect, a telecommunications company trying to predict and prevent customer churn.

### Part 1: Feature Engineering (Week 1)
**Notebook:** `feature_engineering_lab.ipynb`  
**Duration:** ~60 minutes

Learn how to prepare raw customer data for machine learning:
- Cleaning messy data
- Handling missing values
- Creating new features
- Encoding categories for ML models
- Splitting data for training and testing

### Part 2: Model Training (Week 2)
**Notebook:** `model_training_lab.ipynb`  
**Duration:** ~60 minutes

Use your prepared data to build prediction models:
- Training multiple ML models
- Evaluating model performance
- Understanding overfitting
- Identifying churn drivers
- Making predictions on new customers
- Deploying a model for production

**Important:** You must complete Part 1 before starting Part 2, as Part 2 uses the processed data files created in Part 1.

**All instructions are in the notebooks** - this guide just helps you get set up!

---

## Setup Instructions

### Prerequisites
- A GitHub account (free) - [Sign up here](https://github.com/signup) if needed

---

## Step 1: Access the Lab Repository

Your instructor has provided a GitHub repository link. It should look like:
```
https://github.com/[instructor-username]/bis438-churn-prediction-lab
```

Click the link to open the repository.

**Note:** This repository contains both Part 1 and Part 2 notebooks. You'll use the same Codespace for both weeks!

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

2. **Week 1 - Find and click on:** `feature_engineering_lab.ipynb`
   - This is Part 1 of the lab
   - It contains all instructions and code
   
   **Week 2 - Find and click on:** `model_training_lab.ipynb`
   - This is Part 2 of the lab
   - Make sure you've completed Part 1 first!

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
- **Follow along with visualizations and interpretations**

### First Action - Week 1:
1. Open `feature_engineering_lab.ipynb`
2. Click on the **first code cell** (imports libraries)
3. Press **Shift + Enter** to run it
4. You should see: "✅ Libraries loaded successfully!"

### First Action - Week 2:
1. Open `model_training_lab.ipynb`
2. Make sure you completed Part 1 first (you should see `.pkl` files in your directory)
3. Run the first code cell
4. You should see: "✅ Libraries loaded successfully!"

If you see success messages, you're all set!

---

## What's in This Repository?

```
Repository Contents
├── README.md ← You are here (setup guide)
├── feature_engineering_lab.ipynb ← PART 1 - Start here!
├── model_training_lab.ipynb ← PART 2 - Do this second!
├── customer_data.csv (customer data - don't open directly)
├── requirements.txt (Python packages - auto-installed)
├── X_train.pkl (created by Part 1, used by Part 2)
├── X_test.pkl (created by Part 1, used by Part 2)
├── y_train.pkl (created by Part 1, used by Part 2)
├── y_test.pkl (created by Part 1, used by Part 2)
└── .devcontainer/ (Codespaces config - ignore this)
```

**Week 1:** Work with `feature_engineering_lab.ipynb` - it creates the `.pkl` files  
**Week 2:** Work with `model_training_lab.ipynb` - it uses the `.pkl` files

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

- **Environment setup:** 2-3 minutes (one time only)
- **Part 1 (Feature Engineering):** ~60 minutes
- **Part 2 (Model Training):** ~60 minutes
- **Total:** ~2 hours across two class periods

Each lab is designed to be completed in one class period.

**Between weeks:** Your work is automatically saved in Codespaces. When you return for Part 2, just reopen your Codespace and continue where you left off!

---

## What Happens Next?

### Week 1 (Part 1):
1. Complete all code cells in `feature_engineering_lab.ipynb`
2. Answer embedded "YOUR TURN" exercises as you go
3. Take note of interesting findings
4. At the end, you'll save four `.pkl` files for Part 2

### Week 2 (Part 2):
1. Reopen your Codespace (or create a new one)
2. Open `model_training_lab.ipynb`
3. The notebook will load your `.pkl` files from Part 1
4. Complete all code cells and review model results
5. Answer reflection questions

### After Both Labs:
- Your instructor may ask you to submit your completed notebooks
- You'll have built a complete end-to-end ML solution!
- Consider exploring the "Next Steps" section in Part 2 for additional challenges

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

✅ GitHub account created  
✅ Codespace launched successfully  
✅ Notebook opened: `feature_engineering_lab.ipynb` (Week 1) or `model_training_lab.ipynb` (Week 2)  
✅ First cell runs without errors

**If all checked, you're ready!**

**Week 1:** Open `feature_engineering_lab.ipynb` and follow the instructions inside. Good luck!

**Week 2:** Open `model_training_lab.ipynb` and continue your ML journey!

---

## Additional Resources

- **GitHub Codespaces Help:** https://docs.github.com/codespaces
- **Jupyter Notebook Basics:** Press `Shift + Enter` to run cells
- **Keyboard Shortcuts:** Click the keyboard icon in the notebook toolbar

---

**Questions before starting?** Ask your instructor!

**Ready to start Week 1?** Open `feature_engineering_lab.ipynb` now!

**Ready to start Week 2?** Open `model_training_lab.ipynb` now!
