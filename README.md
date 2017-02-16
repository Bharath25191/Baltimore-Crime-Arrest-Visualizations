# Baltimore-Crime-Arrest-Visualizations<br>
</h>A visualization project on Crime/Arrest characteristics of Baltimore City Province</h>

<b>Introduction</b>
The aim of this project is to study the Crime and Arrest public datasets of Baltimore for understanding the pattern through visualization and to derive meaningful insights from these visualizations. Making use of the coordinates of the crimes, the police department can understand the trends of crime with respect to the time and location, these analyses will help them answer key questions like identifying the sensitive areas, the time at which most crimes occur, crime types etc. These studies will help them come up with better strategies to cope with crimes. I have also made a comparison between the crimes and arrests to analyse the efficiency of the police forces using an array of visualizations.<br>
<b>Data Source</b>
The data was fetched from the Baltimore Government site by downloading the arrests and crimes data in CSV format. The site also provides a SODA API to get live data, but it has a limitation of fetching only 50,000 records. As both the datasets are big (more than 100000 records), I preferred uploading the dataset rather than API calls, as it provides a faster access and doesn’t impose any limitation on the records.
The datasets have information such as Metadata: Arrest-ID, Age, Sex, Crime Date, Arrest Date, crime type, locations etc.
While all the fields provide significant information about the nature of the crime and arrest, I have filtered certain fields for the visualizations.<br>
The Data sources can be explored through the link https://data.baltimorecity.gov/<br>

<b>Technology Used</b>
Anaconda Python Notebook was used to do the cleansing, data transformation and visualizations.
<br>
<br>
<b>Process</b><br>
The project was mainly divided into two parts:

1.	Data Cleansing 
2.	Data Visualization
<br><br>

<b>Data Cleansing</b>:
The first step was to load both the datasets into the Jupyter Notebook. After loading the data was analysed in terms of missing rows, data types of columns, relevance of fields etc.
It was observed that the timestamp was in the format of yyyymmdd hhmmss. So, it required processing to extract the data and time details.
The coordinates were also stacked to a single field and a logic was developed to separate them into latitudes and longitudes.
The unnecessary fields were then identified and dropped from the datasets for better clarity while visualizing and to save processing time.
The rows which had null values were then removed to obtain cleansed CSV files, this process was carried out for both the datasets.
<br><br>

<b>Data Visualization</b>:
I made the following visualizations to derive insights from the datasets: -
1.	Line plot
2.	Bar Graph
3.	Geocoded Heat Maps
4.	Terrain Maps
5.	Heat Maps

