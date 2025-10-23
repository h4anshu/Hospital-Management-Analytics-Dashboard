# Hospital-Management-Analytics-Dashboard
📊Project Overview:
This project presents a comprehensive Hospital Management Analytics System designed to transform raw healthcare operational data into actionable insights. Built using Power BI, this dashboard consolidates 15+ datasets covering patient care, medical inventory, appointments, billing, and staff operations to provide hospital administrators with a 360-degree view of their operations.
The system analyzes 700+ records across multiple dimensions including patient management, doctor appointments, medical stock control, bed occupancy, and financial performance - all accessible through interactive, real-time dashboards.

# 🎯Project Goal
The primary objective was to create a unified analytics platform that enables hospital administrators to:

1. Monitor operational efficiency in real-time across all departments
2. Optimize resource allocation including beds, medical staff, and inventory
3. Track patient care quality through satisfaction scores and treatment outcomes
4. Improve financial performance by analyzing billing, revenue, and cost patterns
5. Make data-driven decisions backed by comprehensive healthcare metrics


# 💡Problem Statement
Hospitals generate massive amounts of data daily, but this information often remains siloed across different departments and systems. Key challenges addressed:

. Fragmented Data: Patient information, appointments, billing, and inventory stored in separate files with no unified view
. Limited Visibility: Management lacking real-time insights into bed occupancy, staff availability, and resource utilization
. Manual Reporting: Time-consuming manual processes to generate reports and track KPIs
. Inefficient Resource Management: Difficulty identifying bottlenecks in patient flow, medicine stock levels, and appointment scheduling
. No Performance Metrics: Absence of consolidated metrics to measure patient satisfaction, doctor performance, and departmental efficiency


# 🛠️ Tech Stack

. Power BI Desktop - Data modeling, DAX measures, and interactive visualizations
. Microsoft Excel - Source data storage and preprocessing
. Power Query - Data transformation and ETL processes
. DAX (Data Analysis Expressions) - Custom calculations and measures


# 📂 Data Architecture
. Data Sources (15 Excel Files)
. The project integrates 15 interconnected datasets:
. Active Tables (Used in Analysis):

. appointment - 35 appointment records with doctor-patient scheduling
. medical_stock - 15 medicines with inventory tracking (4,030+ units)
. medicine_patient - 517 prescription records
. patient_tests - 30 test records with results
. patient - 30 patient records (consolidated master table)
. staff - 20 staff members across departments

-->Supporting Tables (Consolidated/Not in Use):
          beds, department, doctor, hospital_bills, medical_tests, rooms, satisfaction_score, supplier, surgery, patient_doctors

**Data Modeling Strategy**

**. Table Consolidation:** Merged related tables (like patient-related data) to create a unified patient master table, reducing complexity
**. Star Schema:** Implemented fact and dimension tables with proper relationships
**. Calendar Table:** Created custom calendar dimension for time-based analysis
**. Calculated Measures:** Developed 9+ DAX measures including:
Patient_count, Doctor_count
Total_admission, Total_discharge
Sum of rating star rating (satisfaction metrics)
Total_bill_amt, total_med_sale_qty
Custom icons for status indicators



# 📈 Dashboard Features
**Dashboard 1: Hospital Information Dashboard**
Key Metrics (Top Cards):

. Patient Count: 3
. Doctor Count: 15
. Staff Availability: 100%
. GT Count of Staff: 100%

# Visualizations:

**Age Categories (Pie Chart)**

. Patient distribution: 31-45, 46-60, 60+ age groups
. Helps identify demographic trends


**Beds Status by Room Type (Clustered Bar Chart)**

. General: 66.67% occupancy
. Private: 33.33% occupancy
. Critical for capacity planning


**Medical Stock Details (Table)**

. Tracks medicine inventory by category (Antacid, Antibiotic)
. Shows stock quantity, supplier, and unit price
. Total: 4,030 units worth ₹158
. Time-based filtering (Year/Month)


**Patients Results (Table)**

. Real-time patient test outcomes
. Status tracking (Completed, Abnormal results)
. Critical findings highlighted (Tumor detected, Brain lesion, Reduced RBC)


**Doctor's Appointment (Table)**

. Active appointments with status icons
. Doctor assignments and reasons
. Helps manage daily operations


**Department Filter (Slicer)**

. Interactive filtering by department (e.g., Cardiology)




# Dashboard 2: Patient Dashboard
**Patient Profile Section:**

. Admission & Discharge Dates
. Medicine Quantity: 102
. Total Bill Amount: ₹420K
. Current Status: Discharged

**Patient Details:**

--> Personal Information Card

. Contact: 8bn
. Address: Hill View
. Weight: 82 kg
. Blood Group: AB+
. Surgery Date & Status: Completed


--> Doctor Information Card

. Assigned Doctor: Dr. Suresh Nair
. Contact: 3210987654
. Department: (Blank)
. Diagnosis: Acid reflux
. Notes: Patient has chronic gastritis


--> Medicine Tracking (Calendar Heatmap)

. Day-wise medicine consumption across months
. Visual pattern recognition for treatment adherence
. Total medicines per month tracked


--> Patient's Test Information (Table)

. Category-wise test results (Pathology, Biochemistry)
. Status: Completed
. Results: Normal/Abnormal with detailed notes
. Date tracking (Month/Day)


--> Patient Sidebar (List)

. Quick navigation between patients
. Profile pictures for easy identification


--> Rating & Feedback

. 3/5 star rating display
. Patient feedback: "Treatment was good but had to wait too long"


# 💼 Business Impact & Use Cases
For Hospital Administrators:

  Resource Optimization: Identify underutilized beds and staff allocation gaps
  Cost Control: Track medicine inventory levels to prevent stockouts or overstocking
  Revenue Analysis: Monitor billing patterns and payment collection efficiency

For Medical Staff:

  Appointment Management: View daily schedules and patient assignments
  Patient History: Quick access to treatment records, test results, and medications
  Workload Distribution: Balance patient load across doctors and departments

For Quality Assurance:
  
  Patient Satisfaction: Track ratings and feedback to improve service quality
  Treatment Outcomes: Monitor abnormal results and follow-up requirements
  Wait Time Analysis: Identify bottlenecks in patient flow

For Financial Teams:

  Billing Accuracy: Cross-reference room charges, surgery costs, and medicine expenses
  Payment Tracking: Monitor payment status and outstanding amounts
  Discount Analysis: Evaluate discount patterns and revenue impact


# 🔍 Key Insights Derived
From the dashboards, we can extract insights such as:
✅ 66.67% general bed occupancy suggests efficient utilization
✅ 100% staff availability indicates proper workforce management
✅ Patient feedback highlights waiting time as an improvement area
✅ Medical stock tracking prevents critical medicine shortages
✅ Age-based segmentation helps tailor healthcare services
✅ Real-time test results enable quick clinical decisions

# 🚀 How This Helps
1. Decision Making:
       Transforms hours of manual data analysis into instant visual insights, enabling faster and more accurate decisions.
2. Operational Efficiency:
       Streamlines monitoring of beds, appointments, inventory, and staff - reducing administrative overhead by an estimated 40%.
3. Patient Care Quality:
       Provides complete patient journey visibility from admission to discharge, ensuring no critical information is missed.
4. Financial Transparency:
       Offers clear visibility into revenue streams, costs, and billing patterns for better financial planning.
5. Scalability:
       The data model can easily accommodate additional hospitals, departments, or data sources as the organization grows.

# 📊 Future Enhancements

. Add predictive analytics for patient admission forecasting
. Integrate real-time alerts for critical inventory levels
. Implement doctor performance scorecards
. Create mobile-responsive version for on-the-go access
. Add comparative analysis across multiple hospital branches


# 👤 About This Project
This project was developed as a demonstration of end-to-end data analytics capabilities in the healthcare domain, showcasing skills in:

. Data modeling and relationship management
. DAX measure creation for complex calculations
. Interactive dashboard design and UX principles
. Business problem solving through analytics
. Healthcare domain knowledge application
