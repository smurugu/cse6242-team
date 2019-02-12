# Bike Lane Buildout

from: https://data.seattle.gov/Transportation/Existing-Bike-Facilities/raea-rshc

We can get a timestamp of when bike improvements were created.

The key columns here are:
DATE_COMPLETED - use this to detemrine when the bike line is active.
PLANNED_FACILITY_TYPE - (TODO: enumerate these) type of improvement (i.e. protected lane, marked lane, shared lane)
COMPKEY - identifier which allows us to determine *where* the improvement is located.

from: https://data-seattlecitygis.opendata.arcgis.com/datasets/street-network-database-snd

We can get all street network buildouts.  The column we are interested in is:
COMPKEY - Identifier to join against for bike facilities
L_ADRS_FROM - street address numbers on left side of street.  This can be used to determine starting point of road segment.
L_ADRS_TO - street address numbers on right side of street.  This can be used to determine ending point of road segment.
L_CITY
L_STATE
L_ZIP
ORD_STREET_NAME - i.e. 45th
ORD_PRE_DIR - i.e. NE.
ORD_STREET_TYPE - ie. St.
ORD_STNAME_CONCAT - i.e. NE 45th St
R_ADRS_FROM
R_ADRS_FROM
