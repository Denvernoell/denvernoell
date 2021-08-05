+++
author = "Denver Noell"
date = 2021-08-05T07:00:00Z
description = "How to use the Excel tool"
tags = []
title = "Akel Helper"
[[images]]
alt = ""
src = "/uploads/cesar-couto-tihiil6_lhe-unsplash.jpg"
stretch = ""

+++
# Getting Started

Akel Helper is written in python and uses xlwings to interact with excel. Because Akel Helper has a specific set of modules that need to be installed, the easiest way to work with it is to have Anaconda installed. This will allow for the app to run on a python installation that has the required modules.

If Anaconda is installed, running **Akel Helper.bat** will start the app. This will start in your default browser.

# PDF

All of the following

* Create a pdf in the same folder as the current workbook
* If a pdf in the folder shares the same name, it will be moved to OldPdfs and labeled with the number copy it is. (i.e 1st, 2nd, ...)
* Saves pdf path to clipboard

## Current

Creates a pdf of only the current page.

Naming convention - sheet name_date

## Chapter

Creates a pdf of all dark green sheets in the chapter of the current sheet.

Naming convention - workbook name_chapter name_date

## All

Creates a pdf of all dark green sheets in workbook.

Naming convention - workbook name_date

# Sizing

## Display Height

All cells in selection will display the height of the row.

## Set Height

Sets height of each row based on the value of the cell.

## Display Width

All cells in selection will display the width of the column.

## Set Width

Sets width of each column based on the value of the cell.