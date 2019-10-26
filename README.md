# Consultation-eventdata
Use some open data, scrap some sites and parser for event dates and locations 

* Write out the steps and methodology so that you can blog about the process. (Medium)

## Brain dump

What this sets out to do:

Civic tech project - for my porfolio

## Objective
Get event level data so that it can be shared in a flat file, mapped and put on a calendar.

## Issues
* Location mapping - need to learn about standardized formatting
Need to find and parse dates that maybe in various structures, need to standardize to Government of Canada date standard (citation).

## Sources of information
* open.canada.ca
* canada.ca style guide design pattern for consultations pages: https://design.canada.ca/recommended-templates/consultations-page.html
* https://scraperwiki.com/ --> https://quickcode.io/
* Date standard: https://www.iso.org/iso-8601-date-and-time-format.html (https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=18909&section=xml)
* 

## How the program needs to work:
1. Needs to get the dataset from open.canada.ca every 24 hours
* Specifically the one that's every two years (https://open.canada.ca/static/current_consultations_open.csv)
2. Needs to put into a new flat file and pull out the the English title (title_en), French Title (title_fr), and links to the consultation profile pages (profile_page_en,profile_page_fr).
3. Needs to then navigate to each profile pages (EN/FR) and look for a section called "Attend a meeting". 
* There might be multiple phrases that should be specified here... look at a sample of pages to provide a few options. This is where standardization could be useful.
4. Take the content below the "Attend a meeting" section and add it to the flat file. 
* There should be content for an event location, date and time, and venue.
5. Take this new file and save it somewhere?
6. Take the location, date and time, and venue and see if it needs to be standardized?
7. Take the locations and add them to a map.
* Google map - Should this be the WET mapping tool?
8. Take the data and add it by date to a calendar.
* Google calendar or the WET calendar on a new page? Should this be a github page prototype that looks like canada.ca?
