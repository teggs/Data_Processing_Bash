# Data_Processing_Bash
1. main.  Just Invoke this function to get the final route.html. You don't need to run any file else.

2. calender.txt, fremantle, fstn, rstn, stn, trips, stops.  This 7 files are intermediate files. Since I can
only take train or subway to get  to the destination, so a lagre part of the original files are useless 
actually. To improve the time efficiency, I preprocessed them to these concise versions.

3. haversine.wak. This file calculates the distance between two locations.

4. stngrep. This file find all the stations that near from you(i.e. less than 1km), and calculate the 
times to walk there.

5. linegrep.(core file!) Find all the triplines that passing two given station. 

6. findline.(core file!) Find the earliest line and earlier than 15:25:00 from many given lines.

7. nonstop. If you can go to fremantle directly, this file calculates the route using the two core files.

8. transfer. If you can go to the Perth Station or Perth Subway Station, this file calculates the route and
then calculates one route from 99007 to 99352 using the two core files.

9. extract. The transfer file will provide all the possible routes. This file will find one earlist routes.

10. ghtml. Generate a html file containing the optimal route infomation.
The answer will be presented as a HTML file
