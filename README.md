# BATB Automation desk data and project governance <br> 
N.B: The data governance regulation has been set based on the data collected from public survey acting as the justification of the regulations. Find the excel file(BATB DBS Automation Desk Data Governance Test Feedback) in this repository to see the detailed data.<br> 

<h1>PowerApps Data source</h1><br>
1. Excel is not recommended to use as a data source because of it's sharing issue. justification: Excel data can only be shared within BAT environment but the sharing modality works only in individual links. that means anyone without the link can not access or need to hit the link at least once which is not feasible. <br>
2. Use SharePoint list as data source. Justification: SharePoint can be shared with everyone in BAT modality. This is very convenient to use and there are no issues with access. <br>
3.SharePoint list settings for best outcome is as below: <br>
a. Settings > b. Site Permissions > c. Advanced permissions Settings > <br>
d. If Some content on this site has different permissions from what you see here.  Show these items. <br>
or <br> 
e. Grant Permissions> f. Everyone except external users <br>
g. Select members , visitors and users > h. edit user permissions > i. Contribute > j. select ok <br> 
4. Adding this seting will block users to make changes to sharepoint list. But keep in note that this will still allow item level permissions. That means user can edit / delete their/others data. <br>
 <h1>PowerApps</h1><br>
1. Create all apps through DB Automation Desk service account <br> 
2. Go to File > Share and Add Everyone in BAt as User this will allow everyone to get direct access to the app. <br>
3. In case if you are using Excel as data source you need to keep that in one drive and share that as public and then add in powerApps data source <br> 
4. While using excel make sure it is not open anywhere or else the app can not read or write. <br> 
<h1>Power Automate Data source</h1><br>
1. Excel and SharePoint both can be used as Power Apps data source <br>
2. The dafault limit of Excel as data source is 255 rows but it can be tweaked upto 5000 by pagination 
