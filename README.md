# Employee-Performance-Analysis

Sheet_Name	Field_Name	Data_Type	Description	Sample_Values	
DATASET OVERVIEW	Total Sheets	Count	Number of data sheets: 5		
DATASET OVERVIEW	Total Records	Count	Total records across all sheets: 497,032		
DATASET OVERVIEW	Date Format	Format	All dates formatted as dd/mm/yyyy	31/12/2024	
DATASET OVERVIEW	Manager Assignment	Business Rule	Employees assigned managers based on job hierarchy	Hierarchical structure	
					
EMPLOYEES	SHEET SUMMARY		Contains 7,500 records with 17 fields		
employees	Employee_Id	Text	Unique employee identifier	EMP000001, EMP000002, EMP000003	
employees	Full_Name	Text	Employee full name (synthetic)	Marie Kim DDS, Danny Morgan, Crystal Robinson	
employees	Gender	Text	Employee gender (M/F/Other)	F, Other, M	
employees	Age	Numeric	Employee age in years	23, 26, 38	
employees	Education_Level	Text	Highest education level achieved	Master's, Bachelor's, High School	
employees	Hire_Date	Date (dd/mm/yyyy)	Date when employee was hired (dd/mm/yyyy)	26/04/2021, 03/09/2021, 25/08/2016	
employees	Exit_Date	Date (dd/mm/yyyy)	Date when employee left (dd/mm/yyyy, blank if active)	13/04/2022, , 04/04/2021	
employees	Department	Text	Business department/division	Store Operations, Logistics/Warehousing, Fresh Produce	
employees	Job_Role	Text	Specific job position/title	Assistant Manager, Store Manager, Floor Supervisor	
employees	Job_Level	Text	Seniority level (Entry/Associate/Supervisor/Manager/Executive)	Manager, Supervisor, Associate	
employees	Employment_Type	Text	Employment classification (Full-time/Part-time/Seasonal/Contractor)	Full-time, Part-time, Seasonal	
employees	Store_Location	Text	City/region where employee works	Charlotte, San Jose, Jacksonville	
employees	Store_Location_Latitude	Numeric	Data field - see sheet for values	35.2271, 37.3382, 30.3322	
employees	Store_Location_Longitude	Numeric	Data field - see sheet for values	-80.8431, -121.8863, -81.6557	
employees	Store_Id	Text	Store identifier	STR058, STR137, STR008	
employees	Manager_Id	Text	Direct manager employee ID	EMP001772, EMP002303, EMP000784	
employees	Base_Salary_Annual	Numeric	Annual base salary in currency units	82900.51, 76074.52, 76059.01	
					
STORES	SHEET SUMMARY		Contains 150 records with 7 fields		
stores	Store_Id	Text	Store identifier	STR001, STR002, STR003	
stores	Store_Name	Text	Store display name	San Antonio Regular #1, Charlotte Regular #2, Portland Superstore #3	
stores	City	Text	Store city location	San Antonio, Charlotte, Portland	
stores	City_Latitude	Numeric	Data field - see sheet for values	29.4241, 35.2271, 45.5152	
stores	City_Longitude	Numeric	Data field - see sheet for values	-98.4936, -80.8431, -122.6784	
stores	Store_Type	Text	Store format (Superstore/Regular/Express)	Regular, Superstore, Express	
stores	Opening_Date	Date (dd/mm/yyyy)	Store opening date (dd/mm/yyyy)	20/05/2021, 09/11/2015, 08/02/2018	
					
MONTHLY_PERFORMANCE	SHEET SUMMARY		Contains 236,591 records with 13 fields		
monthly_performance	Employee_Id	Text	Unique employee identifier	EMP000001, EMP000002, EMP000003	
monthly_performance	Year_Month	Text	Performance period (YYYY-MM)	2022-01, 2022-02, 2022-03	
monthly_performance	Performance_Rating	Numeric	Overall performance rating (1-5 scale)	4.13, 3.6, 3.65	
monthly_performance	Training_Hours	Numeric	Hours of training completed	2, 9, 3	
monthly_performance	Overtime_Hours	Numeric	Overtime hours worked	15, 10, 12	
monthly_performance	Absenteeism_Days	Numeric	Days absent from work	1, 0, 2	
monthly_performance	Promotion_Flag	Boolean	Whether employee was promoted (True/False)	False, True	
monthly_performance	Salary_Increase_Flag	Boolean	Whether employee received salary increase (True/False)	False, True	
monthly_performance	Monthly_Bonus	Numeric	Performance-based bonus amount	657.44, 626.76, 554.12	
monthly_performance	Benefits_Cost	Numeric	Monthly benefits cost	1727.09, 1584.89, 1584.56	
monthly_performance	Employee_Satisfaction	Numeric	Employee satisfaction survey score (1-10)	8.0, 6.3, 8.1	
monthly_performance	Engagement_Index	Numeric	Employee engagement index (1-10)	8.1, 9.1, 5.1	
monthly_performance	Manager_Evaluation	Numeric	Manager evaluation score (1-5)	4.5, 3.6, 3.5	
					
ROLE_KPIS	SHEET SUMMARY		Contains 236,591 records with 9 fields		
role_kpis	Employee_Id	Text	Unique employee identifier	EMP000001, EMP000002, EMP000003	
role_kpis	Year_Month	Text	Performance period (YYYY-MM)	2022-01, 2022-02, 2022-03	
role_kpis	Kpi_1_Value	Numeric	Data field - see sheet for values	87.77, 88.94, 85.0	
role_kpis	Kpi_1_Name	Text	Data field - see sheet for values	Task Completion Rate %, Store Sales vs Target %, Items Scanned per Hour	
role_kpis	Kpi_2_Value	Numeric	Data field - see sheet for values	8.2, 6.66, 17.37	
role_kpis	Kpi_2_Name	Text	Data field - see sheet for values	Quality Score, Employee Turnover %, Till Accuracy %	
role_kpis	Kpi_3_Value	Numeric	Data field - see sheet for values	9.15, 6.09, 7.21	
role_kpis	Kpi_3_Name	Text	Data field - see sheet for values	Efficiency Rating, Customer Satisfaction, Customer Complaints	
role_kpis	Productivity_Index	Numeric	Data field - see sheet for values	1.565, 1.302, 1.323	
					
BUSINESS_OUTCOMES	SHEET SUMMARY		Contains 16,200 records with 9 fields		
business_outcomes	Store_Id	Text	Store identifier	STR001, STR002, STR003	
business_outcomes	Department	Text	Business department/division	Store Operations, Fresh Produce, Meat/Fish & Bakery	
business_outcomes	Year_Month	Text	Performance period (YYYY-MM)	2022-01, 2022-02, 2022-03	
business_outcomes	Sales_Target	Numeric	Monthly sales target	153000, 38250, 29750	
business_outcomes	Sales_Actual	Numeric	Actual monthly sales	164399.59, 39851.0, 30829.76	
business_outcomes	Customer_Satisfaction	Numeric	Customer satisfaction score (1-10)	7.4, 8.5, 5.6	
business_outcomes	Nps_Score	Numeric	Net Promoter Score (-100 to 100)	47.0, 51.5, -24.1	
business_outcomes	Waste_Percentage	Numeric	Waste/loss percentage	0.73, 2.73, 3.64	
business_outcomes	On_Time_Delivery	Numeric	On-time delivery percentage	98.6, 92.4, 92.3
