# Overview 
The objective of this project is to train a model that should learn from the data (of California census data) and be able to predict the median housing price in any district in California, given all other attributes. The analysis is intended to help real estate experts price housing depending on the number of rooms, the area it is located and other variables and not to rely on manual guesses.

## Prerequisites
Knime Installed on local / production environment

## Setup
Clone this repository:
```bash
git clone https://github.com/PAnsah98/CHP-.git
```

## Ways to deploy
* KNIME uses a one-click deployment (drag and drop to copy the final workflow to the production server).
* Another deployment option includes model recoding in a traget language(KNIME offers model recoding in Java and SQL), we use DB query and DB SQL Executor nodes.  
* The model can also be deployed as a RESTful service: The workflow implements model prediction as a REST API service, It is accepted as JSON format so we use JSON input, JSON to Table, Table to JSON and output nodes.
* Another deployment mode involves creating an interactive dashboard on a web browser through the KNIME webPortal. The workflow reads data from a file, applies the model, and uses some JS-based visualization nodes to produce the dashboard page for the webportal(check this out)
* The last Deployment option produces a static report and sends an update email. The data could be sent to Tableu or spotfire using the data to report node.
