# lots-and-spaces
Final Project for Map 671: Mapping Westchester County Parking Lots &amp; Open Spaces
#### [View map here](https://michael-sparks13.github.io/lots-and-spaces/)

## Project Lots And Spaces
Examines Parking Lots and Open Spaces in Westchester County, NY. Westchester is a 450 sq. mile county just a few minutes north of NYC. One million people live there and, if we think about our built environment as a physical manifestation of our vales, the relative amount of parking lots vs. open spaces in Westchester tells us a lot about what we value. 

## Findings and Areas for Futher Exploration
#### Findings
How Westchester uses its space:
- 11 sq miles of parking lots
- Over 42 sq miles of state & county parklands
- 31 sq miles of water supply lands (much of which provides NYC's water)
- 3 sq miles of cemetaries!
"Open space" is basically any non-built environment, including public & private parks. Water supply lands, and farms. 

Most of the county's parking lots are concentrated in two areas:
- along travel corridors like I-95 from north to south and 287 from east to west. 
- on the edges of the Bronx, particulary in Pelham Manor, Mount Vernon and Yonkers. 

What's more, the vast, vast majority of the county's parking lots are in the southern half of the county, below White Plains. 

The story starts to get really interesting when we add race into the mix. First, it's important to note that Westchester is a majority white:

- 52% White alone
- 26% Hispanic or Latino
- 17% Black or African American

White is the predominate race basically everywhere in the county except Yonkers and Mount Vernon. When we look at areas where the majority of the population is either Hispanic or Black, those areas correlate almost entirely with the major roads & transportation hubs.

Are Black and Hispanic persons in Westchester–one of the most affluent county's in the population–exposed to more car pollution than its White residents? More study is needed, but the data we have available raises important questions. 


#### Futher exploration
Westchester is typically known as an affluent county home to high powered executives who commute from their big houses with big lawns down to their big jobs with big offices on Wall St. But that's not the whole story. On its most southern end Westchester is more similar to the Bronx than to Beverly Hills. While in its northeastern sections, the county is much more rural. Cutting the spaces/races/lots divde by economic indicators would surely reveal some fascinating insights.

One other area of exploration: how do race & car ownership correlate? There are almost no pockets of Westchester that aren't serviced by MetroNorth Railroads where the predominate race is either Black or Latino. 


### Data
From Westchester County's GeoHub
- [Parking Lots](https://gis.westchestergov.com/datasets/parking-lots-1/explore?location=41.188605%2C-73.757497%2C12.39)
- [Open Spaces](https://gis.westchestergov.com/datasets/wcgis::open-space/explore?location=41.122403%2C-73.734250%2C11.00)
- [2020 Population By Race](https://gis.westchestergov.com/datasets/2020-population-by-race/explore?location=41.119013%2C-73.733550%2C11.00)

### Process and Tools
- After acquiring the data from Westchester County, I used QGIS for some exploratory analysis. Including querying the underlying data with SQL to calculate the relative areas for each type of space. 
- Then, I loaded the data as tilesets into Mapbox & began creating a new style (aka map)
- The original datasets did not have the zoom levels I wanted, so I used Tippecanoe and GDAL to add the levels I needed. Huge thanks to [Anya Prosvetova](https://www.prosvetova.com/blog/2021-08-15-mapbox-adjust-zoom-extent) for the best explainer out there. 
- Once all the correct data was loaded into Mapbox, it was a matter of testing out different designs. And different designs. And different designs. 
- Once I settled on design for the lots & spaces data that worked well with the basemap, I went back to add the "races" data. 
- I acquired the 2020 Population by Race data from Westchester County. 
- After exploring the data in Mapbox studio, I realized I needed it in a different format to make use of it. I used Jupyter Notebooks and Geopandas to create three unique geoJSON files that I could use (one for each race analyzed; notebook included in repo). 
- Similar to what I had to do with the lots & spaces data, I again used Tippecanoe to add the correct zoom layers. 
- Last, I used Mapbox GL JS to add the interactivity components. Thanks to the great Mapbox documentation for making this simple.
