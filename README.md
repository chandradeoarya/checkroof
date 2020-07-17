<h1 align="center">
	<img
		width="300"
		alt="Project Checkroof"
		src="https://github.com/chandradeoarya/checkroof/raw/master/img/checkroof.png">
</h1>

<h3 align="center">
	Project Checkroof
</h3>

<p align="center">
	<strong>
		<a href="https://checkroof.org/">Website</a>
		•
		<a href="https://github.com/chandradeoarya/checkroof/blob/master/README.md">Docs</a>
		•
		<a href="mailto:checkroof.org@gmail.com">Support us</a>
	</strong>
</p>

<p align="center">
	<img src="https://github.com/chandradeoarya/checkroof/raw/master/img/checkroof.gif" width="700">
</p>

## Overview

**Project Checkroof**  is an rainwater and energy conservation initiative started by  Chandradeo Arya and his friends. Project Checkroof is combination of three projects rainroof, sunroof and coolroof. The initiative's stated tagline is "Discover what your roof can do for you".

Project Checkroof, inspired by Project [Sunroof](https://www.google.com/get/sunroof), primarily works to encourage the private adoption of rain water harvesting and energy conservation techniques like solar adoption, coolroof coating by providing a set of tools to facilitate the purchase and installation of these systems. Using data from  [Google Maps](https://en.wikipedia.org/wiki/Google_Maps "Google Maps")  to calculate shadows from nearby structures and buildings and taking into account historical data of monsoon, rainfall, weather and temperature patterns, the Project Checkroof website calculates total rainwater harvesting and energy potential of your house. In addition, the Project Checkroof website also provides a list of local certified retailers capable of installing these systems in that area.

While initially launching only in the cities of  [Hyderabad]([https://en.wikipedia.org/wiki/Hyderabad](https://en.wikipedia.org/wiki/Hyderabad) "Hyderabad"),  [Bangalore]([https://en.wikipedia.org/wiki/Bangalore](https://en.wikipedia.org/wiki/Bangalore) "Bangalore"), and  [Chennai](https://en.wikipedia.org/wiki/Chennai "Chennai"), the project is planned eventually to expand nationally or even globally, depending upon the project's success in its launch areas.

<h3 align="center">
	Working principal
</h3>
<h5 align="center">
	Search --> Research --> Shop
</h5>
<p align="center">
	<img src="https://github.com/chandradeoarya/checkroof/raw/master/img/how-it-works.png" width="700">
</p>


# Core Projects

Project [Checkroof]([https://checkroof.org/](https://checkroof.org/)) is combination of three projects Rainroof, Sunroof and Coolroof. Together these three core projects make final project [Checkroof.org]([https://checkroof.org/](https://checkroof.org/))

## [Rainroof](https://github.com/chandradeoarya/rainroof/blob/master/README.md)

<p align="center">
	<img src="https://github.com/chandradeoarya/checkroof/raw/master/img/search-page.png" width="700">
</p>

All major cities in India and developing countries are facing acute shortage of water with Chennai being the worst this year. Annually India gets over 468 billion liters of rainwater which if potentially harvested can meet 40% of total demands. But due to lack of government initiatives and harvesting mechanism in place, no rainwater is conserved for recharging ground water. 

In spite of huge interest from public, there is no one single platform where one can measure their RWH potential and also connect with local vendors to install it.  Project rainroof is a step in that direction only.

## [Sunroof](https://github.com/chandradeoarya/sunroof/blob/master/README.md)


<p align="center">
	<img src="https://github.com/chandradeoarya/checkroof/raw/master/img/sunroof-portal.png" width="700">
</p>

We are building one stop platform to help you discover solar potential of your house. It asks you for your monthly electricity bill and gives you the recommended solar installation size to meet your energy needs. It also tells your the up-front cost of installations or suggest leasing or renting options. It lists the best state and central governmental incentives for you to choose. 

We have also partnered with certified solar installation vendors and list their pricing and services details like warranties and maintenance for help you choose the most suitable one for you.

## [Coolroof](https://github.com/chandradeoarya/coolroof/blob/master/README.md)

<p align="center">
	<img src="https://github.com/chandradeoarya/checkroof/raw/master/img/uhi.jpeg" width="550">
</p>
Air Conditioning inside buildings consume 10% of total global energy over 100,000 TWh (terawatt-hour). On a typical summer day, traditional “dark roofs” absorb significant sunlight – around 100 watts per square foot which increase temperature inside building by 3-7°C which in turn leads to higher use of ACs. If we could just paint or coat the roof with high reflective materials like Titanium Dioxide then it can reflect about 70-80% of infrared rays of sunlight which account for 49% of heat generated.
<p align="center">
	<img src="https://github.com/chandradeoarya/checkroof/raw/master/img/infrared.png" width="550">
</p>
<p align="center">
	<img src="https://github.com/chandradeoarya/checkroof/raw/master/img/uhi-house.png" width="550">
</p>
Project Checkroof helps you discover the coolroof potential of your house with just few clicks. It also provides you list of vendors who can do white painting or coolroof coating on your roof.


# Sub Projects
Smooth functioning of the portal [checkroof.org]([https://checkroof.org/](https://checkroof.org/)) depends on the following list of sub-projects. These projects, being unique on its own and having no known ready to use alternatives, are being developed as multipurpose micro-services available to public for extended use cases. 

## [PinMap](https://github.com/chandradeoarya/pinmap/blob/master/README.md)

<p align="center">
	<img src="https://github.com/chandradeoarya/checkroof/raw/master/img/pinmap.png" width="700">
</p>
For any search of area based on name, pin code or region Google map clearly shows the outline and clear border for that area. To effectively perform any GIS analytics on any area like calculating the solar and rainwater harvesting potential of a region border coordinates are required. But presently there is no openly available api, library which can be used for it.

**List of present solutions and their limitations**

 1. **Google Maps** - At this moment there is no option from Google in the Maps API v3. Developers have been making [feature requests since 2012](https://issuetracker.google.com/issues/35816953) and over 400 users have starred this issue as well but there is no update from Google on it.
 2. **Twitter API** - It seems twitter had this feature and [api](https://developer.twitter.com/docs/api/1/get/geo/id/:123) as well but it requires authentication now and [only gives five coordinates](https://i.stack.imgur.com/X3OMj.png)  which is not enough to draw the boundary. 
 3. **[Open street map](https://en.wikipedia.org/wiki/OpenStreetMap)** - This is an open source, editable and collaborative map which presents boundaries. Searching [a place in maps](https://nominatim.openstreetmap.org/details.php?osmtype=N&osmid=245640543&class=tourism) and collecting OSM ID and coordinates in json can be later used in Google maps built in [KML system](https://wiki.openstreetmap.org/wiki/KML) a standard now moderated by [Open Geospatial Consortium](https://wiki.openstreetmap.org/wiki/Open_Geospatial_Consortium "Open Geospatial Consortium") or it can be directly used as well. But it works only for some selected areas in United States and for most searched cities it doesn't have boundary data as well.
 4. **Properitory APIs** - some organisation like [http://housing.com/](http://housing.com/) have built it for their internal usage. As seen in housing data for [whitefield, Bangalore](https://regions.housing.com/api/v1/polygon/show/2dd0d8ff553613d1aa3f). But it's not right to scrap them or depend on them as internal apis keep changing this is also not a good solution.

**Our methodology** - Over the time being Project Checkroof team has built a massive database of all pincodes of India, their coordinates using [India Post](https://en.wikipedia.org/wiki/India_Post) as the baseline of areas. We will refer these admin areas conjugated with [GADM](https://gadm.org/about.html) data which can help us achieve admin level 3 accuracy and draw the map using [Google Maps polygon overlays](https://developers.google.com/maps/documentation/javascript/overlays#Polygons). Later as portal is used user's location information of all inquiries will be stored and later used to build the map of all administrative regions.

Continuous efforts are ongoing to establish a communication with Google Maps team to give us access of proprietary data. Depending on our success we may reach out to proprietary api owners as well for giving us access of their database.

## SoilMap

Every installation of rainwater harvesting system by us gives us excavated soil in the depth upto 15 ft. Geochemistrial study of soil gives lot of information about major nutrients, major elements, essential trace elements, trace elements of special interest and minor elements of soil. This study builds point and spatial distribution maps of soil which is later used in more research works like earthquake engineering, construction and building science.

We plan to collect all these soil and make a soil bank and national soil archive of India. All developed countries like USA, Ireland, Canada etc. have their soil databases like Ireland has national soil database, United States has Digital General Soil Map of the United States (STATSGO2), Soil Survey Geographic Database (SSURGO), National Soil Information System (NASIS) etc. programs. 

In India we have programs like soil and land survey authority of India which works under department of agriculture and all of their studies have been towards land usage, degradation. Last soil survey was done in 1958 mostly around watersheds of rivers. 

We have planned to build Soil Map for India and rest of the world.

<img
		width="500"
		alt="Project Checkroof"
		src="https://www.gestiriego.com/wp-content/uploads/2018/05/5-Parametros.jpg">
</img>


![enter image description here](https://www.nrcs.usda.gov/Internet/FSE_MEDIA/nrcs142p2_050140.jpg)       ![enter image description here](https://3.imimg.com/data3/CA/OS/MY-10154958/soil-analysis-250x250.png)

## Thanks
The project is under active development. Please reach out to us if you have any more questions or if you want to partner us or join the team. We can be reached on checkroof.org@gmail.com