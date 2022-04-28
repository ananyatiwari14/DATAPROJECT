# COVID-19 in 2021 LEADS TO SHARP FALL IN PEACEFUL PROTESTS IN INDIA
### ANANYA TIWARI <br><br>

Dataset at: https://docs.google.com/spreadsheets/d/1xkkj_kNYFCDJ2xIho91ygNlUp186rOAyhxiNq_sr6AY/edit?usp=sharing <br><br>

FROM: Armed Conflict Location & Event Data Project (ACLED)<br><br>

## **MARKDOWN** <br><br>

In this dataset collected by the ACLED, events in India from 2016-2022 - such as peaceful protests, riots, insurgency, police violence, mob violence - has been recorded. They are collected via news reports. My goal in this analysis was to figure out any obvious trends. <br><br>

1. Even though the data set looked clean, I opened it via OpenRefine. <br><br>
2. I could individually use the cluster/facet functions to explore each column. <br><br>
For example, when I used the text facet on the Sub_event_type (which states what form of event occurred such as mob violence, peaceful protests, etc), I could see for myself the various kinds of activity that have been recorded. <br><br> 
3. I immediately noticed that “Peaceful protest” was recorded 74544 times, way higher than any other activity. Image below shows this:<br><br><br>

!['Peaceful protests are highest'](/numberone.jpg) <br><br><br>



4. Similarly, the text facet for the “year” column revealed the most occurrences happened in 2019. <br><br>
5. The occurrences peaked in 2019, and then dropped. <br><br>
6. I opened the file on Google sheets. <br><br>
7. I froze the rows displaying the headers. <br><br>
8. I opened a PIVOT TABLE.<br><br>

9. Checking the states, Jammu & Kashmir and Punjab saw most activities occur during all the years. However, Punjab saw most number of peaceful protests (over 11,000 versus over 9,000 in J&K), even though overall, most activities occured in J&K. This can be explained as since 2020 farmers across Punjab were ferociously and relentlessly agitating against the 3 farm laws passed in July 2020. <br><br>
10. With these facets, I could already see that the trends for all states are the following: <br>
 *Most of these activities are peaceful protests. <br>
 *These activities peaked in 2019. <br>
 *They have dropped significantly since, especially from 2020 onwards. <br><br>
Since I did not need to clean up anything, I did not download this OpenRefine file and opened up this CSV on Google sheets for further analysis. <br><br>

11. After opening up Google Sheets, I froze the top row and opened a PIVOT TABLE. <br><br>

12. I opened a pivot table for the main sheet and in ROWS - admin1, event_type | VALUES - eventy_type. <br><br>

13. For J&K, it showed that though riots occurred a lot, peaceful protests were by far the most common occurrence. This data shows events from 2016-22 <br><br><br>

| **Jammu and Kashmir**       	| **Battles**                    	| **3468**  	|
|-------------------------	|----------------------------	|-------	|
|                         	| Explosions/Remote violence 	| 532   	|
|                         	| Protests                   	| 10288 	|
|                         	| Riots                      	| 2655  	|
|                         	| Strategic developments     	| 336   	|
|                         	| Violence against civilians 	| 826   	|
| **Jammu and Kashmir Total** 	|                            	| **18105** 	|

<br><br><br>



14. In 2019 the Indian government repealed Article 370 which granted a special status to J&K. This abrogation was followed by an intense statewide lockdown for months, including cutting off of the internet. This was lifted, very slowly, only in 2021. One of the reasons the events came down during this period is this. Yet, data shows that despite the lockdown, peaceful events as well as violence continued. <br><br>
15. To show this trend of events, I opened up another pivot table. <br><br>
16. PIVOT TABLE: ROWS: sub_event_type, admin1 and year (in that order) and Values: Sub_event_type shows the “J&K Trends over the years” for Peaceful Protests.<br><br><br>
 
 !['Peaceful protests in J&K over the years'](/numberthree.jpg)<br><br> <br>


17. Peaceful protests too have reduced, along with other events. But they continued through 2019-20, when the lockdown was imposed. <br><br>

18. Creating a **QGIS map** illustration to show that most peaceful protests and other events are occurring in J&K. <br><br>
19. I copied “STATES EVENTS” onto a separate Google sheet, and downloaded it to the computer. I named this file “QGIS”. It can be found here: https://docs.google.com/spreadsheets/d/1e6hUkkGKETSvNupdqudCt46fSAIdtfG-2rsTz6zJNsc/edit?usp=sharing <br><br>
20. I downloaded an Indian state shapefile from the web. <br><br>
21. In QGIS, I added it as a new vector layer. <br><br>
22. I then added the CSV file (QGIS) by adding a delimited text file layer, and in Geometry chose no geometry as no coordinates are mentioned. <br><br>
23. I right-clicked the map layer and selected Join, and added the CSV file to it.<br> I matched the STATES with the NAME_1 (I checked the attribute table for the shape file and saw that the state names were given as this). <br><br>
24. I right-clicked the map layer again and went to its Properties, where in Symbology I selected the Categorize option for EVENTS. I chose the graduated range. <br><br>
25. In the Layer section, I chose to label the states too. <br><br>

!['States in India with most peaceful protests'](/MAP.jpg)<br><br> <br>

26. The PDF version of this map is: https://drive.google.com/file/d/1mKUfn8rlUNSR83WPK3h0HeCFHIIQi3Pd/view?usp=sharing <br><br>

27. Now, I wished to show how peaceful protests are progressing over the years since 2016. For this, I chose to create a line chart. For this I chose *Infogram*. <br><br>
28. I copy-pasted the data on “J&K peaceful protest trends” to another google sheet and named it under the same name.<br><br>
29. I wished to compare the trend of J&K with a few other states. Thus, in this new sheet, I copy-pasted the trend values (from the PIVOT TABLE) to adjacent columns. This Sheet can be found here: https://docs.google.com/spreadsheets/d/1SO9e2vtwBisjzgawprUcDgCkWye_J3tUzIgnBzqgSfU/edit?usp=sharing <br><br>
30. I chose the states which were darker (or with more peaceful protest events occurring). These are Punjab, Uttaranchal (or Uttarakhand). I also chose to include Assam. <br><br>

31. I downloaded this CSV file to the computer under the same name. <br><br>
32. In a new Infogram for a line chart, I imported this CSV. <br><br>
33. The result is as follows:<br><br>

 !['Peaceful protests over the years'](/Infogram.jpg)

* The following chart shows that for all these states peaceful protests dropped significantly since 2021, during the height of the pandemic. <br>
* In 2020 however, even as the pandemic was ongoing and a lockdown was imposed in J&K, protest movements peaked in J&K, Punjab. <br><br>
* In Punjab, since 2020, farmers have been fighting and agitating against the 3 farm laws that were passed. <br><br>
* The farmer movement was also present in Uttarakhand and thus the protests occured. <br><br>
* However for Assam, since COVID-19, it has been a reduction. <br><br>
##Conclusion: Since 2021, due to COVID-19, protest movements in these states with most events have fallen sharply. <br><br>
34. This infographic can be found at: https://infogram.com/chart-project-ananya-tiwari-1hxr4zxl737gq6y <br><br>
35. For this story, I contacted the ACLED as well as Fahad Khan. ACLED responded but has not gotten back to me yet. Fahad Khan, who runs a publication in Kashmir, unfortunately, got arrested for his work. <br><br><br>

**About the Dataset** <br><br><br>

This dataset contains riots that took place in India along with the actors and geolocations. This record ranges from 1997-to 2022 and has 50,000+ records. This data is collected from ACLED. The Armed Conflict Location & Event Data Project (ACLED) is a non-governmental organization specializing in disaggregated conflict data collection, analysis, and crisis mapping. ACLED codes the dates, actors, locations, fatalities, and types of all reported political violence and demonstration events around the world in real-time. As of 2022, ACLED has recorded more than 1.3 million individual events around the world. The ACLED team conducts analysis to describe, explore, and test conflict scenarios, making both data and analysis open for use by the public.<br><br><br>
