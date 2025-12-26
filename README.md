
Table	Column Name
Complaints (Fact)	Complaint ID	Unique identifier for each complaint.	
Complaints (Fact)	Submitted via	Submission channel used by the consumer (e.g., Web, Referral).	
Complaints (Fact)	Date submitted	Date the consumer submitted the complaint.	
Complaints (Fact)	Date received	Date the authority/company recorded receipt of the complaint.	
Complaints (Fact)	State	U.S. state of the consumer.	
Complaints (Fact)	State_Latitude	Latitude of the state centroid. REQUIRED for ZoomCharts Drill Down Map PRO.	
Complaints (Fact)	State_Longitude	Longitude of the state centroid. REQUIRED for ZoomCharts Drill Down Map PRO.	
Complaints (Fact)	Product	Financial product category (e.g., Mortgage, Credit reporting).	
Complaints (Fact)	Sub-product	More specific product type (e.g., Conventional mortgage).	
Complaints (Fact)	Issue	General problem category reported by the consumer.	
Complaints (Fact)	Sub-issue	More detailed problem description.	
Complaints (Fact)	Company public response	Public statement from the company regarding the complaint.	
Complaints (Fact)	Company response to consumer	Outcome communicated to the consumer (e.g., Closed with explanation).	
Complaints (Fact)	Timely response?	Whether the company responded within the required timeframe (Yes/No).	
Complaints (Fact)	Census_Region	U.S. Census region for the state (Northeast, Midwest, South, West).	
Complaints (Fact)	Census_Division	U.S. Census division for the state (nine-division scheme).	
Complaints (Fact)	Company_Response_Date	Company response date.	
Complaints (Fact)	Company_ID_1081	Company identifier (COMP-0001 … COMP-1081).	
Complaints (Fact)	Response_Time_Days	Calculated days between Date submitted and Company_Response_Date.	
Company (Dimension)	Company_ID_1081	Company identifier (COMP-0001 … COMP-1081).	
Company (Dimension)	Market_Share_Percent	Market share percentage; sums to ~100% across all companies.	
Company (Dimension)	Reputation_Score	Reputation score (50–100).	
Company (Dimension)	Enforcement_History	Flag for past regulatory actions (Yes/No).	
Company (Dimension)	Company_Size_Tier	Company size classification based on market share rank.	
Company (Dimension)	Complaint_Count	Number of complaints linked to the company (from fact table).	
Company (Dimension)	Timely_Response_Rate	Percentage of complaints marked 'Timely response?' = Yes for the company.	
Company (Dimension)	Avg_Response_Time_Days	Average days from submission to response date for the company.	
Company (Dimension)	Complaints_per_1pct_Share	Complaint_Count divided by Market_Share_Percent; normalization KPI.	
			
