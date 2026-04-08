##### Student Performance Analysis Dashboard



* ###### **Project Overview**



The Student Performance Analysis Dashboard is a comprehensive Power BI solution designed to monitor academic excellence, student engagement, and behavioral patterns. This two-page dashboard provides school administrators and teachers with high-level summaries and granular individual student profiles to drive data-informed decisions.





* ###### **Data Architecture \& Measures**



The dashboard is built upon a robust data model comprising four main tables: Students, Scores, Attendance, and Behavior.



###### Key Measures Created:



Total Students: A count of all unique student IDs.

Overall Average Score: The mean percentage across all subjects and terms.

Attendance %: Calculated as Present Days / Total Days.

Positive Behavior %: Measures the ratio of helpful/proactive behavior logs.

Target Attendance: A benchmark set at 90% for KPI tracking.





###### **Dashboard Structure**



Page 1: Landing Page (Executive Summary)

This page provides a "Big Picture" view of the entire class or institution.

KPI Cards: Four primary cards displaying Total Students, Average Score, Attendance %, and Behavior Type.

Academic Health Check: A Donut Chart categorizing students into "High," "Medium," and "Low" performance brackets based on their scores.

Discipline Index: A Gauge Chart visualizing overall behavioral trends.

Performance Trends: A Line Chart showing subject scores across different terms.

Interactive Slicers: Filters for Class, Section, Term, Subject, and Gender to allow for dynamic data exploration.



Page 2: Descriptive Page (Individual Student Profile)

An in-depth analysis page accessible via Drill through from the main dashboard.

Subject-wise Detailed Analysis: A Matrix visual breaking down performance by subject and term.



**Student Growth Insights:**

Class Standing: Current rank of the student.

Best Performance: Identification of the student's highest-scoring subject.

Subject Performance Flow: A Ribbon Chart visualizing how a student's subject rankings change over time.

Behavior \& Attendance Logs: A detailed table documenting specific dates, behavior types, and attendance notes.

Target vs. Actual KPI: A specialized KPI visual that turns Green when a student meets the 90% attendance target and Red when they fall below it.



**Implementation Steps**



Step 1: Data Modeling

Import datasets and establish relationships using the Student ID as the primary key.

Create a Calculated Column for performance categories (e.g., High >= 80%, Medium >= 50%, Low < 50%) to enable categorical legends.



Step 2: Visual Development

Apply Rounded Corners (12px) and Shadow Effects to all containers for a modern UI/UX.

Use Conditional Formatting in tables and matrices to highlight risks (Red) and successes (Green).



Step 3: Interactivity Setup

Configure Slicer Settings to "Dropdown" style to maximize canvas space.

Enable "Select All" options in filters for user convenience.

Set up Drill through on the "Name" field to link the Landing Page to the Individual Profile.

