# COVID-19 Open Research Dataset (CORD19) analysis
repository about articles related to coronaviruses, using data from the CROD19 Kaggle challenge.

# Description of the data file 
Datafile 'CORD19_Geo_info.csv'

### The notebook 'covid_articles_geoMap.ipynb' in notebooks folder of the repo extracts authors information from the CORD19 kaggle data set and creates a dataframe as a .csv file. The Schema for the csv file is as follows:


#### format in which each row is entered  --- PaperId, Title, Authors, Institutes, PostalCodes, Countries

Since a paper can have multiple authors, their names have been registered as strings with names separated with semi-colon (;).
Then each authors affiliation info is sequentially stored in the .csv file


for example if a paper P1 has:

authors --- a1,a2,a3 

affiliations --- I1,I2,I3, 

postal codes ---- postcode1,postcode2,postcode3, 

countries ---- c1,c2,c3 

respectively then the row entry would look like

P1_id , Title_of_P1 , a1;a2;a3 , I1;I2;I3 , postcode1;postcode2;postcode3 , c1;c2;c3

Note - Each authors name is as follows = first_middle_last

## Researh Questions

1. Perform some basic network analysis on the CORD19 dataset provided by kaggle 
(Link to dataset - https://www.google.com/url?q=https://www.kaggle.com/allen-institute-for-ai/CORD-19-research-challenge&sa=D&source=hangouts&ust=1586857198871000&usg=AFQjCNGetfltrYHXAgGPK2d67a_mlkP03Q)
to find the network of  
a) collaboration between researchers
b) collaboration between countries
c) major contributing institutes

2. Construct the citation graph from references information to construct a pathway of ideas on corona virus research

3. Observe how ideas are created and then accepted in a community by looking at the papers text content   --- This needs to be clarified 
