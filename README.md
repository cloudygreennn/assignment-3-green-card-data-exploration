# 🇺🇸 U.S. Employment-Based Green Card Dashboard

**Interactive Analysis of PERM Application Data**

---

## 📋 Project Overview

This interactive dashboard analyzes U.S. employment-based green card applications (PERM data) to uncover patterns in education, salary, timing, and geographic distribution of sponsorships. Built as part of a data visualization course, this project transforms 90,000+ applications into actionable insights for prospective immigrants.


---

## 🎯 Project Goals

As a first-generation immigrant with 8 years of experience, I wanted to answer critical questions about the green card sponsorship process:

- **Does education level affect salary?**
- **Where are sponsoring companies located?**
- **What is the optimal timing after graduation to apply?**
- **Which companies sponsor the most applicants?**
- **Am I on track compared to others?**

---

## 📊 Dashboard Features

### **5 Interactive Visualizations:**

1. **📊 Education Level vs. Salary (Box Plot)**
   - Shows salary distribution across education levels
   - Reveals Bachelor's degree as a key salary threshold

2. **📈 Years After Graduation vs. Salary (Scatter Plot with Dual Y-Axes)**
   - Displays salary patterns over time
   - Includes applicant volume line showing peak application years
   - Features personal 8-year marker for context

3. **🎻 Education vs. Years After Graduation (Violin Plot)**
   - Reveals timing patterns by education level
   - Shows Master's holders typically wait 5-10 years

4. **🗺️ Top 10 States by Applications (Stacked Bar Chart)**
   - Geographic distribution of opportunities
   - Color-coded by education level
   - California, Washington, and Texas dominate

5. **🏢 Top Companies (Treemap)**
   - Visual hierarchy of sponsoring companies
   - Microsoft, Meta, LinkedIn, and Oracle lead the pack
   - Size represents sponsorship volume

### **3 Global Filters:**

- **🎓 Education Level** - Filter by degree (High School to Doctorate)
- **🏢 Industry** - Focus on specific sectors (e.g., Information)
- **💰 Salary Range** - Adjustable $20K-$500K range

**All visualizations update simultaneously when filters change!**

---

## 📊 Key Insights

### **Finding #1: Bachelor's Degree = Salary Threshold**
Bachelor's degree holders see a significant salary jump compared to Associate's degrees, with median salaries around $130-160K in the Information industry.

### **Finding #2: Peak Application Timing is 4-8 Years**
Most successful applicants apply within 4-8 years after graduation, as shown by the applicant volume line in Chart 2.

### **Finding #3: Master's Holders Wait 5-10 Years**
The violin plot reveals Master's degree holders typically wait 5-10 years before applying—right on schedule at the 8-year mark.

### **Finding #4: California Dominates Geographic Distribution**
With 3,000+ applications, California leads, followed by Washington (Microsoft, Amazon) and Texas—mostly Master's degree holders.

### **Finding #5: Tech Giants Lead Sponsorships**
Microsoft sponsors the most applicants, followed by Meta, LinkedIn, Oracle, and Amazon—the treemap shows clear market dominance.

---

## 🚧 Challenges & Solutions

### **Challenge 1: Large Dataset Performance**
**Problem:** 90,000+ records caused slow rendering  
**Solution:** Implemented smart filtering and data aggregation before visualization

### **Challenge 2: Panel Framework Issues**
**Problem:** Panel had compatibility issues with Jupyter rendering  
**Solution:** Switched to ipywidgets for more reliable interactive controls

### **Challenge 3: Multiple Visualizations Update**
**Problem:** Charts not updating simultaneously  
**Solution:** Implemented manual UPDATE button with centralized filter_data() function

### **Challenge 4: Dual Y-Axes Complexity**
**Problem:** Scatter plot needed to show both salary and volume  
**Solution:** Used plotly's secondary y-axis feature with contrasting line style

---


## 📌 Quick Start Summary

```bash
# 1. Install dependencies
pip install pandas numpy plotly ipywidgets jupyter

# 2. Enable widgets
jupyter nbextension enable --py widgetsnbextension

# 3. Open notebook
jupyter notebook assignment_3_-_green_card_data_exploration.ipynb

# 4. Run all cells

# 5. Interact with dashboard in the final section!
```

---

**Last Updated:** November 2025  
**Version:** 1.0

---

*"This dashboard turns data into actionable career insights for aspiring immigrants."* 🇺🇸✨
