# Conference Registration Forecasting System

A real-time forecasting system that predicts conference registration numbers based on current data and historical patterns. Perfect for event organizers who need to make data-driven decisions about their marketing campaigns.

## 📊 What This System Does

- **Predicts final registration numbers** based on your current registration data
- **Provides confidence ranges** (conservative, likely, optimistic estimates)
- **Shows weekly targets** to help you stay on track
- **Accounts for external factors** like UK bank holidays and disruptions
- **Creates visual dashboards** with charts and graphs
- **Gives actionable recommendations** for your marketing strategy

## 🎯 Perfect For

- Event organizers planning conferences
- Marketing teams tracking registration campaigns
- Anyone who needs to predict event attendance
- Organizations wanting data-driven insights

---

## 🚀 Quick Start Guide

### Step 1: Install Python (if you don't have it)

1. **Download Python:**
   - Go to https://www.python.org/downloads/
   - Download Python 3.8 or newer
   - **Important:** During installation, check the box "Add Python to PATH"

2. **Verify installation:**
   - Open Terminal (Mac) or Command Prompt (Windows)
   - Type: `python --version`
   - You should see something like "Python 3.x.x"

### Step 2: Download the System

1. **Download all files** to a folder on your computer
2. **Make sure you have these files:**
   - `realtime_conference_forecasting.ipynb` (the main system)
   - `sample_data.csv` (example registration data)
   - `CONF. DATASET/` folder (historical data)
   - `README.md` (this file)

### Step 3: Set Up Your Environment

1. **Open Terminal/Command Prompt**
2. **Navigate to your project folder:**
   ```bash
   cd "path/to/your/registration-forcasting folder"
   ```
   Example: `cd "/Users/yourname/Desktop/registration-forcasting"`

3. **Create a virtual environment:**
   ```bash
   python -m venv .venv
   ```

4. **Activate the environment:**
   
   **On Mac/Linux:**
   ```bash
   source .venv/bin/activate
   ```
   
   **On Windows:**
   ```bash
   .venv\Scripts\activate
   ```
   
   You should see `(.venv)` at the start of your command line.

5. **Install required packages:**
   ```bash
   pip install jupyter pandas numpy matplotlib scipy scikit-learn
   ```

### Step 4: Prepare Your Data

1. **Replace the sample data:**
   - Open `sample_data.csv` in Excel or any spreadsheet program
   - Replace with your actual registration data
   - **Required columns:**
     - `Created Date` (format: DD/MM/YYYY, e.g., "15/07/2025")
     - Any other columns are fine to keep

2. **Update event details:**
   - Open the notebook (Step 5) and look for cell 3
   - Change these values to match your event:
     - `event_date = "15/08/2025"` (your event date)
     - `marketing_start_date = "01/07/2025"` (when you started marketing)

### Step 5: Run the System

1. **Start Jupyter:**
   ```bash
   jupyter notebook
   ```
   This will open your web browser automatically.

2. **Open the notebook:**
   - Click on `realtime_conference_forecasting.ipynb`

3. **Run all cells:**
   - Click "Cell" → "Run All" from the menu
   - Or press `Shift + Enter` on each cell one by one

4. **View your results:**
   - Scroll down to see forecasts, charts, and recommendations
   - Look for the "FINAL REGISTRATION FORECAST" section

---

## 📋 Understanding Your Results

### Main Forecast Section
```
FINAL REGISTRATION FORECAST
Current registrations: 179
Most Likely Total: 539 registrations
Conservative Estimate: 179 registrations  
Optimistic Estimate: 1045 registrations
Weekly target: 120 registrations/week
```

**What this means:**
- **Current registrations:** How many people have registered so far
- **Most Likely Total:** Our best estimate of final attendance
- **Conservative/Optimistic:** The range of possible outcomes
- **Weekly target:** How many registrations you need per week to reach the forecast

### Risk Assessment
- **🟢 LOW RISK:** You're on track, keep doing what you're doing
- **🟡 MODERATE RISK:** Need to maintain or slightly increase efforts  
- **🔴 HIGH RISK:** Significant acceleration needed in marketing

### Charts and Graphs
- **Registration Timeline:** Shows actual vs. predicted registrations
- **Weekly Performance:** Bar chart of registrations per week
- **Method Confidence:** How much we trust each prediction method

---

## 🔄 Updating with New Data

As new registrations come in, update your forecasts:

1. **Update your CSV file** with new registration data
2. **Run the notebook again** (Cell → Run All)
3. **Review new forecasts** and adjust marketing strategy accordingly

**Recommended:** Update weekly for best results.

---

## 📁 File Structure

```
registration-forcasting/
├── realtime_conference_forecasting.ipynb  # Main system
├── sample_data.csv                         # Your registration data
├── README.md                               # This guide
└── CONF. DATASET/                          # Historical patterns
    ├── Education Managers/
    ├── Education property managers/
    ├── IT MANAGER/
    └── Property Managers/
```

---

## ❓ Troubleshooting

### "Python not found" or "Command not found"
- Make sure Python is installed and added to PATH
- Try `python3` instead of `python`

### "Module not found" errors
- Make sure your virtual environment is activated (you should see `.venv`)
- Run: `pip install jupyter pandas numpy matplotlib scipy scikit-learn`

### "File not found" errors
- Make sure you're in the correct folder
- Check that `sample_data.csv` exists and has the right name
- Verify the `CONF. DATASET` folder is present

### Jupyter won't start
- Try: `python -m jupyter notebook`
- Make sure you're in the virtual environment

### Charts don't appear
- Try restarting Jupyter: Close browser, stop with Ctrl+C, restart
- Run cells one by one instead of "Run All"

### Poor predictions
- Make sure your registration data has dates in DD/MM/YYYY format
- Check that your event date and marketing start date are correct
- Ensure you have at least 2-3 weeks of registration data

---

## 💡 Tips for Best Results

1. **Data Quality:** Ensure your registration dates are accurate and complete
2. **Regular Updates:** Run forecasts weekly as new data comes in
3. **Multiple Scenarios:** Use the confidence ranges to plan for different outcomes
4. **External Factors:** Pay attention to warnings about holidays or short timelines
5. **Historical Context:** The system learns from similar past events automatically

---

## 🆘 Need Help?

If you encounter issues:

1. **Check the troubleshooting section** above
2. **Verify your data format** matches the sample
3. **Make sure all files are in the right place**
4. **Try running cells one by one** to isolate problems

---

## 📈 Example Use Case

**Scenario:** You're organizing a tech conference in August 2025.

1. **Week 1:** 64 registrations → System predicts 539 total
2. **Week 2:** 80 new registrations → Revised prediction: 612 total  
3. **Week 3:** 35 new registrations → System warns of slowdown
4. **Action:** Increase marketing spend based on recommendations

The system helps you make informed decisions throughout your campaign!

---

*This system uses proven forecasting methods including pattern matching, velocity analysis, and curve fitting to provide reliable predictions for your event planning needs.*