# MIST 4610 Project 2
# Team Name: cs_g2p1
# Team Members:
1. Thommy Chhim [@SpaMnky](https://github.com/SpaMnky)

2. Vasil Gerchev [@vgg01171](https://github.com/vgg01171)

3. Robert You [@PointBrok3n](https://github.com/PointBrok3n)

4. Brian Ferro  [@dinough](https://github.com/dinough)

5. Nathan Rockwell [@nathanrockwell](https://github.com/nathanrockwell) 

## Description of dataset:
Our dataset details the information on motor vehicle collisions in Montgomery County, sourced from the Automated Crash Reporting System (ACRS) of the Maryland State Police and reported by various law enforcement agencies. We obtained our dataset through the website provided: https://catalog.data.gov/dataset/crash-reporting-drivers-data. Included below is a description of each of the individual columns, as well as the data type associated.

Report Number: A unique identifier for each collision report. (Integer) 

Local Case Number: Local identifier assigned to the case by law enforcement. (Integer)

Agency Name: Name of the law enforcement agency handling the collision report. (String) 

ACRS Report Type: Type of ACRS report, indicating whether it resulted in property damage or injury. (String) 

Crash Date/Time: Date and time when the collision occurred. (Date and Time) 

Route Type: Specifies the type of route where the collision occurred, providing information about the classification of the roadway (e.g., County, Maryland State). (String) 

Road Name: Indicates the name of the road where the collision occurred. (String) 

Cross-Street Type: Describes the type of street intersecting with the main road. (String) 

Cross-Street Name: Provides the name of the cross-street intersecting with the main road. (String) 

Off-Road Description: Description of the off-road location if the collision occurred off the road. (String) 

Municipality: The municipality where the collision occurred. (String) 

Related Non-Motorist: Involvement of non-motorists (e.g., pedestrians or cyclists) in the collision. (String) 

Collision Type: Type of collision (e.g., rear-end, head-on, same direction rear-end). (String) 

Weather: Describes the prevailing weather conditions during the collision. (String) 

Surface Condition: Indicates the condition of the road surface, such as dry, wet, or icy. (String) 

Light: Specifies the lighting conditions at the time of the collision (e.g., daylight, dusk, dark with streetlights). (String) 

Traffic Control: Describes the type of traffic control present at the collision location, such as stop signs or traffic signals. (String) 

Driver Substance Abuse: Indicates whether the driver involved in the collision was under the influence of substances (e.g., alcohol or drugs). (String) 

Non-Motorist Substance Abuse: Indicates if substances played a role in the behavior of non-motorists involved in the collision, such as pedestrians or cyclists. (String) 

Person ID: Unique identifier for individuals involved in the collision. (Integer) 

Driver At Fault: Indicates whether the driver was at fault in the collision. (String) 

Injury Severity: Severity of injuries sustained by individuals. (String) 

Circumstance: Circumstances surrounding the collision. (String) 

Driver Distracted By: Factors distracting the driver during the collision. (String) 

Drivers License State: State of issuance of the driver's license. (String) 

Vehicle ID: A unique identifier for each vehicle involved in the collision. (Integer) 

Vehicle Damage Extent: Describes the extent of damage sustained by the vehicle (e.g., superficial, functional, disabling, destroyed). (String) 

Vehicle First Impact Location: Specifies the location on the vehicle where the first impact occurred. (String) 

Vehicle Second Impact Location: Specifies the location on the vehicle where the second impact occurred. (String) 

Vehicle Body Type: Indicates the body type of the vehicle (e.g., passenger car, medium/heavy truck, SUV). (String) 

Vehicle Movement: Describes the movement of the vehicle during the collision (e.g., slowing or stopping, making a right turn). (String) 

Vehicle Continuing Dir: Specifies the direction in which the vehicle continued after the collision. (String) 

Vehicle Going Dir: Specifies the direction in which the vehicle was initially going before the collision. (String) 

Speed Limit: Indicates the speed limit of the roadway where the collision occurred. (Integer) 

Driverless Vehicle: Indicates whether a driverless vehicle was involved in the collision. (String) 

Parked Vehicle: Indicates whether a parked vehicle was involved in the collision. (String) 

Vehicle Year: Specifies the manufacturing year of the vehicle. (Integer) 

Vehicle Make: Indicates the make or manufacturer of the vehicle. (String) 

Vehicle Model: Specifies the model of the vehicle. (String) 

Equipment Problems: Indicates any reported equipment problems with the vehicle. (String) 

Latitude: The geographic coordinate specifying the north-south position of the collision location. (String) 

Longitude: The geographic coordinate specifying the east-west position of the collision location. (String) 

Location: Detailed information about the collision location. (String) 

However, it is essential to note that this dataset may include preliminary information subject to further verification and investigation. Overall, this dataset has a variety of dimensions that provide a comprehensive view of the information on motor vehicle collisions in Montgomery County. These dimensions enable a detailed analysis of each collision, contributing to a better understanding of the factors involved in traffic incidents.



## Question 1:

Question: 
During which hours of the day are car crashes most frequent? Within these peak hours, which days of the week experience the highest number of crashes, and during which months do most of these accidents occur?


Importance:  
This question is significant in understanding the timing and patterns of car crashes, which is crucial for implementing safety measures and resource allocation. Analyzing the temporal patterns of car crashes within a dataset is essential for informed decision-making and enhanced road safety. By discerning the hours, days, and months when car accidents are most prevalent, authorities can allocate resources more efficiently, ensuring that law enforcement and emergency services are adequately prepared during peak periods. This knowledge also facilitates the development of targeted public safety campaigns and initiatives to address specific risk periods. Furthermore, this dataset raises public awareness of peak high-risk hours which are during rush periods of 3 pm - 5 pm. We can also identify which days are the most risky for drivers on the road, which is shown to be during weekdays. With this data we can also identify peak high-risk periods of the year, we can noticeably see an increase in risk reports from April to June and from September to October. 

<img width="464" alt="image" src="https://github.com/nathanrockwell/MIST4610-Project-2/assets/148256894/84e9fdb7-7782-4f32-ac65-2918ed73befd">

The first graph shows us the number of crashes based on the time of day. By looking at this graph, it is clear that most accidents occur between the hours of 3:00 PM and 5:00 PM. This data is further analyzed in the following graph:

<img width="746" alt="image" src="https://github.com/nathanrockwell/MIST4610-Project-2/assets/148256894/8ffcda25-f274-43fe-a1ed-c473164ed6c0">

This visualization shows accidents between hours of 3:00 PM and 5:00 PM with the corresponding day of the week they occurred. The graph shows that most of these accidents occur on weekdays, which is most likely a result of rush-hour traffic with commuters returning home from work.

<img width="554" alt="image" src="https://github.com/nathanrockwell/MIST4610-Project-2/assets/148256894/db141649-9e4f-4ff1-b6a7-ec1fa1231bb6">

The final visualization for this questions shows the total number of crashes between 3:00 PM and 5:00 PM for each weekday, along with the month in which these accidents occurred. This data shows us that there is a decrease in the number of accidents in June and July, which could be due to people being on vacation or our of work for the summer. The data makes it clear that the number of accidents is directly correlated to the number of travellers on the road. This is important because it shows that law enforcement should allocate their resources to enforce traffic laws more during rush hour, and that drivers on the road should drive with more caution during these hours.





## Question 2:


Question: 
Which streets record the highest frequency of crashes, and what types of traffic controls were in place at the time of these incidents on those particular streets?

Importance: 
Correlating road names with the number of crashes helps identify high-risk areas and implement targeted safety measures. Understanding which roads have more accidents allows authorities to focus resources where they're needed most, improving overall road safety. It also informs public awareness efforts to promote caution on roads with a higher frequency of crashes.
Correlating traffic controls with car crashes is crucial for understanding and improving road safety. Traffic controls, such as stop signs, traffic lights, and yield signs, regulate the flow of traffic and mitigate potential conflicts between vehicles. Analyzing the presence or absence of these controls at crash sites can help identify patterns. 

<img width="470" alt="image" src="https://github.com/nathanrockwell/MIST4610-Project-2/assets/148256894/47d7d196-427c-4634-9039-56bf1e153434">

This heat map shows the most dangerous streets, namely the most dangerous streets are Connecticut Ave, Frederick Rd, Georgia Ave, New Hampshire Ave, and Rockville Pike.

<img width="467" alt="image" src="https://github.com/nathanrockwell/MIST4610-Project-2/assets/148256894/a8870e2e-5764-49ee-b6ed-59e3b24236b6">

This graph shows that the primary controls on the most dangerous streets include a prevalence of no controls and street lights, while secondary controls like stop signs, yield signs, and flashing traffic signals are notably low. These findings underscore a critical need for heightened safety measures on these roadways. Implementing targeted interventions, such as increased signage or additional traffic signals, may be essential to address the identified risk factors and enhance overall road safety. The data provides valuable insights for local authorities to prioritize and allocate resources effectively, mitigating the frequency of accidents on these specific streets.




## Manipulations applied to the data set for analysis:
We used Tableau's "Cleaned with Data Interpreter" to refine our dataset for analysis. This tool transformed raw data into an optimal format for nuanced examination. The dataset, designed for clarity, includes quantitative and semantically rich information. Rigorous purging removed duplicates, extraneous variables, and inaccuracies. Tableau's Data Interpreter ensured data integrity by addressing incomplete or aberrant entries. Attention to formatting excluded disruptive third-party imports. The resultant dataset is a refined, internally consistent foundation for use in Tableau.
## Tableau packaged workbook

The packaged workbook containing the visualizations shown above is attached to this repository.


