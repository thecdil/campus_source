# campus_source

University of Idaho Campus Photographs Collection

<https://www.lib.uidaho.edu/digital/campus/>

------

The campus collection has two metadata spreadsheets, one describing the photographs (the PG1 collection) and one describing campus buildings. 

## Buildings Data

Buildings information is broken into two parts:

1. spreadsheet "_data/campus-buildings.csv" - contains the structured metadata about the buildings. Each row is the record of one building. It populates the "Buildings" page and each row generates an individual Building item page. Note: the "featured_image" column will match one "objectid" from the "campus.csv" spreadsheet that describes all the individual photos--that id will be used to pull in image information for the primary image for the building listings.
2. markdown collection "_histories/" - the "_histories/" folder contains markdown files, one for each building, matching the "objectid" of the building. The file can contain longer form narrative content about the history of the building. It can use Markdown and Liquid includes (like a collectionbuilder About page). The long form content is pulled into the individual Building pages (using the "objectid" in the markdown file's front matter). Most of these are currently empty--if the building does not need an extended narrative, it can be left blank!

## Photograph Data

Metadata about each individual image is found in "_data/campus.csv".
Each row describes one image. 

The "buildingid" column can match one "objectid" in the "campus-buildings.csv" data to link the image record with a specific Building (this is blank for some images).
