# geoid_heights
I read this page on how to convert from lat/lon to a geoid height, used to correct GPS altitudes to be from mean sea level.
http://stackoverflow.com/questions/22196714/wgs84-geoid-height-altitude-offset-for-external-gps-data-on-ios

It has a great conversion of a c-lib to cocoa for calculating those corrections, however it requres 10MB worth of text files and a loading process that will consume app memory.  To avoid those expenses, I used that code to create a sqlite file for the correction value of all lat/lons (as integers).  This project contains that database and the CSV I used to make it.
