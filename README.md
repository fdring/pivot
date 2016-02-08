Pivot creation API
======

## Downlowd junit (https://github.com/junit-team/junit/wiki/Download-and-Install) 
## & sqlite-jdbc (https://bitbucket.org/xerial/sqlite-jdbc/downloads) jars and 
## place in the lib folder

## Run using [ant](http://ant.apache.org/)

====================================
General
====================================
Five parameters are always expected:
--> Action
--> -Dtable
--> -Dcolumn
--> -Drow
--> -Dmeasure
--> -DmeasureField

====================================
Print results
====================================
Example:
>>ant print -Dtable=ProductType -Dcolumn=Year -Drow=Client -Dmeasure=Sales -DmeasureField=count
--> Result is printed

====================================
Print results as html
====================================
Example:
>>ant printHtml -Dtable=ProductType -Dcolumn=Year -Drow=Client -dmeasure=Sales -DmeasureField=count
--> Result is printed as html

====================================
Save results as html
====================================
Example:
>>ant saveHtml -Dtable=ProductType -Dcolumn=Year -Drow=Client -dmeasure=Sales -DmeasureField=count
--> Result is save in a html file & can be found in HtmlOutput/{table]_{column}_{row}__{measure}.html