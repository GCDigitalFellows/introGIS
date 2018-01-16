[<<< Previous](linesto.md)  | [Next >>>](more.md)  

# Geoprocessing Tools: Difference

Now we are ready to confront the hydrography buffer versus the elevation. To do this, let’s use a tool called “Difference” in the Vector/Geoprocessing Tools menu. Difference is a function like a geographic substraction: Wherever the two layers meet, the input layer will have substracted whatever trespasses the inner boundaries of the Difference layer. So let’s use the Hydro Buffer as the input and the Elevation Polygon as the Difference layer. Be sure to check the “Ignore invalid input features” so that the operation goes smoothly.

![Geoprocessing Tools: Difference Dialog Box](images/differ1.png)

Now we have a new layer called Difference. We are approaching the end of this brief exercise, so let’s clean the view a bit and turn off the visibility of all layers except for Difference, Blocks Study Area and Elevation Raster (you can turn this last one off if you want to, but it looks nice so you can leave it on). The last step is actually repeating an operation we already did earlier: Clipping. We are going to clip the Blocks Study Area layer using the resulting Difference layer as a clipper, this way, we will have a layer that contains only the Blocks that will actually be vulnerable to the floods. So let’s rename this new “Clipped” layer, and call it “Vulnerable areas”. The resulting layer should look like this:

![Rough Final Result after Clipping](images/differ2.png)

And there we have it. The orange area is the Vulnerable Area. If we look at the attribute table of this layer, we can analyze the characteristics of the vulnerable population, according to the attributes that already existed in the original Census Blocks layer, that is: Population, Age, Race and Gender.

[<<< Previous](linesto.md)  | [Next >>>](more.md)  