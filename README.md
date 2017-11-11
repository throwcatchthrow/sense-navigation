# sense-navigation
> Sense Sheet Navigation + Actions visualization extension for Qlik Sense.

---
[![Codacy Badge](https://api.codacy.com/project/badge/Grade/84d52444a6084f6cb3694424a968b036)](https://www.codacy.com/app/stefan-walther/sense-navigation?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=stefanwalther/sense-navigation&amp;utm_campaign=badger)
---

![](https://raw.githubusercontent.com/stefanwalther/sense-navigation/master/docs/images/sense-navigation.png)

---
## Table of Contents

- [Purpose and Description](#purpose-and-description)
- [Screenshots](#screenshots)
- [Installation & Download](#installation--download)
- [Configuration](#configuration)
- [Compatibility](#compatibility)
- [Room for improvement / contribution](#room-for-improvement--contribution)
- [Contributing](#contributing)
- [Related projects](#related-projects)
- [Authors & Contributors](#authors--contributors)
  * [Contributors](#contributors)
- [License](#license)
- [Change log](#change-log)

_(TOC generated by [verb](https://github.com/verbose/verb) using [markdown-toc](https://github.com/jonschlinkert/markdown-toc))_

---

## Purpose and Description
The Visualization Extension ***sense-navigation*** for Qlik Sense allows you to add a button to a Qlik Sense sheet to navigate in your app:

* Go to the next sheet
* Go to the previous sheet
* Go to a specific sheet
* Go to a sheet (defined by the sheet Id)
* Go to a story
* Open a website
* Switch to the edit mode

The button can be easily styled nicely by selecting some of the predefined designs.

Furthermore ***sense-navigation*** offers the option to define **actions**~ which will be executed **before** the navigation happens.
This could for example be:

* Apply a bookmark
* Clear selections
* Lock selections
* Unlock selections
* Select value(s) in a field
* Select alternatives
* Select possible values in a field
* Set a variable value

See [here](./docs/actions.md) for a complete list of all available 20 actions.

Note: The main difference between version 0.x and 1.x of sense-navigation is that with v1.x you can define more than two actions.

## Screenshots
### Button styles

There are several predefined styles available, you can choose from:

> ![](https://raw.githubusercontent.com/stefanwalther/sense-navigation/master/docs/images/sense_navigation_styles.png)

### Button icons
Every button can also include an icon:

> ![](https://raw.githubusercontent.com/stefanwalther/sense-navigation/master/docs/images/sense_navigation_button_icons.png)

**sense-navigation** uses the [Fontawesome icons](http://fontawesome.io/), therefore you can select from a collection of 675 icons.

###

## Installation & Download
### Fresh Installation

0. **Do not download the entire Github repository, this will not work!**
1. Download the [latest version](https://github.com/stefanwalther/sense-navigation/raw/master/build/sense-navigation_latest.zip) or [any other version](https://github.com/stefanwalther/sense-navigation/tree/master/build) you want to install.
2. Then install on either *Qlik Sense Desktop* or *Qlik Sense Server*:

* Qlik Sense Desktop
	* To install, unzip all files and copy the content to the folder folder `"C:\Users\%USERNAME%\Documents\Qlik\Sense\Extensions\sense-navigation"`
* Qlik Sense Server
	* See instructions [how to import an extension on Qlik Sense Server](http://help.qlik.com/sense/2.0/en-US/online/#../Subsystems/ManagementConsole/Content/import-extensions.htm)

### You are already using an **sense-navigation** version 0.x?

* I have unfortunately bad news: Version 0.x of **sense-navigation** does not seamlessly upgrade to version v1.x of **sense-navigation**!
* If you upgrade to v1.x, you will have to
  * First install new new version of **sense-navigation**.
  * Delete existing old instances of **sense-navigation**.
  * Add it again to your sheets and apply the previous configurations.

## Configuration
Drag & drop the object onto a sheet (as you would do it with any other native object or visualization extension).
Then define how the **sense-navigation** should behave:

- [Layout Options](./docs/config-layout.md)
- [Navigation Behavior](./docs/config-navigation-behavior.md)
- [Actions](./docs/config-actions.md)

## Compatibility
**sense-navigation** is designed to work with Qlik Sense *September 2017* or higher.
If you want to use _sense-navigation_ in older versions, install an older version than v1.0.

### **sense-navigation** & Mashups

**sense-navigation** it built to be used within the Qlik Sense Client.
Any usage in a mashup-based solution might work, but there are many features in **sense-navigation** which can never work in a mashup-based solution (e.g. "Go to next sheet", "Go to edit mode", etc.).
So use **sense-navigation** in a mashup-based solution only at your own risk!

## Room for improvement / contribution
* Allow to add **additional styles for the button** (very similar to [sense-themable-kpi-tile](https://github.com/stefanwalther/sense-themable-kpi-tile))
* Allow templates for buttons ([see here](https://github.com/stefanwalther/sense-navigation/issues/14))
* **Additional actions**, e.g.
	* Reload the app
	* Opening another app and pass the current selections to the app (similar to "document chaining in QlikView")
* Allow icons instead of images ([see here](https://github.com/stefanwalther/sense-navigation/issues/37))
* Select fields instead of defining fields in the expression editor ([see here](https://github.com/stefanwalther/sense-navigation/issues/25))
	
Is there **anything else you'd like to see** in this visualization extension?

* Don't hesitate to add the feature and create a pull request!
* You don't have the time or skills to implement this specific feature? No problem, [drop a note here](https://github.com/stefanwalther/sense-navigation/issues).

## Contributing
Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](https://github.com/stefanwalther/sense-navigation/issues).
The process for contributing is outlined below:

1. Create a fork of the project
2. Work on whatever bug or feature you wish
3. Create a pull request (PR)

I cannot guarantee that I will merge all PRs but I will evaluate them all.

### Building the project

See [https://github.com/stefanwalther/sense-extension-contrib](https://github.com/stefanwalther/sense-extension-contrib)

## Related projects
Some related projects (Qlik Sense Visualization Extensions) I have recently created:

- [qliksense-extension-tutorial](https://www.npmjs.com/package/qliksense-extension-tutorial): Comprehensive tutorial to start developing Qlik Sense Extensions. | [homepage](https://github.com/stefanwalther/qliksense-extension-tutorial "Comprehensive tutorial to start developing Qlik Sense Extensions.")
- [sense-calendar-heatmap](https://www.npmjs.com/package/sense-calendar-heatmap): Qlik Sense Visualization Extension with a diverging color scale. The values are displayed as colored… [more](https://github.com/stefanwalther/qsCalendarHeatmap) | [homepage](https://github.com/stefanwalther/qsCalendarHeatmap "Qlik Sense Visualization Extension with a diverging color scale. The values are displayed as colored cells per day. Days are arranged into columns by week, then grouped by month and years.")
- [sense-extension-recipes](https://www.npmjs.com/package/sense-extension-recipes): Recipes on working with Qlik Sense Visualization Extensions. | [homepage](https://github.com/stefanwalther/sense-extension-recipes "Recipes on working with Qlik Sense Visualization Extensions.")
- [sense-funnel-chart](https://www.npmjs.com/package/sense-funnel-chart): Funnel Chart for Qlik Sense. | [homepage](https://github.com/stefanwalther/sense-funnel-chart "Funnel Chart for Qlik Sense.")
- [sense-media-box](https://www.npmjs.com/package/sense-media-box): Include web pages, videos, images and much more into your Qlik Sense app. | [homepage](https://github.com/stefanwalther/sense-media-box "Include web pages, videos, images and much more into your Qlik Sense app.")
- [sense-on-off-switch](https://www.npmjs.com/package/sense-on-off-switch): Set a variable in Qlik Sense to true/false using an on-off switch. | [homepage](https://github.com/stefanwalther/sense-on-off-switch "Set a variable in Qlik Sense to true/false using an on-off switch.")
- [sense-qr-code](https://www.npmjs.com/package/sense-qr-code): QR Code to be embedded into Qlik Sense. | [homepage](https://github.com/stefanwalther/qsQRCode "QR Code to be embedded into Qlik Sense.")
- [sense-range-slider](https://www.npmjs.com/package/sense-range-slider): Slider object for Qlik Sense to manipulate one or two variables. | [homepage](https://github.com/QlikDev/qsRangeSlider "Slider object for Qlik Sense to manipulate one or two variables.")
- [sense-themable-kpi-tile](https://www.npmjs.com/package/sense-themable-kpi-tile): KPI Tile for Qlik Sense with the ability to use themes or to customize background… [more](https://github.com/stefanwalther/sense-themable-kpi-tile) | [homepage](https://github.com/stefanwalther/sense-themable-kpi-tile "KPI Tile for Qlik Sense with the ability to use themes or to customize background color, comparison indicator, etc.")  

## Authors & Contributors
**Stefan Walther**

* [qliksite.io](http://qliksite.io) - Qlik Sense / QAP related blog
* [qlikblog.at](http://qlikblog.at) - QlikView related blog
* [stefanwalther.io](http://stefanwalther.io) - Private blog
* [twitter/waltherstefan](http://twitter.com/waltherstefan)  
* [github.com/stefanwalther](http://github.com/stefanwalther)  

### Contributors
- [rvaheldendaten](https://github.com/rvaheldendaten)
- [rjriel](https://github.com/rjriel)

## License
MIT

## Change log
See [CHANGELOG.yml](https://github.com/stefanwalther/sense-navigation/blob/master/CHANGELOG.yml)  

***

_This file was generated by [verb-generate-readme](https://github.com/verbose/verb-generate-readme), v0.6.0, on November 11, 2017._

