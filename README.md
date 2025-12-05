# BS5228-in-QGIS
Build the script to calculate noise levels from construction activities following the BS 5228 standard

# step 1: determine the equipment and noise levels
determine the equipment, number of units, on time, duration / programme, SPL at 10m or SWL
Save this in a table and save it as CSV

# step 2: import the CSV to QGIS
Layer -> Add Layer -> Add Delimited Text Layer ...

# step 3: use script from Plug-in to calculate the total SPL or SWL for each activity
load the added text layer (CSV) then calculate the total SPL at 10m or total SWL

# step 4: draw the working area for each activity, NSR points in QGIS
create a working activity layer and features which are the working areas in polygon format
add the NSR as points, build the houses in

# step 5: distribute the SWL to the working area
split the working areas to square shaped grid
distribute the SWP or SPL to the centre of each grid

# step 6: calculate noise level at NSR or grid
calculate the nosie level for each grid (of the source) at the NSRs then sum them up
split the receiving areas to square shaped grid
calculate the noise level at the center of each grid

# step 7: generate grid in QGIS
