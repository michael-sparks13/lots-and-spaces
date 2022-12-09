# lots-and-spaces
Final Project for Map 671: Mapping Westchester County Parking Lots &amp; Open Spaces
#### [View map here](https://michael-sparks13.github.io/lots-and-spaces/)

## Project Lots And Spaces
Examines Parking Lots and Open Spaces in Westchester County, NY. Westchester is a 450 sq. mile county just a few minutes north of NYC. One million people live there and, if we think about our built environment as a physical manifestation of our vales, the relative amount of parking lots vs. open spaces in Westchester tells us a lot about what we value. 

## Findings and Areas for Futher Exploration
#### Findings
# write some major takeway
- 11 sq miles of parking lots
- 3 sq miles of cemetaries!
- Over 42 sq miles of state & county parklands
- 31 sq miles of water supply lands (much of which provides NYC's water)

#### Futher exploration
Westchester is typically known as an affluent county home to high powered executives who commute from their big houses with big lawns down to their big jobs with big offices on Wall St. But that's not the whole story. On its most southern end Westchester is more similar to the Bronx than to Beverly Hills. While in its northeastern sections, the county is much more rural. Cutting the spaces/races/lots divde by economic indicators would surely reveal some fascinating insights.


### Data
From Westchester County's GeoHub
- [Parking Lots](https://gis.westchestergov.com/datasets/parking-lots-1/explore?location=41.188605%2C-73.757497%2C12.39)
- [Open Spaces](https://gis.westchestergov.com/datasets/wcgis::open-space/explore?location=41.122403%2C-73.734250%2C11.00)

### Process and Tools
- After acquiring the data from Westchester County, I used QGIS for some exploratory analysis. Including querying the underlying data with SQL to calculate the relative areas for each type of space. 
- Then, I loaded the data as tilesets into Mapbox & began creating a new style (aka map)
- The original datasets did not have the zoom levels I wanted, so I used Tippecanoe and GDAL to add the levels I needed. Huge thanks to [Anya Prosvetova](https://www.prosvetova.com/blog/2021-08-15-mapbox-adjust-zoom-extent) for the best explainer out there. 
- Once all the correct data was loaded into Mapbox, it was a matter of testing out different designs. And different designs. And different designs. 
- Last, I used Mapbox GL JS to add the interactivity components. 


## to do
1) some of the in process details that you have listed on your index.html file and 2) a concluding thoughts/takeaway message section. After creating this map, are there any key findings that viewers should keep in mind? Any future maps that should be made to evaluate items further?
