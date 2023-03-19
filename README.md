# Covid Analysis

## Requirements and Background

```python
import plotly.express as px
import pandas as pd
import plotly.io as pio
import plotly.graph_objects as go
from plotly.subplots import make_subplots
from sodapy import Socrata
```

When a virus replicates its genetic makeup can be slightly changed randomly due to insertions, deletions, or recombinations. These mutations don't usually cause too much of a change in the virus but occassionally it can cause changes in the pathogenicity of the virus. This was quite apparent wih the coronavirus that recently cause a worldwide pandemic. We have seen 4 variants and their various subvariants that have changed the pathogenicity of the virus generally making it easier to spread.

## Analysis

Using the known discovery dates of the different variants we can overlay this with the infection and death counts and rates in order to see how each variant affected the ability of the virus to infect or kill.

![Covid_Analysis](https://user-images.githubusercontent.com/95090904/226202743-abb26fc1-93c0-40eb-a3f6-85579ad60532.png)

A 7 day moving average was added in order to smooth the curve and take out the fluctuation that was occuring in the data. As we can see in the plot above the omicron variant was by far the most effective at infection. This in turn increased the amount of deaths but the mortality rate stayed roughly the same telling us that the new variant didnt have an affect on the mortality rate.

## Geographic Plotting of Cases and Deaths

A Chloropleth map was used to display the case and death load per state. The cloropleth map is very popular and easy to undestand. It provides in most circumstances a great way to visualize data in a geographic manner. This definitely became popularized during the pandemic and gives you a clear idea of where the highest case and death numbers are.

![TotalCases_USA](https://user-images.githubusercontent.com/95090904/226202883-5cc909a0-5451-48e9-9c6e-fb0cfd8d2928.png)

It's clear to see that the three states that had the highest amount of cases are Texas, Florida, and California. 

![Total_Deaths_USA](https://user-images.githubusercontent.com/95090904/226202891-21248261-d430-4511-b9f5-0486fdd04715.png)

We can also see that the three states that had the highest amount of deaths are Texas, Florida, and California which makes sense given the case amount for those three states. 

## Data Sources

Centers for Disease Control and Prevention, COVID-19 Response. 
COVID-19 Case Surveillance Public Data Access, Summary, and Limitations

Data retreived from CDC: https://data.cdc.gov/Case-Surveillance/United-States-COVID-19-Cases-and-Deaths-by-State-o/9mfq-cb36
Variant Information: https://www.who.int/en/activities/tracking-SARS-CoV-2-variants/
