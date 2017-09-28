# Conference badge generator
This is a HTML/JS/d3 app which helps to generate printable pages with conference badges. You just need to prepare the conference badge template (as badgeTemplate.svg) and the list of participants (as participants.csv). Requirements for the files are described below.

Unless 54x180mm badges suit you, you will have to adjust CSS code in index.html. Adjustments are pretty minimal, so everything should be fine even if you are not a programmer.

## Requirements for the badge template

* SVG format
* saved as badgeTemplate.svg in the same folder as index.html
* must have text elements with the following classes:
    * name - these text elements will be used for participant's name
    * surname - these text elements will be used for surnames
    * afil1 - first line of affiliation
    * afil2 - second line of affiliation
* it is best to set template's size in mm and set the same size in index.html

## Requirements for the list of participants

* CSV format with "," as separators (other format requirements are outlined in d3 v4 documentation)
* first line must contain column labels
* column labels must include:
    * name - to mark column which stores participants' names
    * surname - to mark column which stores participants' surnames
    * afil - to mark column which stores participants' affiliations (you can split affilations into two lines by using "|" symbol)
