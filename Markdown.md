# Peaceful Protests in Jammu and Kashmir Peaked in 2021
 
### ANANYA TIWARI <br><br>
 
Dataset at: https://docs.google.com/spreadsheets/d/1xkkj_kNYFCDJ2xIho91ygNlUp186rOAyhxiNq_sr6AY/edit?usp=sharing <br><br>
 
DATA FROM: Armed Conflict Location & Event Data Project (ACLED)<br><br>
 
Jammu and Kashmir, which contains Kashmir, India’s contested state, witnessed increased peaceful protests as well as insurgency and violence since 2016. This trend peaked in 2021. The entire region was under a harsh lockdown for 2 years from 2019 when the central government revoked Article 370. <br><br>

### History <br><br>

After the Partition of the British-ruled subcontinent in 1947, Kashmir, which was and continues to be Muslim-dominated, was taken over by the new Indian government and military rule ensued. Article 370 of the Indian constitution gave the state (comprising also the region of Jammu, which is Hindu-dominated) a special status. This gave the region the right to have a separate flag, state constitution, and internal governance constituting Kashmiri and Jammu locals in the government. Despite this, Kashmir was conflict-ridden and ruled by the military. <br><br>

Citing that Article 370 had fed the flames of separatism, the BJP-ruled central government revoked it and separated the regions into two Union Territories (administered directly by the central government only without an option of elections) of Jammu and Kashmir, and Ladakh respectively. This revocation of August 2019 was followed by a stringent state-wide lockdown which lasted till 2021. Curfews, disconnection of the internet, and communication blockades were justified as a means to control anticipated violence and unrest following this revocation. <br><br>

### Data shows increased protest activity in the region since 2016 <br><br>

The ACLED’s data shows that in states such as J&K, Punjab, and Odisha, there have been increasing riots, violence, and peaceful protests since 2016. The data tracks incidents of arrests, armed clashes, mob violence, peaceful protests, violent demonstrations, excessive force against protesters, and many others.<br><br>

The J&K region saw over 18,000 incidents and topped all the states over the period of 2016. However, most incidents reported were peaceful protests. Only Punjab - which rebelled against the 3 farm laws from July 2020 - witnessed more protests than the region. These protests - both in the region and in Punjab - peaked in 2021. This is despite the 2-year lockdown in the Jammu and Kashmir region - which included the suspension of the internet - and the COVID-19 pandemic across the country. <br><br>


!['Peaceful protests across the country from 2016-22'](/MAP.jpg) <br>
(Darker areas saw more incidents, period 2016-22)<br><br>



!['J&K saw most incidents overall'](/two.png)<br><br>
Peaceful protests in J&K occurred far more than the violent clashes.<br><br>

 
!['J&K saw more peaceful protests than other incidents'](/three.jpg)<br><br>

Despite the fact that a harsh lockdown was imposed and military rule by India intensified in the Kashmir region from 2019 onwards, peaceful protests continued to occur, and actually peaked in 2021. The lockdown was lifted on September 2021, more than 2 years after the imposition of lockdown on August 5, 2019. Yet, protests continued unabated during this entire period. <br><br>

Since only a few months of 2022 have passed, the instances are lesser this year as of now. <br><br>



!['J&K saw more peaceful protests peak in 2021, and these have been growing over the course of 6 years’](/four.jpg)<br><br>

The protests have been at a historic high and escalated immensely. Even though they show a slight dip during the lockdown period (2019-2021), they peaked in 2021, possibly due to the fact that the lockdown was lifted then. <br><br>

Intriguingly, the trend of rising peaceful protests in many Indian states - instigated or led by a wide variety of people, including political parties, students, unions, etc - have shown an immense rise over the course of the years. This is especially true for those states with the most incidents, such as Punjab and Assam. Their trends are similar to what is seen in Jammu and Kashmir. <br><br>

!['Protests trend similar to that of other states with lots of activity’](/five.jpg)<br><br>

Peaceful protests have been rising steadily over the years in India in many states, though the causes are multiple, and participants are diverse groups including those of opposing political parties, unions and student groups. Over 74,000 overall peaceful protests were recorded from 2016 onwards. <br><br>



!['Protests have increased in states with most reported incidents of this activity’](/six.jpg)<br><br>

States such as J&K, Punjab, Assam, Tamil Nadu, Telangana, West Bengal, Uttar Pradesh, and others (except for Delhi and Haryana) have witnessed increasing protest activity recently, often peaking in 2019. <br><br><br>
 
## **MARKDOWN** <br><br>
 
In this dataset collected by the ACLED, events in India from 2016-2022 - such as peaceful protests, riots, insurgency, police violence, mob violence - has been recorded. They are collected via news reports. My goal in this analysis was to figure out any obvious trends. <br><br>
 
1. Even though the data set looked clean, I opened it via OpenRefine. <br><br>
2. I could individually use the cluster/facet functions to explore each column. <br><br>
For example, when I used the text facet on the Sub_event_type (which states what form of event occurred such as mob violence, peaceful protests, etc), I could see for myself the various kinds of activity that have been recorded. <br><br> 
3. I immediately noticed that “Peaceful protest” was recorded 74544 times, way higher than any other activity. Image below shows this:<br><br><br>
 
!['Peaceful protests are highest'](/numberone.jpg) <br><br><br>
 
4. Similarly, the text facet for the “year” column revealed the most occurrences that happened in 2019. <br><br>
5. The occurrences peaked in 2019, and then dropped. <br><br>
6. I opened the file on Google sheets. <br><br>
7. I froze the rows displaying the headers. <br><br>
8. I opened a PIVOT TABLE.<br><br>
 
9. Checking the states, Jammu & Kashmir and Punjab saw most activities occur during all the years. However, Punjab saw the most peaceful protests (over 11,000 versus over 9,000 in J&K), even though overall, most activities occurred in J&K. This can be explained as since 2020 farmers across Punjab were ferociously and relentlessly agitating against the 3 farm laws passed in July 2020. <br><br>
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
 
 
 
14. In 2019 the Indian government repealed Article 370 which granted a special status to J&K. This abrogation was followed by an intense statewide lockdown for months, including cutting off the internet. This was lifted, very slowly, only in 2021. Yet, protests peaked in 2021, showing that there seems to be a lot of activity in the state despite a harsh lockdown. Even during the lockdown data shows that peaceful events, as well as violence, continued. <br><br>
15. To show this trend of events, I opened up another pivot table. <br><br>
16. PIVOT TABLE: ROWS: sub_event_type, admin1 and year (in that order) and Values: Sub_event_type shows the “J&K Trends over the years” for Peaceful Protests.<br><br><br>
 
 !['Peaceful protests in J&K over the years'](/numberthree.jpg)<br><br> <br>
 
 
17. Peaceful protests reduced drastically in 2021 in J&K. <br><br>
 
18. Creating a **QGIS map** illustration to show the intensity of peaceful protests in J&K and other states of India since 2016. <br><br>
19. I copied “STATES EVENTS” onto a separate Google sheet, and downloaded it to the computer. I named this file “QGIS”. It can be found here: https://docs.google.com/spreadsheets/d/1e6hUkkGKETSvNupdqudCt46fSAIdtfG-2rsTz6zJNsc/edit?usp=sharing <br><br>
20. I downloaded an Indian state shapefile from the web. <br><br>
21. In QGIS, I added it as a new vector layer. <br><br>
22. I then added the CSV file (QGIS) by adding a delimited text file layer, and in Geometry chose no geometry as no coordinates are mentioned. <br><br>
23. I right-clicked the map layer and selected Join, and added the CSV file to it.<br> I matched the STATES with the NAME_1 (I checked the attribute table for the shapefile and saw that the state names were given as this). <br><br>
24. I right-clicked the map layer again and went to its Properties, wherein Symbology I selected the Categorize option for EVENTS. I chose the graduated range. <br><br>
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
 
* The following chart shows that for all these states peaceful protests dropped significantly since 2021, during the height of the pandemic. However, they peaked in 2020-21. <br>
* In 2020 however, even as the pandemic was ongoing and a lockdown was imposed in J&K, protest movements continued J&K, Punjab. <br><br>
* In Punjab, since 2020, farmers have been fighting and agitating against the 3 farm laws that were passed. In J&K, people have been protesting against the abrogation of Article 370, among other issues. <br><br>
* The farmer movement was also present in Uttarakhand and thus the protests occurred there too. <br><br>
 
### **Conclusion** <br><br>
**Since 2021, protest movements in  states have fallen sharply, even in the conflict region of J&K.** <br><br>
34. This infographic can be found at: https://infogram.com/chart-project-ananya-tiwari-1hxr4zxl737gq6y <br><br>
35. For this story, I contacted the ACLED as well as Fahad Khan. ACLED responded but has not gotten back to me yet. Fahad Khan, who runs a publication in Kashmir, unfortunately, got arrested for his work. <br><br><br>
 
##Writing the story <br><br>
 
While writing the story, I realized that I more charts.<br><br>
 
36. For each of the charts mentioned in the story, I copied and pasted the data from the main file to a separate sheet after working on it with a pivot table. I used Infogram to do this. <br><br>
37. For example, for the last chart showing how peaceful protests have increased in general across various states, I opened a new pivot table, took that data to a separate Google sheet, and created a chart for it on Infogram.<br><br>
. !['Analyzing data using pivot tables’'](/six.jpg)
 
**Reports**<br><br>
 
* 87 civilians, 99 security personnel killed in J&K since Article 370 scrapped: https://www.theweek.in/news/india/2022/04/06/87-civilians-99-security-personnel-killed-in-jandk-since-article-370-scrapped.html <br><br>
* 1,999 stone-pelting incidents in 2019 in J-K, 1,193 post abrogation of Article 370: https://economictimes.indiatimes.com/news/politics-and-nation/1999-stone-pelting-incidents-in-2019-in-j-k-1193-post-abrogation-of-article-370/articleshow/73129411.cms?utm_source=contentofinterest&utm_medium=text&utm_campaign=cppst <br><br>
* A New Phase of Militancy in Kashmir: Challenges for India: https://www.mei.edu/publications/new-phase-militancy-kashmir-challenges-india <br><br>
* India’s Kashmir Conundrum: Before and After the Abrogation of Article 370: https://drive.google.com/file/d/1LlEJbbakb8mhkXZSM18D78hzdNnJMK3d/view?usp=sharing <br>
Lalwani, Sameer P., and Gillian Gayner. India’s Kashmir Conundrum: Before and After the Abrogation of Article 370. US Institute of Peace, 2020, http://www.jstor.org/stable/resrep25405. Accessed 28 Apr. 2022.<br><br>
* Communication blackout and media gag: State-sponsored restrictions in the conflict-hit region of Jammu and Kashmir: https://drive.google.com/file/d/1W-amFIJgXwqW-GjXkChhBNDKtdwTQOFC/view?usp=sharing <br> Pandow, Bilal Ahmad. “Communication Blackout and Media Gag: State-Sponsored Restrictions in Conflict-Hit Region of Jammu and Kashmir.” Identities (Yverdon, Switzerland) ahead-of-print. ahead-of-print 1–20. Web. <br><br>
 
**About the ACLED Dataset** <br><br><br>
 
This dataset contains riots that took place in India along with the actors and geolocations. This record ranges from 1997-to 2022 and has 50,000+ records. This data is collected from ACLED. The Armed Conflict Location & Event Data Project (ACLED) is a non-governmental organization specializing in disaggregated conflict data collection, analysis, and crisis mapping. ACLED codes the dates, actors, locations, fatalities, and types of all reported political violence and demonstration events around the world in real-time. As of 2022, ACLED has recorded more than 1.3 million individual events around the world. The ACLED team conducts analysis to describe, explore, and test conflict scenarios, making both data and analysis open for use by the public.<br><br><br>
 
 

