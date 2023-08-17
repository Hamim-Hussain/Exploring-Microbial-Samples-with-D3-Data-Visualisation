# belly-button-challenge
<img src="Images/microbs.JPG" width="1000" height="491">

## Introduction

D3 is a JavaScript library used to create interactive data visualizations, which can help the audience better understand dynamic data. The JSON data available at the specified URL provides information about microbial samples collected from different individuals. Each sample is identified by a unique ID number, and its data includes an array of the top 10 Operational Taxonomic Units (OTUs) found in the sample, along with their corresponding values. 

## Sources of data

URL: https://2u-data-curriculum-team.s3.amazonaws.com/dataviz-classroom/v1.1/14-Interactive-Web-Visualizations/02-Homework/samples.json

## Findings

- There are 153 different sample IDs, ranging from "BB_940" to "OTU_999".
- Each sample has an array of 10 OTUs, identified by their numeric ID (e.g. "OTU_1167").
- For each OTU, there is a corresponding sample value indicating the number of times that OTU was found in the sample.

## Conclusion

- There is considerable variation in the number of OTUs found in each sample, with some samples having fewer than 10 OTUs and others having more.
- Some OTUs are much more common than others, with the top OTU ("OTU_1") appearing in over 50% of the samples.
- There is also considerable variation in the relative abundance of OTUs within each sample, with some OTUs having much higher sample values than others.

# Project Outline

## Instructions

1. Use the D3 library to read in `samples.json`.

2. Create a horizontal bar chart with a dropdown menu to display the top 10 OTUs found in that individual.

* Use `sample_values` as the values for the bar chart.

* Use `otu_ids` as the labels for the bar chart.

* Use `otu_labels` as the hovertext for the chart.

![](Images/hw01.png)

3. Create a bubble chart that displays each sample.

* Use `otu_ids` for the x values.

* Use `sample_values` for the y values.

* Use `sample_values` for the marker size.

* Use `otu_ids` for the marker colors.

* Use `otu_labels` for the text values.

![](Images/bubble_chart.png)

4. Display the sample metadata, i.e., an individual's demographic information.

5. Display each key-value pair from the metadata JSON object somewhere on the page.

![](Images/hw03.png)

6. Update all of the plots any time that a new sample is selected.
Additionally, you are welcome to create any layout that you would like for your dashboard. An example dashboard is shown below:
![](Images/hw02.png)

## Advanced Challenge Assignment (Optional)

The following task is advanced and therefore optional.

* Adapt the Gauge Chart from <https://plot.ly/javascript/gauge-charts/> to plot the weekly washing frequency of the individual.

* You will need to modify the example gauge code to account for values ranging from 0 through 9.

* Update the chart whenever a new sample is selected.

![](Images/gauge.png)

## Deployment

Deploy your app to a free static page hosting service, such as GitHub Pages or Heroku. Submit the links to your deployment and your GitHub repo.

Here is a [guide](Heroku_Deployment_Guide.md) to deploying your app Heroku. 

## Hints

* Use `console.log` inside of your JavaScript code to see what your data looks like at each step.

* Refer to the [Plotly.js documentation](https://plot.ly/javascript/) when building the plots..
