---
title: Getting Started
icon: material/book-open-variant-outline
---
# Getting Started

The vertical navigation bar on the left hand side of the screen provides access to the main features of the Climate Application.  

![Hazard indicator alt text](/climate-app-docs/images/navigation/navbar.png "Hazard indicator title")

This page provides an overview of the various options accessible from this navigation bar.

!!! note
    Some features require logging in using an EODH account.  Details on user accounts are available in the [login documentation page][login].

## About

![About](/climate-app-docs/images/navigation/about.png "About"){ align=right }
The [About page][about] is the home page for the application and includes an introduction to the project and its contibutors.

## Hazards

![Hazards](/climate-app-docs/images/navigation/hazards.png "Hazards"){ align=right } The [Hazards page][hazards] allows you to view *Hazard Indicators* on the map and overlay your own asset data on top.  *Hazard Indicators* are datasets that are derived from Climate Projections that provide metrics for key climate indicators under a variety of future climate scenarios.  An example of a *Hazard Indicator* for *Chronic Heat* is the number of days per year that the average temperature is expected to exceed a particular threshold.  These indicators can be used to understand the potential exposure of assets to different risks in future.

## Observations

![Observations](/climate-app-docs/images/navigation/observations.png "Observations"){ align=right }
The [Observations page][observations] allows you to view Earth Observation data on the map and overlay your own asset data on top.  Observations, such as *Land Surface Temperature* provide historic insights that are at a finer "spatial resolution" (i.e. more granular) than climate projection data.  *Observation data* may comprise of both daily observations or monthly averages, helping us understand how assets might be exposed during particular scenarios - such as during a heatwave - or explore trends in changes of monthly averages.

## Assets

![Assets](/climate-app-docs/images/navigation/assets.png "Assets"){ align=right }
The [Assets page][assets] allows you to load assets on to the map and to search, filter and navigate the map to specific assets.  You can either explore some of the sample asset datasets that are included with the application, or upload your own asset data in either `CSV` or `GeoJSON` format.  Once an asset datasets has been opened, you can either view it on top of [hazards][hazards] or [observations][observations] or analyse it using specific analysis workflows.

## Portfolios

![Portfolios](/climate-app-docs/images/navigation/portfolios.png "Portfolios"){ align=right }
A [Portfolio][portfolios] is an asset dataset that has been uploaded to your own personal storage area on the hub and is stored persistently.  *Portfolios* will therefore be available to you next time you log in, thereby saving the inconvenience of needing to upload your assets each time.  The [Portfolios page][portfolios] provides you with some tools to manage these portfolio datasets (for example deleting those that are no longer needed).

## Workflows

[Workflows] allow you to run analysis on your asset data.  Workflows that have been included within the application include **Land Surface Temperature** analysis workflows, that will allow you to determine the *exposure* of your asset to variations in LST from the *observations data*.   There is also an **OS Climate Physical Risk** workflow that the *vulnerability* of certain types of asset resulting from changes in *Chronic Heat* for a variety of future climate scenarios and years.

## Analytics

![Analytics](/climate-app-docs/images/navigation/analytics.png "Analytics"){ align=right }
The [Analytics page][analytics] displays the results of any workflows that you have executed on your asset portfolio.  *Workflow analysis* can be called from the *hazards*, *observations*, and *assets* pages once an asset dataset has been uploaded or opened from an existing portfolio.

## Activity

![Activity](/climate-app-docs/images/navigation/activity.png "Activity"){ align=right }
The [Activity page][activity] page lists all the workflows that have been executed on your asset portfolios including the history of whether they were successful or had any errors.  For historic workflows, you are able to load up the results of the previous analysis, which will then be displayed in the [Analytics page][analytics].

## Information

![Information](/climate-app-docs/images/navigation/information.png "Information"){ align=right }
The [Information page][information] provides access to this documentation.

## Login

![Login](/climate-app-docs/images/navigation/login.png "Login"){ align=right }
The [Login page][login] page allows you to log in and out of your EODH account.  More details on logging in are included on the login help page.

***
[**Next Topic:** User Guide - Hazards][hazards]

[about]: ../b2-about
[hazards]: ../b3-hazards
[observations]: ../b4-observations
[assets]: ../b5-assets
[portfolios]: ../b6-portfolios
[analytics]: ../b7-analytics
[activity]: ../b8-activity
[information]: ../b9-information
[login]: ../bb1-login
[workflows]: ../b5a-workflows
