# Introduction
This dataset captures the global migration of students pursuing higher education from 2019 to 2023, including their countries of origin, destinations, universities, courses, placement outcomes, and more. It covers 10 major destination countries with realistic mappings of top universities and cities and reflecting trends. 

# Background

 To analyze global student migration trends, scholarship distribution, university choice, and job placements, with a focus on factors such as field of study, country of origin, and language proficiency.
Migration Patterns;Determine which countries are the most popular for students to migrate to.
 Identify trends in student migration based on origin and destination countries/cities,Scholarships and Enrollment.
 Analyze the relationship between scholarships and student enrollment. Investigate the reasons students migrate, including higher rankings, job opportunities, scholarships, etc.

# Tools Used
             Purpose	                     Tools/Tech Used
      Data Cleaning & Sorting	                  Excel
      Dashboard & Visualization	                Power BI
      Presentation	                            Powerpoint    

# Methodology/Tools
Steps: Convert From CSVfiles → Clean 
 Excel:helper columns using IF and nested IF;
Scholarflag=IF([@scholarship_received]="Yes",1,0)
Placement Success=IF([@placement_status]="Placed","Successful","Unsuccessful")
Salary Category (nested IF)=IF([@starting_salary_usd]=0,"Unemployed",IF([@starting_salary_usd]<30000,"Low",IF([@starting_salary_usd]<60000,"Medium","High")))
Performance Level (Based on GPA)=IF([@gpa_or_score]>=3.5,"Excellent",IF([@gpa_or_score]>=3.0,"Good",IF([@gpa_or_score]>=2.0,"Average","Poor")))

 # Power BI = Visualization + KPI dashboard 
      # Visual Title                                   Type                                Description
Placement Rate by Destination                       Ribbon Chart                        %GT Placement Rate by destination_country
Top 10 Destination Countries                        Line & Stacked Chart                Total Students by destination_country  
Global Student Migration Insights Dashboard         Cards & Charts                       Dashboard

# Conclusion
The analysis of global student migration reveals clear patterns in destinations, fields of study, and career outcomes.
Top destinations like the USA, UK, Canada, and Germany continue to attract the majority of students.
STEM and Business fields dominate enrollment, reflecting global job market demand.
Scholarships and higher GPA significantly improve placement success and starting salaries.
Post-graduation outcomes show that academic performance, financial support, and visa opportunities are key drivers of employability.

# Recommendation
Focus recruitment in top destinations and fields with higher placement/salaries.
Expand scholarship programs where they correlate with higher placements.
Strengthen language-test prep in regions with lower placement rates.
 Help shows which countries are most attrative for international students
Helps universities & governments see demand pattern.





