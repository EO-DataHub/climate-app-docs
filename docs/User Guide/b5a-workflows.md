---
title: Workflows
icon: material/book-open-variant-outline
---
# Workflows

## Overview
[Workflows] allow you to run analysis on your asset data.  Workflows that have been included within the application include **Land Surface Temperature** analysis workflows, that will allow you to determine the _exposure_ of your asset to variations in LST from the _observations data_.   There is also an **OS Climate Physical Risk** workflow that the _vulnerability_ of certain types of asset resulting from changes in _Chronic Heat_ for a variety of future climate scenarios and years.

## Running an analysis workflow

First you need to open an [assets] dataset - which can either be a _sample portfolio_, a previously _saved portfolio_ or a new file that you have uploaded.  Once the asset dataset has been loaded on the [assets] page, select the **Analyse Assets** option from beneath the asset table.

![Workflows](/uk_eodatahub/images/workflows/1.png "Workflows")

You will then be displayed a list of available workflows.  These provide a brief overview of what the workflow does, along with details of any specific pre-requisites needed in the asset data - for example any particular data columns.  It will also provide details of what geometry types (i.e. point, line or area) are supported in the workflow.
![Workflows](/uk_eodatahub/images/workflows/2.png "Workflows")

Use the **Select Workflow** option to pick the analysis to run.  Some workflows may require you to provide further inputs to the workflow - such as a date range over which to run the analysis.  If this is the case, then enter these details on the following screen. 
![Workflows](/uk_eodatahub/images/workflows/3.png "Workflows")

Finally select **Run analysis**.  Confirmation will be provided in the green box in the bottom right hand corner of the screen that *analysis is in progress**.
![Workflows](/uk_eodatahub/images/workflows/4.png "Workflows")

Once the analysis has finished (which usually takes a couple of minutes) the *analysis in progress* message will be replaced with a **confirmation** that the analysis has finished, and a link to view the analysis results.  

On selecting **View analysis** you are redirected to the [Analytics] page to view the results.
***

***
[**Next Topic:** User Guide - Portfolios][portfolios]

[login]: https://demo.eodh.sparkgeo.dev/login

[gettingstarted]: ../b1-getting-started
[about]: ../b2-about
[hazards]: ../b3-hazards
[observations]: ../b4-observations
[assets]: ../b5-assets
[portfolios]: ../b6-portfolios
[analytics]: ../b7-analytics
[activity]: ../b8-activity
[information]: ../b9-information


