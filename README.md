# Corpus Chrisi Race Marks
GPS coordinates for sailing race markers for the Corpus Christi, Texas sailboat racing area.

## Please help
Please consider creating a similar GitHub repository for your local sailing area if one does not already exist. Visiting sailors well have the pleasure of knowing where they are going in their first race, and the locals will look like they know what they are doing too.

## Source
These mark coordinates were found on the Corpus Christi Midget Ocean Racing Fleet (CCMORF) [website](http://ccmorf.org/) in this [handy PDF](https://ccmorf.files.wordpress.com/2011/12/2-1-10-ccyc-bay-race-map-and-chart.pdf)(downloaded 2015-07-17) that lists distance and bearing for all combinations of the different race marks.

The idea for this repository came from Norbert Kiesel's [GitHub repository](https://github.com/nkiesel/YRA-Marks) for San Francisco Bay race marks, which he's been keeping up to date for several years.

## Garmin GPX File
In order to create the Garmin compatible GPS file (aka a GPX file), the following [GPSBabel](https://www.gpsbabel.org/) command was used in Linux:

```gpsbabel -i unicsv -f corpus-christi-bay.csv -o gpx -F corpus-christi-bay.gpx```

If you are using Linux, you can easily upload the GPX file to your Garmin GPS using the following command:

```sudo gpsbabel -D9 -i gpx -f $1 -o garmin -F usb:```

## Updates
If you want a new mark added or an old one updated, please either [issue a pull request](http://yangsu.github.io/pull-request-tutorial/) from your forked GitHub repository (preferred) or create a support ticket at [Sail Tactics](http://www.sailtactics.com/support).
