# SPARClink
SPARClink: Visualizing the Impact of SPARC

## What is SPARClink?
SPARClink is a tool that shows the impact of SPARC generated datasets and their publications on the overall research landscape. This tool is meant to create interactive visualizations (graphs) on the relationships (citations) between datasets, protocols, publications, and other external resources. This project was created during the 2021 SPARC FAIR Codeathon.

## How it works
Metadata information is extracted from [Pennsieve](https://app.pennsieve.io/), and the SPARC Airtable database. This information is queried against the [NIH Reporter](https://api.reporter.nih.gov/) and [Google Scholar](https://serpapi.com/google-scholar-api) to extract citations and create a well connected graph using [d3.js](https://d3js.org/). 

<p align="center">
  <img src="https://user-images.githubusercontent.com/21206996/125478715-d5f83b6f-8a6d-4ef8-a845-952baa27d8da.png" />
  <br/>
  <span> SPARClink workflow </span>
</p>

## Run the project
The development environment uses Anaconda to keep track of the python dependencies. Download Anaconda here: [Anaconda Individual Edition](https://www.anaconda.com/products/individual)

``` bash
git clone https://github.com/SPARC-FAIR-Codeathon/SPARClink.git
cd SPARClink
conda env create -f environment.yml
conda activate sparclink

## Run the backend python server
cd backend
python api.py

## Run the front end
cd frontend
npm install
```


Keep track of the project [here](https://github.com/SPARC-FAIR-Codeathon/SPARClink/projects/1)

## Created by 
* Sanjay Soundarajan
* Monalisa Achalla
* Jongchan Kim
* Ashutosh Singh
