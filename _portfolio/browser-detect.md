---
layout: single
title:  "Browser Detect"
author_profile: true
comments: true
share: true
---

Detect user's browser settings to aid in SaaS Support team troubleshooting. When users give permission, their browser information is saved to the database for Support users to examine.

## Demo
View the [live demo](https://browser-detect.herokuapp.com/). _This may take minute to load on first click as this is hosted for free on Heroku and the dyno has to start up._

## Code
View this project on [GitHub](https://github.com/meagerfindings/browser_detect).


## Features

Detects the following about Visitor's Browsers:
- Adblock Enabled
- Browser & Version
- OS & Version
- IE:
    - Compatibility Mode
- Sends email with visitor's browser information upon submission.
    - _Email recipient is set by the environment variable:_ `EMAIL_TARGET`
- Visitors can create an account to see, edit, and delete previous browser submissions submitted with their email
- Employees can create an account in order to add Browser, Versions, Issues and view and edit the visitor records.

Warns users regarding:
- Adblock
- IE Compatibility Mode
- Currently known issues with user's browser. Checks against internal database for this information.
- When browsers are more than 2 versions out of date.

UUIDs are used for Visitor ID's and User ID's for obscurity and to allow visitors to share their uniquely generated ID with the Support team for reference.

Website name can be set globally through ENV Variable: `COMPANY_WEBSITE_NAME`.
