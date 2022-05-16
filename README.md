# UFO Sightings Analysis
## Overview of Project
### Purpose

Using Dana's static Javascript file filled with UFO sighting information, we were able to help Dana create an interactive online dashboard with her findings. Due to the sheer volume of data available, we were able to update the webpage to allow users to filter for multiple criteria (i.e., date, city, state, country, and shape) at the same time. This report will describe how to use the updated webpage as well as describe a drawback and two recommendations for further development.

## Results
### Overview of UFO Sightings Website

![image](https://user-images.githubusercontent.com/99936542/168508510-b4a905bb-3ef4-4d9f-80e9-c176391e3d6b.png)

<b>Fig.1 - UFO Finder Website</b>

Dana's UFO sightings website, pictured above in Figure 1, uses the following components --

- Jumbotron for the page header, "The Truth Is Out There"
- text blocks for the article's title - "UFO Sightings: Fact of Fancy? Ufologists Weigh In" - and text 
- grid system for the UFO sightings table and filters 

### UFO Sightings Table and Filters

Dana's collection of UFO data is somewhat extensive, such as the date, location, and the type of each sighting, so the full table in its entirety is too much for an user to reasonably look through and study. The ability to filter the data was therefore created to help fine tune the results. Originally, the website was only able to filter by date of sighting. However, the HTML and Javascript code was refactored to allow users to filter for multiple criteria at the same time.

Users may input the following search criteria on the left side of table as shown in Figure 2:
- Date of sighting
- City of sighting
- State of sighting
- Country of sighting
- Shape of sighting

Initially, sample placeholder text is provided in the text box as an user input suggestion/example.

![image](https://user-images.githubusercontent.com/99936542/168511763-e6ff710b-77bf-47ea-9a86-bf79ccb20e09.png)

<b>Fig.2 - Filter Search</b>

By using the D3 JavaScript library interactive functionality by "listening" for events -- in this case, a text change in the any of the search criteria input boxes -- the website is able to detect the text change and able to display a filtered table of searched results. For example, a search for UFO sightings in the state of Kansas (ks) provide the following table of search results (Figure 3).

![image](https://user-images.githubusercontent.com/99936542/168513279-8440f3af-2560-43ee-9400-236f235ffc42.png)

<b>Fig.3 - Filter Search for State of Kansas</b>

## Summary
### New Design Drawback

Although a placeholder text is displayed for each of the search criteria, a lack of valid search suggestions may be inefficient since users may have to enter various dates, locations, and shapes of sightings in order to produce a filtered findings table. 

### Recommendations for Further Development

Below are two additional recommendations for further development:

1. Update the filter search input boxes as drop-down menu of valid search texts instead of open-ended text boxes to improve efficiency of producing a successful filtered table. Using a drop-down menu of valid search text for each search criterion will also eliminate the need of the ambiguous placehoder text -- it's easy to mistake the placeholder text with entered search criteria because of its identical text color and font.

2. The ability to sort the UFO sighting findings by the various data columns.