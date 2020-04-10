# CovidMonitor.info API - Italy Statistics Viewer
A simple implementation example of CovidMonitor.info API to retrieve JSON data about COVID-19 in Italy.
You can easily code your own COVID-19 Statistics Viewer.

# What is CovidMonitor.info?
CovidMonitor is a project that I developed to monitor the spread of the COVID-19 virus and displays it on an interactive density heatmap. You can use it as a data source to retrieve your desired informations.

![Thumbnail www.covidmonitor.info](https://github.com/vincenzot/CovidMonitor-API-Italy-Statistics-Viewer/blob/master/thumb.PNG?raw=true)

# API Usage
You can use CovidMonitor API with this URL:

<pre>
https://covidmonitor.info/api/get.php?type=<b>[TYPE VALUE]</b>&date=<b>[DATE VALUE]</b>
</pre>
There are two mandatory GET request fields to fill:

| Field | Description | Values |
| --- | --- | --- |
| type | It is the type based on area | national, regional, provincial |
| date | You can choose between today data or all days data  | latest, all |

## Type values

| Value | Description |
| --- | --- |
| national | Get national data |
| regional | Get regional data  |
| provincial |Get provincial data  |

## Date values

| Value | Description |
| --- | --- |
| latest | Get latest update day data |
| all | Get all day data  |

## Response Data Structure

This is an example JSON response.
<pre>
[
    {
        "date": "2020-04-09T17:00:00",
        "state": "ITA",
        "hospitalized_with_symptoms": 28399,
        "intensive_therapy": 3605,
        "total_hospidalized": 32004,
        "home_isolated": 64873,
        "total_positive": 96877,
        "variance_total_positive": 1615,
        "new_infected": 4204,
        "discharged_recovered": 28470,
        "deaths": 18279,
        "total_infected": 143626,
        "swabs": 853369,
        "note_it": "",
        "note_en": ""
    }
]
</pre>

# Instructions
1. Download this repository;


# Author

**Vincenzo Tartaglia**

  - http://github.com/vincenzot
  - https://www.linkedin.com/in/vincenzotartaglia/
  - http://stackoverflow.com/users/5861977/vincenzo-tartaglia
