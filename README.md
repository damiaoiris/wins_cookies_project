## COOKIE: Community Observation On cooKie dIstribution on the intErnet

##### Authors
&Iacute;ris Dami&atilde;o, Elena Candellone, Gabriela Juncosa, Emma Crenshaw, Sabina Adhikari, and Adeola Adegbemijo

### PURPOSE
This repo was created as part of the Women in Network Science Collabathon 2023. It investigates whether companies differentiate between websites that contain misinformation versus those that do not when considering where to place cookies for advertising, tracking, etc.

### DATA

The data (companies_cookie_data) contains information about cookies obtained by two bots while visiting websites.

Relevant columns in the dataset:

* _site_visit_url_: websites the bot has visited
* _crawl_: This database only has non - disinformation websites (pilot_1_US_base) and disinformation websites (pilot_1_US_misinfo)
* _is_third_party_: cookie is set by the domain visited (first-party) or by another domain = third_party (third-party)
* _ps_plus_1_: domain of the third-party website
* _disconnect_tracker_category_: if the third-party is associated with some type of content/function (Advertisement, Social, Fingerprinting...) that information is in this column. If no type was recorded, the column is NaN
* _companies_: Big company behind the third-party

*(Please don't use this data outside the project)*


### Code 
The Jupyter notebook generates a community-finding stochastic block model as well as several plots to explore the content of the communities. Packages used in the modeling age available from https://github.com/martingerlach/hSBM_Topicmodel.

