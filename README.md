# USA-Locations
- USA Locations repository demostrates how to use global vertices and edges for multiple graphs. See the DDLs/Schema/useGlobalSchema.gsql file on how to define and use Global vertices and edges with a local graph. This approach will allowing you to define "reference" data to be loaded once and reused in specific local graphs. This ensures enterprise-wide data consistency and integrity, reducing redundancy.
  
- USA Locations data is from the U.S. Census American Community Survey - Year 2023. The data includes Continent, Country, Region, Divison, State, County and City and Demographs.

## Install and Run
### Install
To install this USA-Locations demo, clone this repository at a terminal command prompt: 
- \>git clone https://github.com/custom-discoveries/USA-Locations.git
- cd USA-Locations
- prompt>Cheetah [^1]
  - Select -r if your running from a remote server
  - Select -l if your on running from the same server that is running TigerGraph database
  - Once logged in, select -b to load both the schema and the data.
[^1]: See Cheetah [README.md](https://github.com/custom-discoveries/Cheetah/blob/main/README.md) for installation and setup of Cheetah
### Install Queries
Once you have installed the Schemea and data, now create and install the queries.
- In Cheetah, select -q for query menu, then select -b to create and install all queries.
### List of Queries
- findCity - This query finds a city by either the fips code, or by city name
- findCounty - This query finds either all counties in the US or a county by State and City
- findDemographics - This query finds demographic statistics at the Zip level, when providing State and City parameters
- updateZipDemographics - This query will update the Zip Vertex with the state name
  
- Each of the queries has a 'UPDATE DESCRIPTION OF QUERY' commend that allows you to define the query description
#### Using Cheetah, under the query menu (-q), with the --details menu pick, you can display the query descriptions once the queries have been installed.
