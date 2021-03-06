# DATA 512 Project: COVID Analysis 
During the Course Project I took a look at some of the social aspects of the pandemic by conducting a human centered data science analysis of some available COVID-19 data. The course project is consist of four assignments (A4 through A7):
* Assignment A4: Common Analysis sets the stage for the subsequent assignments. In A4 I conducted a base analysis. 
* Assignment A5: Extension Plan - I asked a human centered data science question that extends the work in A4: Common Analysis. 
* Assignment A6: Presentation - I gave a modified (shorter) PetchaKucha presentation of your completed project.
* Assignment A7: Final Report is a written submission of a project report.

## County Assigned 
| County   | State    | FIPS Code |  Area_km^2 | Area_mi^2 | Population_2020_Census | Population_Increase_from_2010 | County Seat   |
| ---------| -------- | ----------| ---------- | --------- | ---------------------- | ----------------------------- | ------------- |
| New York | New York |   36061   |   59.13	   |   22.83   |       1,694,251        |           108,378             | Manhattan, NYC|

## Data
In this project, four datasets are being used:
1. The [RAW_us_confirmed_cases.csv file](https://www.kaggle.com/antgoldbloom/covid19-data-from-john-hopkins-university?select=RAW_us_confirmed_cases.csv) from the Kaggle repository of John Hopkins University COVID-19 data. 
2. The [CDC dataset](https://data.cdc.gov/Policy-Surveillance/U-S-State-and-Territorial-Public-Mask-Mandates-Fro/62d6-pm5i) of masking mandates by county. 
3. The New York Times [mask compliance survey data](https://github.com/nytimes/covid-19-data/tree/master/mask-use).  
4. The kaggle dataset [“Normal and New Normal: NYC Subway Traffic 2017-21 (NYC subway traffic before, during and after the covid lockdown)”](https://www.kaggle.com/eddeng/nyc-subway-traffic-data-20172021) 


## Directories and Files Explanation
* `/raw` directory is the directory that contains all the raw data used in this project, subspecically inside this directory:
    - `RAW_us_confirmed_cases.csv` is the CSV file downloaded from the Kaggle repository of John Hopkins University COVID-19 data that contains the data confirmed cases of the entired United States daily from 2020-02-01 until 2021-11-01
    - `U.S._State_and_Territorial_Public_Mask_Mandates_From_April_10__2020_through_August_15__2021_by_County_by_Day.csv` is the masking mandates data I downloaded from the CDC website, specifically for New York County, New York (for data for other counties, please access the CDC website)
    -  `mask-use-by-county.csv` contains the proportion of people rank their willingness to wear masks for each U.S. county
* `/visualization` directory contains all the visualization output results obtained in both my A4 and A5 analysis, all in PNG format. Their names are self-explainatory.
* `/output_data` contains all the output data generated by both my A4 and A5 analysis, specifically:
   - `a4_combined_data.csv` is the output data I generated in A4 that combines the information from all datasources 1 to 3 I mentioned in the previous "Data" section
   - `ridership_popularity.csv` is the output data file I got for my A5 analysis that describes the ridership of New York City's subway system from 2017-02-04 to 2021-08-13
   - `stop_popularity.csv` is the outout file file I generated for my A5 analysis that has the stop popularity data from 2020-02-01 to 2021-08-13
* `a4-common-analysis.ipynb`: The Jupyter notebook that contain the analysis code for A4 (common analysis)
* `a5-ny-subway.ipynb`: The Jupter notebook that contains the analysis code for A5 (my entension study on New York County Subway Ridership)
* `a6-presentation.pptx`: The presentation slides I used for a in-class PetchaKucha presentation session that covers both my results in A4 and A5 with a heavier focus on A5
* `a7-512-final-report-cx.pdf`: The final project report that introces the backgournd of this project, its related work, the methodology used in this porject, the findings, discussions, liminations, conclusions and other resources used in this project


## Notes for user
* For the most up-to-date data, please go to each of my listed datasource to download the newest version
* `U.S._State_and_Territorial_Public_Mask_Mandates_From_April_10__2020_through_August_15__2021_by_County_by_Day.csv` only contains the mask mandates data specifically for New York County. If you want the data for another specific county, go to the CDC website and use the filter functionality
* For the most comprehensive New York City subway data, please use the [MTA Turnstile Data](http://web.mta.info/developers/turnstile.html)

## License
This project is under [The MIT License](https://opensource.org/licenses/MIT)


