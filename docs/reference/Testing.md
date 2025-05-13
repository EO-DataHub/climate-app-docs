---
title: Testing
icon: material/book-open-variant-outline
---
# Testing
This page contains suggested test scripts that can be used to test the application.  

## Authentication, asset data and workflow tests

|Details|---------------------------------------------------------|
|---|---|
|Tester name:||
|Date:||
|Time:||

### Test 1 - Logging in and out
|#|Test|Expected result|Tested (Y/N)|Pass / Fail|
|---|---|---|---|---|
|1.1|Login with `sparkgeouser` credentials|User is logged in and stays logged in| | |
|1.2|Logout|User is logged out and stays logged out|||
|1.3|Login with `GitHub` credentials|User is logged in and stays logged in| | |
|1.4|Logout|User is logged out and stays logged out|||

!!! note
    For tests 2 to 4, repeat with both `sparkgeouser` and `GitHub` user
    
### Test 2 - Worklow with sample portfolio
|#|Test|Expected result|Tested (Y/N)|Pass / Fail|
|---|---|---|---|---|
|2.1|Open sample portfolio on [assets] page|Assets loaded on map|||
|2.2|Run LST (Day) workflow|Workflow runs Successfully and shows results on [activity] page||
|2.3|Run LST (Night) workflow|Workflow runs Successfully and shows results on [activity] page||
|2.4|Run OS Climate workflow|Workflow runs Successfully and shows results on [activity] page||

### Test 3 - Workflows with user uploaded portfolio
|#|Test|Expected result|Tested (Y/N)|Pass / Fail|
|---|---|---|---|---|
|3.1|Open CSV of asset data from local computer|Assets load successfully on map||
|3.2|Run LST (Day) workflow|Workflow runs Successfully and shows results on [activity] page||
|3.3|Run LST (Night) workflow|Workflow runs Successfully and shows results on [activity] page||
|3.4|Run OS Climate workflow|Workflow runs Successfully and shows results on [activity] page||

### Test 4 - Workflows with user saved portfolio
|#|Test|Expected result|Tested (Y/N)|Pass / Fail|
|---|---|---|---|---|
|4.1|Open saved portfolio of asset data|Assets load successfully on map||
|4.2|Run LST (Day) workflow|Workflow runs Successfully and shows results on [activity] page||
|4.3|Run LST (Night) workflow|Workflow runs Successfully and shows results on [activity] page||
|4.4|Run OS Climate workflow|Workflow runs Successfully and shows results on [activity] page||


***
[**Next Topic:** User Guide - Getting Started][gettingstarted]

[gettingstarted]: /uk_eodatahub/User%20Guide/b1-getting-started
[about]: /uk_eodatahub/User%20Guide/b2-about
[hazards]: /uk_eodatahub/bUser%20Guide/3-hazards
[observations]: /uk_eodatahub/User%20Guide/b4-observations
[assets]: /uk_eodatahub/User%20Guide/b5-assets
[portfolios]: /uk_eodatahub/User%20Guide/b6-portfolios
[analytics]: /uk_eodatahub/User%20Guide/b7-activity
[activity]: /uk_eodatahub/User%20Guide/b8-activity
[login]: /uk_eodatahubUser%20Guide/b10-login
