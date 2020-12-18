# CS50 - Final Project

An app that dynamically generates a table of filtered records based on a provided dataset utilizing JavaScript and DOM manipulation, HTML, and CSS.
It allows users to filter the dataset using specific values provided by users.

### The App

A fun app for the UFO fans. Users are provided with a dynamically generated table of UFO reports based on a user filter-choice.
The user can set multiple filters and search for very specific UFO sightings in the provided dataset very fast and easy.
However, if user seeks a larger output or less unique records, the UFO dataset can be filtered using only one/two filter(s).
The app itself is simple, intuitive, and easy to use. 

The dataset can be filtered by any/all of the following criteria:

* date
* city
* state
* country
* UFO shape

The app consists of two webpages, where the first page is a title page with a button, which redirects user to the second page when clicked,
and the second page has a vertical panel with filters for user to use and a table for the filtered outputs.

### Filters

The following filters are **not case sensitive**: 

* city 
* state 
* country 
* shape

The user can use all upper case, all lower case or the mix of both to input values for any of those filters.

The ***"date"*** filter accepts only one digit for one-digit days and months, which means that there is no need to use zero in front of a one-digit day or month. 
For example, if it is January 5, 2010 (01/05/2010) then the input should be 1/5/2010.

The ***“city”*** filter should have a full name of a searched city. It is case insensitive.

The ***“state”*** filter accepts only two-letter state abbreviations and it is case insensitive.

The ***“country”*** filter accepts only two-letter country abbreviations (us, ca, au) and it is case insensitive.

To filter the table based on the selected filters, user has to click the ***“Filter Table”*** button on the filters panel.

All filters can be cleared at once by clicking ***“Reset Table”*** button on the filters panel, in which case, the table will reset to its original state.

### Table

All filtered data is shown in the table. The table has the following seven columns:

* date
* city
* state
* country
* shape
* duration
* comments

Where ***“duration”*** column shows duration of a UFO sight in minutes, and ***“comments”*** column shows various comments for each record.

If, based on selected filters, no data is found in the UFO dataset then the user will get a message, stating that there are no results, 
and the table will output **N/A** for each column.

### Dataset

The records of UFO sightings are provided by **National UFO Reporting Center (NUFORC)**. 

The dataset has been retrieved from **Kaggle**: [https://www.kaggle.com/NUFORC/ufo-sightings](https://www.kaggle.com/NUFORC/ufo-sightings). 

The app works with provided dataset in the form of an array of JavaScript objects, and for the sake of memory conservation, 
the dataset has been significantly shortened, but the app works with a full version of the dataset as well.  
