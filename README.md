# Ryerson-Security-Incidents-Analysis
In this project, I programmatically analyzed Security incident reports at Ryerson University. <br />
Ryerson University security website provides daily update on nearly all the security incidents which happen near Ryerson University. All Ryerson students, faculty, staff and alumni receive security incident notices directly via their Ryerson email address. You can check the [Ryerson University Security Incidents](https://www.ryerson.ca/community-safety-security/security-incidents/list-of-security-incidents/) website.
### Details included in security incidents
- times and dates of the incident;
- general location of incidents;
- details of the suspect; and
- details on arrests concerning the incident,

### In this analysis we tries to answer the following questions:
1. Where are the most dangerous locations at Ryerson University?
2. In which hour of a day do most of the security incidents happen at Ryerson University?
3. In which month and season do majority of the security incidents occur at Ryerson University?
4. What type of security incident is more common at Ryerson Univeristy?
5. What is the ratio of female suspects over male suspects involved at Ryerson Univeristy?

## In this analysis, we analyzed the detail of incidents in the following steps:
1. I scraped all the incident titles, times and dates of incidents, and the general location of incidents on 20 incident pages using Folium and Pandas package in Python.<br />
2. I extracted the web page for all incidents and we extracted the Incident details and Description information in order to further analyze the gender of the suspect. We used Requests, Beautiful Soup, Seaborn, Matplotlib, and Pandas packages.<br />
3. I further analyzed the incident descriptions and provided the most important words using Term frequency-inverse document frequency and provided the result on Word cloud using Word cloud package .<br />

# Result 
I programmatically extracted 200 security incidents from 2018-06-29 to 2019-08-03. Following is the result for each section:

### Time of incidents
I converted the string date column to pandas datetime column, then I converted to 24-hour time format and defined two-hours time buckets for the time. The following is the result of the hours with the highest number of incidents:

![time](https://user-images.githubusercontent.com/16935815/62913397-df716380-bd59-11e9-88a1-f6ac01305012.png)

### Location of incidents
I combined all the nearby locations, E.g Kerr Hall South and Kerr Hall West to Kerr Hall, and also duplciate locations such as "Victoria Street and Gould Street area", "Victoria Street and Gould Street", and "Gould Street and Victoria Street". In total, I could narrow down all the locations to 23 distinct locations at Ryerson University. Then I manually geo-located all these locations using Google Maps. The following is the result for the most dangerous locations:


![Location1](https://user-images.githubusercontent.com/16935815/62913787-80145300-bd5b-11e9-88a1-2f56ce0e34e9.png)


![location2](https://user-images.githubusercontent.com/16935815/62913802-8f939c00-bd5b-11e9-98e3-db650551060d.png)
