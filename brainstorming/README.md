# Final Project Ideas for New Maps Plus MS
#### Lauren Oldham, January 2020

## 1. College Basketball Domination
I want to design a map that explores the trends in college basketball domination because I want to find out where the most powerful teams exist in order to help the audience have arguments about which team is the best. ;)
 
Building on my [final project for MAP-675](https://laurenoldham1202.github.io/ncaam-basketball/), I'd like to build a 
comprehensive web application that explores all 350 Division I college basketball programs in the United States. Whereas 
my 675 map only included schools that were in the top 50 winningest programs or had at least one National Championship 
title, I would like to include every D1 school with various filtering options to display the data.

### Goal
Have fun! I love college basketball and really like the idea of doing something personally enjoyable (and seasonably appropriate!) for my final project.
There is always a lot of discussion (ahem, argument) about who has the greatest program, the greatest conference, etc. so it would be great to provide a definitive source for all things CBB.
Maps are [wildly popular](https://www.reddit.com/r/CollegeBasketball/search?q=map&restrict_sr=on) over at [/r/CollegeBasketball](https://www.reddit.com/r/CollegeBasketball/), so I'm inspired to do something bigger and better than what currently exists.
My target audience includes /r/CollegeBasketball users, friends, coworkers, family, casual sports fans and fanatics alike.

### Outline/Notes
* Include data for all D1 schools
* Make table collapsible
* Make table filterable
* Make table sortable
* Style table row on click to semitransparent school color
* Update table ranking with each selected field
* Add school filtering options, e.g. display by conference, only top 50 winningest teams, only top win percentages, etc. 
* Add school logo image to popup
* Bonus: Add March Madness appearances, number of lottery picks, etc.
* Use scrollymapping to tell a story
* Create index for most dominant team overall?

### Limitations/Issues
* ~~This dataset doesn't exist! Might need to explore web scraping to avoid painful manual collection of all these datasets~~
Just kidding, the first dataset has a complete history of D1 schools!
* Break classes had to be manually created to create enough visual distinction between schools

### Sources
* [Historical college basketball statistics](https://www.sports-reference.com/cbb/schools/)
* [National Championship titles](https://en.wikipedia.org/wiki/NCAA_Division_I_Men%27s_Basketball_Tournament)
* [Top 50 overall winningest teams](https://en.wikipedia.org/wiki/List_of_teams_with_the_most_victories_in_NCAA_Division_I_men%27s_college_basketball)
* [Top 50 winning percentage teams](https://en.wikipedia.org/wiki/List_of_teams_with_the_highest_winning_percentage_in_NCAA_Division_I_men%27s_college_basketball)
* [Team colors 1](https://en.wikipedia.org/wiki/Module:College_color)
* [Team colors 2](https://teamcolorcodes.com/ncaa-color-codes/)
* [Team colors 3](https://usteamcolors.com/ncaa-division-1/)


* [Mapbox Interactive Storytelling](https://www.mapbox.com/solutions/interactive-storytelling)

### Literature
#### Examples of Interactive Sports Maps
* [College Footbal Fanbases](https://www.nytimes.com/interactive/2014/10/03/upshot/ncaa-football-map.html#5,42.944,-91.752)
* [All D1 College Basketball Teams](https://www.google.com/maps/d/u/0/viewer?dg=feature&ie=UTF8&oe=UTF8&msa=0&mid=1bXEv7hQrqKE6DccLudQ-oywpdZ0&ll=35.710909718852356%2C-113.24631124999996&z=4)
* [CBB Player Hometowns (app defunct)](http://www.thepostgame.com/every-ncaa-basketball-players-hometown-map)
* [North American Professional Championships](http://www.slate.com/articles/sports/sports_nut/2012/05/sports_championship_map_explore_every_championship_in_the_history_of_mlb_the_nba_the_nhl_and_the_nfl_.html)

#### Examples of Scrollymaps
* [Ridgecrest, CA Earthquakes](https://www.nytimes.com/interactive/2019/07/19/us/california-earthquakes.html)
* [Midwest Flooding](https://www.nytimes.com/interactive/2019/09/11/us/midwest-flooding.html?te=1&nl=morning-briefing&emc=edit_NN_p_20190912&section=topNews?campaign_id=9&instance_id=12323&segment_id=16950&user_id=f0e74355e8fe8b3573e180f2b848b4bd&regi_id=80404684tion=topNews)
* [Louisiana Toxic Air](https://projects.propublica.org/louisiana-toxic-air/)
* [Shape of Slavery](https://pudding.cool/2017/01/shape-of-slavery/)
* [North Korea Missile Range](https://www.abc.net.au/news/2017-10-16/north-korea-missile-range-map/8880894)
* [Earthquake Triggers](https://www.williamrchase.com/vizrisk/vizrisk_main/)
* [General Scrollytelling Examples](https://vallandingham.me/scroll_talk/examples/)

### Data Manipulation
Data for school histories of all historical D1 college basketball programs is saved in `data/cbb` as `d1-schools.csv`.

* Rename columns more sensibly
* Split school column to separate school friendly name and mascot
* Pull in additional dataset with full school names
* Split `City State` column into two columns
* Add column to differentiate between current and defunct D1 schools
* Add columns to differentiate between conferences
* Add team colors
* Add logos
* Add coaches? Players? Power 5 conference designation?
* Blue Bloods designation?
* Rivalries?
* Average distance traveled in March Madness?

Kansas > First NCAA national title win > UCLA > Blue Bloods > UK > All KY schools > UNC/Duke > Up and coming schools

Kansas > Blue Bloods > UCLA > Duke/UNC > UK > UK/UofL > All KY > All NC

## 2. March Madness Top Seed Sites Analysis
#### I want to design a map that analyzes and visualizes the tournament sites for top seeds in March Madness because I want to find out whether top teams are given geographical preference (as the seeding rules claim).

Tackling college basketball from a different approach, I'd like to explore the NCAA committee claim that top seeds in 
the tournament will play their first two games at sites "most geographically compatible to those teams." 
In short, the best teams of the year play closer to their fan base, which can give them home court advantage in the most 
upset-prone rounds of the tournament. While many factors go into assigning teams to different sites, it's always a 
contentious issue for fans - every fan base claims that they get screwed by the selection committee, whereas <opposing 
team I hate> gets preferential treatment! 
d
### Goal
Find out if any particular top teams are consistently given preferential locations over other top teams. It's a question
that I would like answered as a fan of college basketball.

### Outline/Notes
* Should probably limit data to modern March Madness seeding rules, beginning in 1985
* Use scrollymapping to show analysis highlights?
* Initial view: every school with a history of 1-4 seeds
* Popup/label with metadata, e.g. closest site, farthest site, average distance traveled as each seed, average distance traveled overall, etc.
* Mouseover or click on a school shows lines to each site (perhaps an animation flying to each site in great circle arc?)
* Dropdown or button toggle for each year, cards to show highlights and averages
* Add logos?
* Connect to overall seeding data
* Weighted average for distance and seed, weighted average for western schools?

### Limitations/Issues
* Data will need to be manually collected
* Not sure if there are any correlations - could be a lot of work with no significant results or visualizations
* The US is big! Most dominant teams are in the midwest/south/eastern, so the few dominant teams in the west often have 
to travel farther than eastern teams
* Not sure how I would visualize the data
* May need to brush up on some basic statistics

### Sources
* [Historical NCAA March Madness statistics](https://www.sports-reference.com/cbb/postseason/)

Relevant Literature:
* [NCAA Has a Geography Problem](https://www.thebiglead.com/2019/02/10/the-ncaa-tournament-has-a-geography-problem-and-should-move-a-western-venue/)
* [Selection Committee Rules](https://www.ncaa.com/news/basketball-men/article/2018-10-19/how-field-68-teams-picked-march-madness)

### Case Study
I wanted to take a quick look at the data to see if it would be suitable for a full analysis and visualization.

Data was manually compiled for years [2016](https://www.sports-reference.com/cbb/postseason/2016-ncaa.html), [2017](https://www.sports-reference.com/cbb/postseason/2017-ncaa.html), and [2018](https://www.sports-reference.com/cbb/postseason/2018-ncaa.html) and saved as `march_madness_161718.csv` in the `data/` directory.

QGIS Workflow:
1. CRS EPSG:32619
2. MMQGIS Geocoder plugin, OSM/Nominatim web service
3. Convert points to line, 'Order by...' and 'Separate by...' unique `id` field
4. Create new field in temporary lines file, `$length`/1069 for distance in miles
5. Spatial oin lines file back to points by `id` 

Data saved as `geocoded.shp` in `data/` directory. Note: West Virginia University was unsuccessfull geocoded.

## 3. Global Overtourism
As I've had the privilege of traveling more in my adult life, I've become more aware of overtourism and its effect on 
local communities worldwide. Many tourist destinations have always been hotspots, but have exploded in popularity as the
global middle class has grown, flight prices have fallen, and short-term rentals like AirBnb have been popularized. 
Other cities, such as Dubrovnik, Croatia, skyrocketed in popularity due to pop culture, but aren't equipped to handle 
the massive influx of tourists. I would love to explore the topic, but I haven't narrowed it down to a specific research 
problem.

### Limitations/Issues
* Most of the data is aggregated to the country level, but most of the overtouristed areas in the world are in Europe with smaller land area. A choropleth map won't be very visually interesting, but it might be the only option for data aggregation.

### Sources
* [Overtourim: Impact and Possible Policy Responses](https://www.europarl.europa.eu/RegData/etudes/STUD/2018/629184/IPOL_STU(2018)629184_EN.pdf) (lots of data by city)
* [Is Overtourism Overused?](https://www.researchgate.net/publication/329159594_Is_Overtourism_Overused_Understanding_the_Impact_of_Tourism_in_a_City_Context)
* [‘Overtourism’? Understanding and Managing Urban Tourism Growth beyond Perceptions](https://www.e-unwto.org/doi/pdf/10.18111/9789284420070)
* [Worst Ranked Overtouristed Cities in Europe](https://www.statista.com/statistics/778687/overtourism-worst-european-cities/)
* [UN World Tourism Organization Statistics](https://www.unwto.org/data) (requires student proposal for free data)
* [UNWTO Dashboard](https://www.unwto.org/unwto-tourism-dashboard) - quick view of above data without 
* Overtourism: A Literature Review to Assess Implications and Future Perspectives (in data directory)

## 4. Homelessness in America/Anti-Homeless Legislation
I don't have as much base knowledge for this topic, but I hear about it in the news increasingly often. 
While homelessness is not explicitly outlawed, many pieces of (controversial) legislation have been enacted in the 
United States to curb the visibility of homelessness in cities. I think that the biggest hurdle would be finding 
complete, reliable, and updated data. I would love input on a more specific topic and/or interesting datasets to combine!

* [2014 Report on Anti-Homeless Legislation](https://nlchp.org/wp-content/uploads/2019/02/No_Safe_Place.pdf)
* [Map Based on No Safe Place Report](https://www.pbs.org/newshour/nation/interactive-map-number-of-u-s-cities-criminalizing-homelessness-doubles)
* [New York Coalition for the Homeless](https://www.coalitionforthehomeless.org/)
* [California Policies by City](http://wraphome.org/wp-content/uploads/2016/06/NVL-Update-2016_Final.pdf)
* [Anti-Homeless Ordinances in American Cities](https://www.researchgate.net/publication/325718729_Anti-Homeless_Ordinances_in_American_Cities) (check sources)
* [Housing Not Handcuffs 2019 Report](http://nlchp.org/wp-content/uploads/2019/12/HOUSING-NOT-HANDCUFFS-2019-FINAL.pdf) (includes updated cities data)

