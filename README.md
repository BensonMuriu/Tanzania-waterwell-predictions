
# Tanzania waterwell status prediction
Tanzania is an East African country with about 59,678,000 in population (2021 est.), and located just south of the Equator. It is a developing country that still has struggles with providing clean water to its entire population. There are many water points already established in the country, but some are in great need of repair while others have failed altogether.

## Data understanding
This project analyzes the Tanzanian Water Wells datasets released by the Tanzanian Government. The dataset includes 59,400 rows each repressenting a unique well within the Tanzanian Governments realm. Our targets are broken down into three categories:

* `Functional `
* `Non Functional`
* `Functional Needs Repair`

We will attempt to predict the status of the wells condition through utilizing Exploratory Data Analysis (EDA) and building classification models tuned to the parameters that will have the largest impact on our predictive ability.

This dataset comes with two applicable files training_set_labels and training_set_values. During our EDA we will join these tables together to give us one file to work with. The values dataset has 39 total columns and contains all of our predicitve features. Below is a description of each column.

* `amount_tsh `: Total static head (amount water available to waterpoint)
* `date_recorded` : The date the row was entered
* `funder `: Who funded the well
* `gps_height` : Altitude of the well
* `installer` : Organization that installed the well
* `longitude` : GPS coordinate
* `latitude `: GPS coordinate
* `wpt_name `: Name of the waterpoint if there is one
* `num_private` :Private use or not
* `basin `: Geographic water basin
* `subvillage` : Geographic location
* `region `: Geographic location
* `region_code` : Geographic location (coded)
* `district_code` : Geographic location (coded)
* `lga` : Geographic location
* `ward` : Geographic location
* `population` : Population around the well
* `public_meeting` : True/False
* `recorded_by `: Group entering this row of data
* `scheme_management` : Who operates the waterpoint
* `scheme_name `: Who operates the waterpoint
* `permit `: If the waterpoint is permitted
* `construction_year` : Year the waterpoint was constructed
* `extraction_type `: The kind of extraction the waterpoint uses
* `extraction_type_group` : The kind of extraction the waterpoint uses
* `extraction_type_class` : The kind of extraction the waterpoint uses
* `management `: How the waterpoint is managed
* `management_group` : How the waterpoint is managed
* `payment `: What the water costs
* `payment_type` : What the water costs
* `water_quality` : The quality of the water
* `quality_group `: The quality of the water
* `quantity `: The quantity of water
* `quantity_group` : The quantity of water
* `source `: The source of the water
* `source_type` : The source of the water
* `source_class` : The source of the water
* `waterpoint_type` : The kind of waterpoint
* `waterpoint_type_group `: The kind of waterpoint

## Requirements

The system requirements are to have `Anaconda environment` pre-Installed to run the models
 
## Business problem

An NGO focused on locating wells needing repair is looking to find patterns in non-functional wells to influence how new wells are built.
## Modelling 
A Model that predicts the status group of the waterpoint is created. A Random forest classifier is found to produce the best model
using pipeline and tuning. The model has an accuracy level of 81%. The model uses features fed into the model and using a binary classifier,
we can predict whether a waterpoint is functional or it has problems all in all.




## Run Locally

Clone the project

```bash
  git clone https://github.com/BensonMuriu/Tanzania waterwell predictions
```

Go to the project directory

```bash
  cd  Tanzania waterwell predictions
```

Install dependencies

```bash
  pip install Anaconda
```

Start the server

```bash
  source activate env
```

