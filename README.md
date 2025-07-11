# Hospital Appointment No-Show Dashboard

## Project Overview

This project is a Power BI dashboard analyzing no-show patterns in hospital appointment data. The dashboard provides actionable insights to improve scheduling efficiency and reduce appointment no-shows by visualizing key trends based on patient demographics, appointment details, and SMS reminders.

---

## Technologies Used

- Microsoft Excel (for data preparation)
- Power BI Desktop (for data modeling and dashboard creation)

---

## Dataset Description

The dataset contains hospital appointment information including:

- AppointmentID
- PatientID
- Gender
- Age
- ScheduledDate
- AppointmentDate
- DayOfWeek
- SMS_Reminder (Yes/No)
- No_Show (Yes/No)

Additional calculated columns in Power BI include:

- `No_Show_Flag`: Numeric flag (1 = No-show, 0 = Show)
- `AgeGroup`: Patient age groups categorized into `<25`, `25-40`, `41-60`, `>60`

---

## Dashboard Components

1. **KPI Cards**  
   - Total Appointments  
   - Total No-Shows  
   - No-Show Rate (%)

2. **No-Shows by Weekday**  
   Clustered bar chart showing no-shows per day of the week.

3. **Gender Breakdown of No-Shows**  
   Pie chart showing distribution of no-shows by gender.

4. **Impact of SMS Reminders**  
   Stacked column chart comparing no-shows based on whether SMS reminders were sent.

5. **No-Shows by Age Group**  
   Bar chart showing no-show counts by patient age group.

---

## Step-by-Step Guide to Build the Dashboard

### Step 1: Load Data

- Open Power BI Desktop
- Import data from Excel (`Appointments.xlsx`)

### Step 2: Prepare Data

- Ensure date columns are set as Date/Time types
- Create calculated columns:
  - `No_Show_Flag = IF(No_Show = "Yes", 1, 0)`
  - `AgeGroup` categorizing ages into buckets

### Step 3: Create KPI Cards

- Card visuals for total appointments, total no-shows, and no-show rate (measure)

### Step 4: Create Visualizations

- Clustered bar chart: No-shows by weekday  
- Pie chart: Gender breakdown of no-shows  
- Stacked column chart: SMS reminder impact  
- Bar chart: No-shows by age group

### Step 5: Polish Dashboard

- Add titles to visuals  
- Use themes and formatting for readability  
- Arrange visuals on the canvas per wireframe layout

### Step 6: Save and Export

- Save as `.pbix` file  
- Export to PDF if needed

---

## How to Use This Repository

- Download the dataset (`Appointments.xlsx`)  
- Open the provided Power BI file (`HospitalDashboard.pbix`)  
- Explore and customize visuals as needed  
- Follow the step-by-step guide in this README to create your own version

---

## Contact

For questions or help, please reach out!

---

## License

This project is released under the MIT License.
