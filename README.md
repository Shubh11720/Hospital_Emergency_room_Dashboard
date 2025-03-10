# Hospital_Emergency_room_Dashboard
Hospital_Emergency_room_Dashboard Ms Excel
Objective:- We need to create a Hospital Emergency Room Analysis Dashboard in Power BI to improve efficiency and provide useful insights. 
This dashboard will help stakeholders monitor, analyze, and make better decisions for managing 
patients and improving services.
KPI's :-
1).Number of Patients:
Count the total number of patients visiting the ER each day.
Show a daily trend with an area sparkline to spot patterns like busy days or seasonal trends
2).Average Wait Time:
Find the average time patients wait to see a medical professional.
Use an area sparkline to track daily changes and highlight days with longer wait times that might need improvements.
3).Patient Satisfaction Score:
Check the average daily satisfaction score of patients to assess service quality.
Use an area sparkline to show trends, spot drops in satisfaction, and link them to busy times or challenges

Charts Create:-
1.Patient Admission Status: Show how many patients were admitted vs. not admitted.
2.Patient Age Distribution: Group patients by age.
3.Timeliness: Measure the percentage of patients seen within 30 minutes.
4.Gender Analysis: Display the number of patients by gender. 
5.Department Referrals: Check which departments patients are referred to the most.
Use Formulas:
1.Calender Table formula
= List.Dates(#date(2023,01,01),731,#duration(1,0,0,0))

2.Dax formulas

DAX Formula for Age Group : 
=IF([Patient Age]>=70,"70-79",IF([Patient Age]>=60,"60-69",IF([Patient Age]>=45,"45-59",IF([Patient Age]>=30,"30-44",IF([Patient Age]>=15,"15-29",IF([Patient Age]>=5,"05-14","0-4"))))))

DAX Formula For Patient Attend Status :
=IF([Patient Waittime]<30,"Within Time","Delay")





