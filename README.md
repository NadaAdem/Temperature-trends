# Temperature Trends for Surf shop in Oahu

## Overview of the analysis

The purpose of this project is to analysis temperature trends before opening the surf shop  in Oahu. The temperature data for the months of June and December, in order to determine if the surf and ice cream shop business is sustainable year-round.For cilent make a more informed decision.


## Resources and Software
Data : hawaii.sqlite
Software :Python 3.7.10
SQLAlchemy 1.4.1

## Results



Statistical summary for  Temperature the month of June in Oahu  

![This is an image](https://github.com/NadaAdem/Surfs_up/blob/main/Resources/June_temp.png)



Statistical summary for  Temperature the month of December in Oahu  

![This is an image](https://github.com/NadaAdem/Surfs_up/blob/main/Resources/Dec_temp.png)


## Summary
Based on the  Statistical summary for  Temperature the month of June and  December , it can be expected that a surf shop in Oahu will have less customers in December than in June due to the slight decrease in average daily temperature. 

for get  Two additional queries on June and December to obatin more weather data about precipitation during those months.

The query below will find precipitation scores in June:

session.query(Measurement.date, Measurement.prcp).filter(extract('month', Measurement.date) == 6).all()


![This is an image](https://github.com/NadaAdem/Surfs_up/blob/main/Resources/Dec_temp.png)


The query below will find precipitation scores in December:

session.query(Measurement.date, Measurement.prcp).filter(extract('month', Measurement.date) == 12).all()

![This is an image](https://github.com/NadaAdem/Surfs_up/blob/main/Resources/Dec_temp.png)
