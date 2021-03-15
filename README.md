# UFO Sightings Interactive Web Site

## Overview of Project
This project is for the use of a data journalist, Dana, to present dynamic UFO data with her article about the topic of UFO sightings.  JavaScript is used to store the JS data
file, as well as to interact with the HTML and CSS files for a dynamic and attractive presentation of her topic.

## Results
Dana's article is accompanied by a dynamic data table with five filters; date, city, state, country and shape (of UFO).  There is an input box for each filter.  The user can enter
one or multiple queries into the input boxes.  

### Sample Search
For example, searching for WI yields three results as can be seen in the image here.
[Image of searching for WI ] https://github.com/CaroShaf/UFOs/blob/main/images/statesearchwdateerror.png

Another example shows a search for disk shaped UFOs, as seen here.
[Image of searching for Disk Shaped UFOs] https://github.com/CaroShaf/UFOs/blob/main/images/shapewstatedateerror.png

Multiple fields can be searched simultaneously, such as state and date.  In this case, the three WI sightings are further reduced to only one when searching by 1/1/2010, as can be seen here.
[Image of searching for both WI and Date] https://github.com/CaroShaf/UFOs/blob/main/images/dateandstatesearch.png


## Summary
### Drawbacks
* Persistent data - It should be noted that in all three of the above searches, previous search terms linger in the input boxes even though they do not affect the results.  For
example, the search for disk shaped objects shows that a previous search for UFO sightings on 12/15/2010 was performed, as it remains in the Date field.  Data input persists even after reloading the table data, not clearing the input boxes.  A likely solution that includes a Clear box in the css stylesheet can be found in this YouTube video: 
https://www.youtube.com/watch?v=v_m16oewrH0
* Inflexible user input - If a user enters 01/01/2010 instead of 1/1/2010 the results are zero, as can be seen here:
[Double digit failure] https://github.com/CaroShaf/UFOs/blob/main/images/doubledigitfail.png
A leading zero is standard, but doesn't work in this case.  However, it would be improved if either worked.  Furthermore, it would also be useful to be able to just search by
year, without including Month and Day.  In this particular data set, however, only two weeks of 2010 is included, which leads to the next drawback.
* Limited data set - Since there is only two weeks of data from January 2010, this project is limited in scope and represents a lot of work for a small dataset.   A plan for expanding the dataset or updating it on a scheduled basis is recommended.

