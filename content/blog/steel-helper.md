+++
author = "Denver Noell"
date = 2021-03-09T00:00:00Z
description = "How to use Steel Helper sites"
tags = ["Steel", "Civil Engineering"]
categories = ["Current"]
removeBlur = true
title = "Steel Helper"
[[images]]
  src = "img/loopstaircase1.jpg"
  alt = "Desert Scene"
  stretch = "cover"
+++

Starting my Steel class, I could tell immediately that the problems in this class had lots of opportunity to be programmed due to the reliance on code. This means that any cutting back on referring to the code book can be very beneficial.

While solving problems I found that although there were many different starting conditions, most of the problems were to determine the same outputs. Because of this I created an ending function that took all of the outputs from previous functions to output the required strengths.

This became repetitive and my functions started having more and more inputs. One of the problems with this is if there is a new process that requires different inputs or has different outputs, there is the potential to not be compatible with later functions. This led me to learning about Object Oriented Programming.

Object Oriented Programming allowed me to cut the amount of inputs and outputs in each function

One of the things that is most beneficial about this method is the implementation of the pint library. This library is used to apply units to values and is able to convert between them. This means that if an equation like the following would output 3.5 feet instead of 9. This was very helpful when the inputs could be of varying units and eliminates the need to account for unit conversions.
$$3 feet + 6 inches$$

In order to determine the properties for a shape, the Steel Construction Manual tables needed to be checked for each shape used. I found a shapes database file on the AISC website which contained all of these values in an Excel file. This allowed me to use the pandas library to extract the needed values, and apply their units using pint syntax. This took out the potential errors that can come with pulling values from a book manually or needing to reference the same values multiple times in a single problem.

Things I learned:

1. Object Oriented Programming
2. Module creation and upload to Pypi
