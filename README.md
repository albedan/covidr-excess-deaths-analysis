# CovidR - Understanding COVID-19 thorugh Italian excess deaths analysis
Why are we expecting to **understand** COVID-19, when most of the analysis rely on the same biased, unreliable and dull data

Death and cases are counted *differently* across countries. In Italy, regions and provinces have *different capabilities and policies* when it comes to testing the population. All this makes drawing conclusions a hard and risky task. 

Here I suggest an *original* approach based on **overall deaths** data from ISTAT, available from 2015 to 2020, done 100% in R.

I focus on **excess deaths with respect to previous years** and answer many questions with a robust quantitative approach. Are men really more hit by COVID-19 than women? Is it true that only the elderly are affected? What really happened in Bergamo and other Italian provinces?

## Data and notes
The "data" folder has to include 3 files:
- comuni_anpr.csv: the list of the municipalities with updated data (till the 15th April 2020), already provided in this repo
- comune_giorno.csv: the historical data from 2015 to 2020, as available through ISTAT website (https://www.istat.it/it/files//2020/03/Dataset-decessi-comunali-giornalieri-e-tracciato-record.zip)
- comuni.csv: the number of inhabitants of Italian municipalities, as provided by ISTAT (http://demo.istat.it/pop2019/dati/comuni.zip)

And 1 folder:
- /Limiti01012020_g/Com01012020_g: the location for the shapefiles of Italian municipalities, ad downloaded from ISTAT (http://www.istat.it/storage/cartografia/confini_amministrativi/generalizzati/Limiti01012020_g.zip). They are 4 files: Com01012020_g_WGS84 (.dbf / .prj / .shp / .shx)