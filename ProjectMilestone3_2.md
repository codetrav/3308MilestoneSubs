# ProjectMilestone3_2: Code Hawks #

*Team Members: Travis Cochran, Fallyn Logan, Avra Saslow, Brett Schneider, Andrew Weller, Will Walker*

[Milestone 3 Demo: Node.js](198.23.146.166:3000/demo)

**What features were completed:**
* The backend script that pulls and parses information from the OBD-II
* The frontend login page and home page
* The postgres database `car` and the Node.js database that displays the information
* The individual tables for each user and their specific car are filled with data from the OBD-II

**What worked during the demo:**

The individual backend and frontend demos both worked as expected during the demo. 

**What issues were faced either during the development or during the demo:**

We faced some minor issues when parsing the car data; we had some varchars that weren't large enough to store all of the data we were pulling in. However, we went into our database and made the the value for each varchar larger. Another issue we ran into is we want to query for the VIN, but that command isn't available in the OBD python library. We might have to add it to the dictionary ourselves if we want to use that command to check for recalls. 

**What were the suggestions offered by the TA:**

*Recommendation 1:* Get data, even a small amount, up on the website so that the frontend team can begin palying with visualizations and widgets.

We decided to display the four common peices of data displayed on a car dashboard:
* fuel level 
* speed 
* RPM
* coolant temp

The frontend team will use these four pieces of data to begin building out the live/asynch page and the home page which displays the most important information. 

*Recommendation 2:* 
Instead of keeping the data in rows, store the data in columns so that it is quicker to query. 
