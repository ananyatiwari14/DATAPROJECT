# COVID-19 in 2021 LEADS TO SHARP FALL IN PEACEFUL PROTESTS IN INDIA
### ANANYA TIWARI <br><br>

Dataset at: https://docs.google.com/spreadsheets/d/1xkkj_kNYFCDJ2xIho91ygNlUp186rOAyhxiNq_sr6AY/edit?usp=sharing <br><br>

FROM: Armed Conflict Location & Event Data Project (ACLED)<br><br>

MARKDOWN<br><br>

Even though the data set looked clean, I opened it via OpenRefine. <br>
Open Refine helps in clustering data. With this, I could individually use the cluster/facet functions to explore each column. <br>
For example, when I used the text facet on the Sub_event_type (which states what form of event occurred such as mob violence, peaceful protests, etc), I could see for myself the various kinds of activity that have been recorded. I immediately noticed that “Peaceful protest” was recorded 74544 times, way higher than any other activity. Image below shows this:<br><br>

!['Peaceful protests are highest'](/numberone.jpg) <br><br>



Similarly, the text facet for the “year” column revealed the most occurrences happened in 2019. The occurrences peaked in 2019, and then dropped. <br>
I opened the file on Google sheets. <br>
I froze the rows displaying the headers. <br>
I opened a PIVOT TABLE.<br>

Checking the states, Jammu & Kashmir and Punjab saw most such activities. <br>
With these facets, I could already see that the trends are : most of these activities are peaceful protests, these activities peaked in 2019, and have dropped significantly since, especially from 2020 onwards. <br>
Since I did not need to clean up anything, I did not download this OpenRefine file and opened up this CSV on Google sheets for further analysis. <br>
After opening up Google Sheets, I froze the top row and opened a PIVOT TABLE. <br>

I opened a pivot table for the main sheet and in ROWS - admin1, event_type | VALUES - eventy_type. <br>

For J&K, it showed that though riots occurred a lot, peaceful protests were by far the most common occurrence. This data shows events from 2016-22 <br><br>

| Jammu and Kashmir       	| Battles                    	| 3468  	|
|-------------------------	|----------------------------	|-------	|
|                         	| Explosions/Remote violence 	| 532   	|
|                         	| Protests                   	| 10288 	|
|                         	| Riots                      	| 2655  	|
|                         	| Strategic developments     	| 336   	|
|                         	| Violence against civilians 	| 826   	|
| Jammu and Kashmir Total 	|                            	| 18105 	|

<br><br>



In 2019 the Indian government repealed Article 370 which granted a special status to J&K. This abrogation was followed by an intense statewide lockdown for months, including cutting off of the internet. This was lifted, very slowly, only in 2021. One of the reasons the events came down during this period is this. <br>
To show this reduction of events, I opened up another pivot table. <br>
PIVOT TABLE: ROWS: sub_event_type, admin1 and year (in that order) and Values: Sub_event_type shows the “J&K Trends over the years” for Peaceful Protests.<br><br>
 
 !['Peaceful protests in J&K over the years'](/numberthree.jpg)<br><br> 


These have also reduced, along with other events. 

Creating a QGIS map illustration to show that most peaceful protests and other events are occurring in J&K. 
I copied “STATES EVENTS” onto a separate Google sheet, and downloaded it to the computer. I named this file “QGIS”. It can be found here: https://docs.google.com/spreadsheets/d/1e6hUkkGKETSvNupdqudCt46fSAIdtfG-2rsTz6zJNsc/edit?usp=sharing 
I downloaded an Indian state shapefile from the web. 
In QGIS, I added it as a new vector layer. 
I then added the CSV file (QGIS) by adding a delimited text file layer, and in Geometry chose no geometry as no coordinates are mentioned. 
I right-clicked the map layer and selected Join, and added the CSV file to it. I matched the STATES with the NAME_1 (I checked the attribute table for the shape file and saw that the state names were given as this). 
I right-clicked the map layer again and went to its Properties, where in Symbology I selected the Categorize option for EVENTS. I chose the graduated range. 
In the Layer section, I chose to label the states too. 

The PDF version of this map is: https://drive.google.com/file/d/1mKUfn8rlUNSR83WPK3h0HeCFHIIQi3Pd/view?usp=sharing 

Now, I wished to show how peaceful protests are progressing over the years since 2016. For this, I chose to create a line chart. For this I chose Infogram. 
I copy-pasted the data on “J&K peaceful protest trends” to another google sheet and named it under the same name.
I wished to compare the trend of J&K with a few other states. Thus, in this new sheet, I copy-pasted the trend values (from the PIVOT TABLE) to adjacent columns. This Sheet can be found here: https://docs.google.com/spreadsheets/d/1SO9e2vtwBisjzgawprUcDgCkWye_J3tUzIgnBzqgSfU/edit?usp=sharing 
I chose the states which were darker (or with more peaceful protest events occurring). These are Punjab, Uttaranchal (or Uttarakhand). I also chose to include Assam. 

I downloaded this CSV file to the computer under the same name. 
In a new Infogram for a line chart, I imported this CSV. 
The result is as follows:

The following chart shows that for all these states peaceful protests dropped significantly since 2021, during the height of the pandemic. In 2020 however, even as the pandemic was ongoing, protest movements peaked in J&K, Punjab. In Punjab, since 2020, farmers have been fighting and agitating against the 3 farm laws that were passed. This movement was also present in Uttarakhand. However for Assam, since COVID-19, it has been a reduction. 
Since 2021, due to COVID-19, protest movements in these states with most events have fallen sharply. 
This infographic can be found at: https://infogram.com/chart-project-ananya-tiwari-1hxr4zxl737gq6y 
For this story, I contacted the ACLED as well as Fahad Khan. ACLED responded but has not gotten back to me yet. Fahad Khan, who runs a publication in Kashmir, unfortunately, got arrested for his work. 

About the Dataset: 

Context
This dataset contains riots that took place in India along with the actors and geolocations. This record ranges from 1997-to 2022 and has 50,000+ records. This data is collected from ACLED. The Armed Conflict Location & Event Data Project (ACLED) is a non-governmental organization specializing in disaggregated conflict data collection, analysis, and crisis mapping. ACLED codes the dates, actors, locations, fatalities, and types of all reported political violence and demonstration events around the world in real-time. As of 2022, ACLED has recorded more than 1.3 million individual events around the world.[1] The ACLED team conducts analysis to describe, explore, and test conflict scenarios, making both data and analysis open for use by the public.
