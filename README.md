<div id="devex-badge"><a rel="Delivery" href="https://github.com/BCDevExchange/docs/blob/master/discussion/projectstates.md"><img alt="In production, but maybe in Alpha or Beta. Intended to persist and be supported." style="border-width:0" src="https://assets.bcdevexchange.org/images/badges/delivery.svg" title="In production, but maybe in Alpha or Beta. Intended to persist and be supported." /></a></div>

---

## Analysis of trends in groundwater levels in B.C.

This is a set of [R](http://www.r-project.org) scripts to reproduce the 2013 analysis of trends in groundwater levels presented on [Environmental Reporting BC](http://www.env.gov.bc.ca/soe/indicators/water/groundwater-levels.html). 

The scripts use the [bcgroundwater](https://github.com/bcgov/bcgroundwater/) package and groundwater monitoring data from the [B.C. observation well network](http://www.env.gov.bc.ca/wsd/data_searches/obswell/index.html) to analyze long-term trends of groundwater levels and produce summary visualizations as well as individual well statistics.

### Usage

**Data**

- Raw groundwater level data can be downloaded from the 
  [B.C. Observation Well Network](http://www.env.gov.bc.ca/wsd/data_searches/obswell/map/obsWells.html).
    - Median monthly groundwater levels are available under the 
      [Open Government Licence - British Columbia](http://www2.gov.bc.ca/gov/content?id=A519A56BC2BF44E4A008B33FCF527F61) 
      as a direct download from the
      [B.C. Data Catalogue](https://catalogue.data.gov.bc.ca/dataset/84c06668-8a1e-4629-90a3-051bba903f22).
      If you would prefer to run the analysis beginning with these data rather than 
      downloading the individual raw data files, set the `downloadMonthly` variable
      to `TRUE` at the top of `01_clean.R`
- Well attribute data are included as a zip file in the `data` folder. They are available from the
  [B.C. Data Catalogue](http://catalogue.data.gov.bc.ca/dataset/ground-water-wells-spatial-view-with-attribute-info),
   under the [Open Government Licence – British Columbia](http://www2.gov.bc.ca/gov/content?id=A519A56BC2BF44E4A008B33FCF527F61)
- Natural Resource Regions used in the summaries are included as a zip file in the `data` folder. They are available from the
  [BC Data Catalogue](https://catalogue.data.gov.bc.ca/dataset/dfc492c0-69c5-4c20-a6de-2c9bc999301f) under the 
  [Open Government License–British Columbia](http://www2.gov.bc.ca/gov/content?id=A519A56BC2BF44E4A008B33FCF527F61)

**Code**

There are four core scripts that are required for the analysis, they need to be run in order:

- 01_clean.R
- 02_analysis.R
- 03_visualize.R
- 04_output.R

### Project Status

The results of our analysis can be downloaded as a .csv in the 
[data](http://www.env.gov.bc.ca/soe/indicators/water/groundwater-levels.html) 
section of the indicator page.

We are not actively developing this analysis, but you can check the 
[issues](https://github.com/bcgov/groundwater_levels/issues/) for things we would 
like to fix or work on.

### Getting Help or Reporting an Issue

To report bugs/issues/feature requests, please file an [issue](https://github.com/bcgov/groundwater_levels/issues/).

### How to Contribute

If you would like to contribute, please see our [CONTRIBUTING](CONTRIBUTING.md) guidelines.

Please note that this project is released with a [Contributor Code of Conduct](CODE_OF_CONDUCT.md). By participating in this project you agree to abide by its terms.

### License

    Copyright 2015 Province of British Columbia

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at 

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

This repository is maintained by [Environmental Reporting BC](http://www2.gov.bc.ca/gov/content?id=FF80E0B985F245CEA62808414D78C41B). Click [here](https://github.com/bcgov/EnvReportBC-RepoList) for a complete list of our repositories on GitHub.


