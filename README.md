# STARS-Scope-Profiles
Config Files and Associated Radar Video Maps to be used in DGSCOPE by K2FC

There will be a sector configuration file for every TRACON in the United States organized by each facility's ID code. To find an ID code go to https://123atc.com/facilities. Some Airports do not have dedicated TRACONs but still have radar data and will be located under TRACABs.

Each folder of a TRACON will include the following files:
- (FACILITY ID).xml = The configuration file preset with the radar information and homepoint to be used on DGSCOPE.
- (FACILITY ID VIDMAP).geojson = The prebuilt set of frequently used video map files for each facility using CRC     
      files current as of 5/10/2025.
- VMAP List-Info = The information regarding the order and names of each video map included in the set as well as position logon identifiers.
- VMAPS = An additional folder including each individual video map .geojson file taken straight from CRC with namings. 

Installation and Usage Instructions:
1. Download the full package or the specific folder of the TRACON you are insterested in and extract contents.
2. Startup DGSCOPE or install here https://github.com/k2fc/scope
3. When the popup opens to select a sector file, choose the (FACILITY ID).xml (It will initially popup and say "empty path name is not legal" because you have not assigned a videomap file yet)
4. Once running, "CTRL+P" to open preferences and then scroll down to "Misc" to find "Video Maps - (Collection)"
5. Click on the three dots on the rights side of the preference menu which will open up a new menu
6. Navigate to "File", "Import", "From GeoJSON" and then upload the (FACILITY ID VIDMAP).geojson
7. After a few seconds, the table should populate with maps. Save and close the screen.
8. The DCB should now show maps in the first few slots. Click to toggle visibilty.
9. "Ctrl + S" once you have loaded videomaps so that is saves your preferences for the future.  

If you have any problems regarding the videomaps, feel free to comment with an issue.  
