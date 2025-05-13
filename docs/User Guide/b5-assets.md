---
title: Assets
icon: material/book-open-variant-outline
---
# Assets

![Assets](/climate-app-docs/images/navigation/assets.png "Assets"){ align=right }
The [Assets page][assets] is accessed from the left hand navigation bar:

## Overview

The [Assets page][assets] allows you to load assets on to the map and to search, filter and navigate the map to specific assets.  You can either explore some of the sample asset datasets that are included with the application, or upload your own asset data in either `CSV` or `GeoJSON` format.  Once an asset dataset has been opened, you can either view it on top of [hazards][hazards] or [observations][observations] or analyse it using specific analysis workflows.

## Loading sample assets on the map

The application includes some sample portfolios of assets.  From the **Portfolios** dropdown, simply select the *sample dataset* from the list provided.  
![Assets](/climate-app-docs/images/assets/2.png "Assets")

These will automatically be loaded on to the map along with a **table** displaying the asset data.  The **Analyse assets** button will also be enabled, allowing you to run [workflows] on the asset portfolio.

![Assets](/climate-app-docs/images/assets/6.png "Assets")

## Loading your own assets on the map

!!! note "Log in first"
    Before you can load your own assets on to the map, you need to log in.  Check out details on the [login] page of this documentation site if you are unfamiliar with how to do this.

To load your own assets, simply select **+ Open file** next to right of the **Portfolios** dropdown and select either a **CSV** or **GeoJSON** file.
![Assets](/climate-app-docs/images/assets/3.png "Assets")

A **CSV** file of point data must be include **ID**, **Latitude** and **Longitude** columns, but can also include other columns, for example:

|id|latitude|longitude|name|
|---|---|---|---|
|1|51.5007|-0.1245|Big Ben|
|2|51.5034|-0.1345|10 Downing Street|

The **case** of the column names does not matter.  The file will then be validated to ensure it is compatible with the application.  Select **Load assets** to add these on to the map.

![Assets](/climate-app-docs/images/assets/4.png "Assets")

## Viewing all columns

If your **CSV** file has more columns than just the **ID**, **Latitude** and **Longitude** are displayed.  To view additional columns in the dataset, select the **eye** icon above the asset table.

![Assets](/climate-app-docs/images/assets/5.png "Assets")

## Filtering assets

It is also possible to filter the asset table with a keyword match. Simply type the keyword into the search table.  In the example below a **schools** dataset includes a *local authority* field.  Typing in the term `Richmond` in the search box has found all those schools within that authority.  Note, if any of the schools had *Richmond* in their name, these would also be displayed.  The map then automatically zooms to the assets that are filtered in the table.  Simply delete the text from the text entry box to display all assets once again.

![Assets](/climate-app-docs/images/assets/6.png "Assets")

## Zoom to a specific asset

To zoom to a specific asset or group of assets, use the check box in the table to select the asset.  The map will then zoom automatically.

## Viewing assets on observations and hazards pages

Once you have opened an asset dataset from within the [assets] page, you can then view the asset data overlayed on both the [observations] and [hazards] pages.  The menu options in those pages will now include the opened file - called **Portfolio 1** in the list of available datasets.

## Analysing assets

After an asset dataset has been loaded on to the map, the **analyse assets** button is displayed beneath the table in the [assets] page.  This will display the **workflow selector** where you can chose the type of analysis that you want to undertake on your assets.

For more information on workflows, check out the [workflows] page in this *User Guide*.

***
[**Next Topic:** User Guide - Workflows][workflows]

[assets]: https://demo.eodh.sparkgeo.dev/assets

[hazards]: ../b3-hazards
[observations]: ../b4-observations
[login]: ../bb1-login
[workflows]: ../b5a-workflows
