1.	Ask data questions – requested information from stakeholders to determine scope of project:
a.	Viz age and vehicle type of fleet in US
b.	Viz electric vehicle (EV) type already existing #s and % in US
c.	Develop model to identify current ICE fleet vehicles to transition to EV based on daily routes <80mi, >80mi-140mi, and >140mi
d.	Viz # and type of fleet vehicles on order
e.	Viz ICE v EV maintenance costs based on historical data
f.	Viz GHG data from Sustainability group
2.	Prep data – determine 1) all data needed 2) where does it live 
a.	Set up daily data extracts from ePlan reports
b.	Set up daily data extracts from Telematics (meeting set up for 1/16)
c.	Combine datasets
d.	Viz 1.e: 
i.	Review   TCO analysis published by Mark Bluestein to understand process already in place
ii.	Review TCO paper from Argone National Laboratory to develop plan/understand components needed and scope of breakout for TCO
3.	Clean data – Identify data scope and clean up dirty data
a.	Utilize PowerQuery (M) to process and clean data from ePlan
i.	Filter out fleet vehicles from Canada, Latin America
ii.	Filter fleet vehicle type to measured vehicle type (Car, Light Duty Truck, Cargo Van, Minivan, Crossover, SUV) and assign data to existing null fields using data from Department of Energy
iii.	Filter fleet vehicle type by fuel type (Diesel, Electric, Gasoline, Hybrid) and assign data to existing null fields using data from Department of Energy
iv.	Work with contractor ePlan to correct/update bad/missing data
v.	 Cleaned data to ensure uniformity across vehicle year, make, and model
vi.	Created filter to ID vehicles <2004
vii.	Removed duplicate data
viii.	Wrote jupyter notebook for each data source cleaning to explain process + code
b.	Utilize PowerQuery (M) to process and clean data from Telematics
c.	Combine data sources into one Excel Workbook to prep for Tableau
4.	Analyze data – load data into Tableau to develop vizzes to answer data questions
a.	Connect data to Tableau
b.	Create data relationships in Tableau
c.	Viz!
i.	Viz 1.a Viz age and vehicle type of fleet in US
ii.	Viz 1.b Viz EV type already existing # and %
iii.	Viz # and type of fleet vehicles on order 
iv.	Viz EV fleet average daily miles on VIN
v.	Viz total cost of ownership (TCO) internal combustion engine (ICE) v EV
vi.	Create dashboard with filter on vehicle type 
5.	Share data – publish Tableau dashboard to CBRE Intranet/Sharepoint
a.	Find CBRE Tableau dashboard entity to answer questions on data upload and sharing practices, POC Dana Treacy
b.	Research Rest API and read about implementation across Tableau and Sharepoint
