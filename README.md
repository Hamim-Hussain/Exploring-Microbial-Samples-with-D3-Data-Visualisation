# belly-button-challenge

### Introduction

Using 'D3' package within the JavaScript libary to create interactive data visualisation . This makes it easy for the audience to see the 'dynamic' data more clearly. The JSON data provided at the given URL contains information about microbial samples taken from various individuals. Each sample is identified by an ID number, and the data for each sample includes an array of the top 10 OTUs (Operational Taxonomic Units) found in the sample, along with the corresponding sample values. 

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

3. Create a bubble chart that displays each sample.

* Use `otu_ids` for the x values.

* Use `sample_values` for the y values.

* Use `sample_values` for the marker size.

* Use `otu_ids` for the marker colors.

* Use `otu_labels` for the text values.

4. Display the sample metadata, i.e., an individual's demographic information.

5. Display each key-value pair from the metadata JSON object somewhere on the page.

6. Update all of the plots any time that a new sample is selected.

## Advanced Challenge Assignment (Optional)

The following task is advanced and therefore optional.

* Adapt the Gauge Chart from <https://plot.ly/javascript/gauge-charts/> to plot the weekly washing frequency of the individual.

* You will need to modify the example gauge code to account for values ranging from 0 through 9.

* Update the chart whenever a new sample is selected.

## Deployment

Deploy your app to a free static page hosting service, such as GitHub Pages or Heroku. Submit the links to your deployment and your GitHub repo.

Here is a [guide](Heroku_Deployment_Guide.md) to deploying your app Heroku. 

## Hints

* Use `console.log` inside of your JavaScript code to see what your data looks like at each step.

* Refer to the [Plotly.js documentation](https://plot.ly/javascript/) when building the plots.
