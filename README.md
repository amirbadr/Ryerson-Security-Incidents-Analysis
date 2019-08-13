# Ryerson-Security-Incidents-Analysis
In this project, we programmatically analyzed Security incident reports at Ryerson University. <br />
Ryerson University security website provides daily update on nearly all the security incidents which happen near Ryerson University. All Ryerson students, faculty, staff and alumni receive security incident notices directly via their Ryerson email address. You can check the [Ryerson Universty Security Incidents](https://www.ryerson.ca/community-safety-security/security-incidents/list-of-security-incidents/) website.
### Details included in security incidents
- times and dates of incident;
- general location of incidents;
- details of the suspect; and
- details on arrests in relation to a previous incident,

## In this analysis, we analyzed the detail of incidents in the following steps:
1- We scraped all the incident titles, times and dates of incidents, and the general location of incidents on 20 incident pages using Folium and Pandas package in Python.<br />
2- We extracted the web page for all incidents and we extracted the Incident details and Description information in order to further analyze the gender of the suspect. We used Requests, Beautiful Soup, Seaborn, Matplotlib, and Pandas packages.<br />
3- We further analyzed the incident descriptions and provided the most important words using Term frequency-inverse document frequency and provided the result on Word cloud using Word cloud package .<br />
