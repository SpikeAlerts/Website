---
layout: page
title: About
---

# Hello!

We are a collective working to make a text alert and reporting system for Air Quality events in Minneapolis. 

All code will be free and open-sourced (MIT License). 

---
---
---

## Background 

When Canadian wildfires blanketed US cities in the summer of 2023, air quality rose to the forefront of public concern across the country. In Minneapolis, the fight for the East Phillips Urban Farm also raised air quality as an environmental justice issue in the public consciousness. Asthma and other health issues are clearly higher in Minneapolis neighborhoods which were [redlined](https://legacy.yourwebedition.com/stories/a-city-divided-0) and have more polluting facilities, particularly in North Minneapolis, a majority black neighborhood, and the Phillips and Cedar-Riverside neighborhoods in south Minneapolis, which have high Indigenous and immigrant populations. 

Federal regulations that monitor air quality at a regional level leave large gaps in data in terms of knowing what people in a particular block or neighborhood are exposed to. [Community-Based Air Quality Monitoring](https://www.georgetownclimate.org/articles/community-based-air-quality-monitoring-equitable-climate-policy.htm) (CBAQM) projects address those gaps by monitoring air quality at a neighborhood level.

Community organizers concerned about air quality have also come up with a variety of ways of tracking data and using it to hold governments and industry accountable for the poison put into our air. In Pittsburgh, for example, [Smell PHG](https://smellpgh.org) crowdsources information about smells to track pollutants that pose health risks to residents. **This is a crucial intervention because it treats people’s lived experiences as valid data.** 

[The City of Minneapolis](https://www.minneapolismn.gov/government/programs-initiatives/environmental-programs/air-quality/) has engaged in CBAM by putting up and maintaining [PurpleAir](https://map.purpleair.com/1/mAQI/a10/p604800/cC0#11/44.9368/-93.2834) monitors, a system which provides real-time readings of PM 2.5 readings. This is a very important investment. However, there is a gap between simply making data available to the public and making an active effort to deliver it to people who need it. The Air Quality Alerts system sets out to close the gap, by providing an easy way to get updates about bad air quality only when there is a significant spike. 

Air quality monitoring initiatives usually emphasize long-term exposure. However, acute exposure at certain levels also presents significant health risks. Future iterations of this project could offer daily, weekly or monthly air quality reports, but this version chooses to focus on 'spikes', which represent possible acute (short-term) exposure events.

We believe clean air is a human right. We believe communities deserve to know exactly what we are breathing in, when, and what effects it might have on our health. This alert system is intended to be a tool to facilitate awareness and capacity to fight against those that would treat marginalized  communities as sacrifice zones. 

## Functionality  

Users who want to receive alert messages can fill out our survey and have their phone number and location of interest stored in a secure [REDCap](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5764586/) database hosted by the University of Minnesota.

The program queries the PurpleAir API every 10 minutes (soon we'll have more sensors) and checks for readings above a threshold (35.5 micrograms/meter^3 for sensitive groups, 55.5 for all) according to the current [24-hr EPA Standards for PM2.5](https://www.epa.gov/pm-pollution/national-ambient-air-quality-standards-naaqs-pm). The thresholds are variables that can easily be changed/adjusted. When the system detects a spike, it sends a text to all subscribers within 1 kilometer of the monitor if they don't already have an active alert. The text links to the sensor on the PurpleAir Webmap.

When all alerts end for a user, an end of spike alert message is sent to the subscriber, detailing the length and severity of the event, and a unique reporting option through REDCap. Alerts are archived for future reference (this does not include the user's location/phone number).

## Readme Authors

Priya Dalal-Whelan

Rob Hendrickson

## Foundational Developers

Rob Hendrickson

Priya Dalal-Whelan

Dan Raskin

Mateo Frumholtz

Doug Carmody

## Sensor Maintenance & Counsel

Jenni Lansing

Lucy Shapiro

## Other Contributors 

Connor Stratton, Urszula Parfieniuk, Michael Wilson, Nazir Khan, Alice Froehlich, Megan Greenberg, Mary Marek-Spartz, Kerry Wang, Daniel Furata, Eamonn Fetherston, Jake Ford

Thank you for organizing, discussion, feedback, research, and everything in between!

We also acknowledge the preliminary work of the [Quality Air, Quality Cities team](https://github.com/RTGS-Lab/QualityAirQualityCities).
