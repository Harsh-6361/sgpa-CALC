# SGPA Calculator 🎮

A web-based SGPA (Semester Grade Point Average) calculator for VTU students following the CBCS (Choice Based Credit System) scheme.

## 📚 What is SGPA?

**SGPA** stands for **Semester Grade Point Average**. It represents your academic performance for a particular semester based on a grading system that considers both marks and credits.

## 🎯 Why Calculate SGPA?

- **Result Analytics**: Provides a single metric to represent your semester performance
- **Credit-Based System**: Accounts for the different credit values of subjects
- **Scholarships & Entrance Exams**: Many programs require SGPA/CGPA as eligibility criteria
- **Campus Placements**: Companies often filter candidates based on CGPA
- **Academic Planning**: Helps track your overall academic progress

## 📊 Grade Point System (VTU Standards)

| Letter Grade | O   | A+  | A   | B+  | B   | C   | P   | F   |
|-------------|-----|-----|-----|-----|-----|-----|-----|-----|
| **Description** | Outstanding | Excellent | Very Good | Good | Above Avg | Average | Pass | Fail |
| **Grade Point** | 10  | 9   | 8   | 7   | 6   | 5   | 4   | 0   |
| **% of Marks** | 90-100 | 80-89 | 70-79 | 60-69 | 55-59 | 50-54 | 40-49 | 0-39 |

## 📝 How to Calculate SGPA Manually

### Formula

```
SGPA = (Sum of Credit Points) / (Total Credits)

Where Credit Points = Credits × Grade Points
```

### Step-by-Step Process

1. **Get Your Results**: Obtain your semester marks from the official VTU website

2. **Convert Marks to Grade Points**: Use the grade point table above to convert each subject's marks to grade points

3. **Note Credits**: Find the credit value for each subject (usually mentioned in your syllabus)

4. **Calculate Credit Points**: For each subject, multiply:
   ```
   Credit Points (Ci × Gi) = Credits × Grade Points
   ```

5. **Sum Up Values**:
   - Add all credits: `Total Credits (ΣCi)`
   - Add all credit points: `Total Credit Points (ΣCi×Gi)`

6. **Calculate SGPA**:
   ```
   SGPA = Total Credit Points / Total Credits
   ```

7. **Convert to Percentage** (Optional):
   ```
   Percentage = (SGPA - 0.75) × 10
   ```
   *This is the official VTU formula*

### 📋 Example Calculation

Let's calculate SGPA for a semester with 9 subjects:

| Course | Credits (Ci) | Marks | Grade | Grade Point (Gi) | Credit Points (Ci × Gi) |
|--------|--------------|-------|-------|------------------|-------------------------|
| XX11   | 3            | 75    | A     | 8                | 3 × 8 = 24              |
| XX12   | 3            | 35    | F     | 0                | 3 × 0 = 0               |
| XX13   | 3            | 85    | A+    | 9                | 3 × 9 = 27              |
| XX14   | 3            | 38    | F     | 0                | 3 × 0 = 0               |
| XX15   | 3            | 58    | B     | 6                | 3 × 6 = 18              |
| XX16   | 1            | 52    | C     | 5                | 1 × 5 = 5               |
| XX17   | 1            | 82    | A+    | 9                | 1 × 9 = 9               |
| XX18   | 2            | 57    | B     | 6                | 2 × 6 = 12              |
| XX19   | 1            | 59    | B     | 6                | 1 × 6 = 6               |
| **TOTAL** | **20**   |       |       |                  | **101**                 |

**Calculation:**
```
SGPA = Total Credit Points ÷ Total Credits
SGPA = 101 ÷ 20
SGPA = 5.05
```

**Percentage Equivalent:**
```
Percentage = (SGPA - 0.75) × 10
Percentage = (5.05 - 0.75) × 10
Percentage = 4.30 × 10
Percentage = 43.0%
```

## 🎓 Calculating CGPA (Cumulative GPA)

To calculate CGPA across multiple semesters:

```
CGPA = (Sum of all Credit Points from all semesters) / (Total Credits from all semesters)
```

**Example:** If you have completed 3 semesters:
- Semester 1: 20 credits, 152 credit points → SGPA = 7.60
- Semester 2: 20 credits, 140 credit points → SGPA = 7.00
- Semester 3: 20 credits, 101 credit points → SGPA = 5.05

```
CGPA = (152 + 140 + 101) / (20 + 20 + 20)
CGPA = 393 / 60
CGPA = 6.55
```

## 🖥️ Using the SGPA Calculator

Instead of manual calculation, use our web-based calculator:

1. Open `index.html` in your web browser
2. Enter your University Serial Number (USN)
3. Select the semester
4. Enter credits and marks for each subject
5. Click "Calculate SGPA"
6. View your SGPA, percentage, and save/print results

### Features
- ✅ Multi-semester tracking
- ✅ Automatic CGPA calculation
- ✅ Data export/import (JSON)
- ✅ Printable grade cards
- ✅ User-friendly interface
- ✅ Mobile responsive design

## 📁 Project Structure

```
sgpa-CALC/
│
├── index.html      # Main calculator application
├── print.html      # Printable result page
├── data.json       # Data storage file
├── Designer.jpeg   # Avatar image
└── README.md       # This file
```

## 🚀 Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/Harsh-6361/sgpa-CALC.git
   ```

2. Open `index.html` in any modern web browser

3. Start calculating your SGPA!

## 💾 Data Storage

- Data is stored in browser's **localStorage**
- Export your data as JSON for backup
- Import previously saved JSON files

## 📱 Browser Compatibility

Works on all modern browsers:
- Chrome
- Firefox
- Safari
- Edge

## 👨‍💻 Author

**Harsh-6361**

## 📄 License

This project is open source and available for educational purposes.

## 🎯 Important Notes

1. **Failed Subjects (F grade)**: Failed subjects are included in SGPA calculation with 0 grade points
2. **Absent Cases**: Mark as failed (0 grade points) if absent for an exam
3. **Backlog Improvement**: When you clear a backlog, recalculate SGPA with the new grade
4. **Official Records**: This calculator is for reference only. Always verify with official VTU results

## 🔗 Official Reference

This calculator follows the VTU CBCS scheme as per **Annexure 3 of VTU regulations**.

---

**© 2024 SGPA Quest. All Rights Reserved. 🎓**
