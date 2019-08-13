# Ryerson-Security-Incidents-Analysis
In this project, we programmatically analyzed Security incident reports at Ryerson University. <br />
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
1. We scraped all the incident titles, times and dates of incidents, and the general location of incidents on 20 incident pages using Folium and Pandas package in Python.<br />
2. We extracted the web page for all incidents and we extracted the Incident details and Description information in order to further analyze the gender of the suspect. We used Requests, Beautiful Soup, Seaborn, Matplotlib, and Pandas packages.<br />
3. We further analyzed the incident descriptions and provided the most important words using Term frequency-inverse document frequency and provided the result on Word cloud using Word cloud package .<br />

### Time of the incident
