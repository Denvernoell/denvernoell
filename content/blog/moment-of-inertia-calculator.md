+++
author = ""
date = ""
description = "My Steps Creating a Moment of Inertia Calculator"
images = []
tags = []
title = "Moment of Inertia Calculator"

+++
In my Design of Steel Structures course, in order to calculate needed values for beams. The Moment of Inertia, Centroid, and related properties need to be calculated. Shapes included in the AISC Steel Manual have these values calculated but if there is a member not included in the manual or if it is a built up member, then it needs to be calculated by hand.

This led me to find a simple example on YouTube in order to break the problem down into variables that could make it work for any situation.

The way it works is to enter the top left and bottom right coordinates of each individual rectangle, counting (0,0) as the bottom left of all points even if it is not part of the object. The shape class takes these and determines the area, length of each side, and the maxes and minimums.

All of the individual shapes are then added to the total class which determines the highest y value, which is needed for the centroid calculation. The centroid for each shape is found and then $\\frac{\\sum{\\overline{y * A}{\\sum{\\overline{y}$ is found to find the centroid of the total shape, which is used for the parallel axis theorem, the $A*d^2$ of the Moment of Inertia calculation.