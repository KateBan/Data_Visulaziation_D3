## Summary
The depicted visualization is a scatterplot that shows how volatile and citric acids affect the quality of both red and white wines. What I wanted to represent is that for red wine both of the acids affect its quality, while there is no connection between quality and the acids for white wine. Also, the values of both acids seem to be mirrored.

## Design
### First attempt
"Photo_1" presents my initial idea. The X axis would represent the red and white colors of the wine; the Y axis would represent the median values of the citric and volatile acid. The size of the bubbles would represent the quality rating of the wine. A gridline would separate the X axis due to color separation. Initially, the bubbles would be with opacity 0.1. Upon hovering over the scatterplot, the bubbles that are from the same acid category would appear in bright colors and then disappear. Though this did not work out so, I changed the design.

### Second attempt
"Photo_2" represents the next idea. The X axis represents the quality ratings; the Y axis represents the median values of the volatile and the citric acids. To encode the different wine colors, I though to make the sizes for the bubbles different. Big for the red wine and small for the white wine, and keep the colors for both wines the same for a specific acid. They would be again with initial opacity 0.1 which would get to 1 upon hovering over the plot. I also added gridlines on the X and Y axis for clarity and add a light gray color to the background. Also, when the mouse is on a given bubble, a message shows up that says from which acid, wine color and quality rating the bubble is. The plot can be seen here: http://bl.ocks.org/KateBan/raw/852a05c924619f3bbff0/. 

### Third attempt
After getting feedback, I changed the color of the bubbles to suit the color of the according wine. Red bubble = red wine, white bubble = white wine. This way I believe there is not need of a legend for the colors because the visualization is self-explanatory. Also, I made the size of the bubbles the same because the size does not communicate any message. I made the background of the chart white, as suggested. This way the graph looks prettier. I added a headline to the depiction. As suggested, I increased the initial opacity, so I changed it from 0.1 to 0.3. You can see it here: http://bl.ocks.org/KateBan/raw/497e5d6be410c5ebf495/.

### Forth attempt
After the further feedback, I added "Median" to the Y axis label to convey the message clearer. I added a commentary under the headline that the view should hover over the plot for full effect. I also tried to make the message that pops up when you move the mouse on a particular bubble more informative and clearer. There was a suggestion to increase the opacity more; I did not do that because the effect of the interaction will be lost. Also, it was suggested that I frame the bubbles with the black line; I did not do that because the visualization would not look as pretty as it is now. You can see it here: http://bl.ocks.org/KateBan/raw/0c35288198c087b735e9/

### Fift attempt 
I switched the X and the Y axis places because as mentioned in the feedback the independent variable should be on the X-axis and the dependent on the Y axis. I also added a legend to make the distinction to the colors of the wines more visible. This is the last version here: http://bl.ocks.org/KateBan/cb3cba762df638d1982c

### Sixth attempt 
Based on my first project review I changed the circles into two shapes according to the acid type - citric acid diamonds and volatile acid crosses. I made an experiment with different shapes like triangles that point upwards and downwards but the easiest to distinguish between were diamonds and crosses, so they were my last choice. Also, as it was suggested, I switched the places of the X and Y axis. I believe it conveys a clearer message to the viewer. (I collected feedback from one person here at home, and he confirmed my thoughts.) Also, I edited the labels of the Y axis to make it clearer which symbol to which acid is connected. 

##Feedback
Here is the link to the forum discussion over my visualization: https://discussions.udacity.com/t/project-6-need-feedback-for-wine-quality-visualization/45495. Also, there is another photo of additional feedback from our Slack channel you can check "Photo_3".

#### Feedback 1:
The intial opacity is a little too light
I dont know what the x axis is
and why there are two values that seem to have the same X value
what does the size of the dot represent?
Otherwise the transitions work great 
impressive you built this in plain d3
really clean code

#### Feedback 2
Something that caught my attention was that the data of citric and volatile acids seem almost mirrored. Would be interesting to see a scatterplot showing the relationship between the two measures.
Also, took me some time to understand what was the meaning of the size and color in your chart. Perhaps would be better if you included a legend.

#### Feedback 3
It was interesting to look at this visualisation, as I was doing EDA on this dataset.
I think that white background will work better and you should add legend.

#### Feedback 4
What do you notice in the visualization?
The median acetic and citric acid level for different quality red and wine wines are presented as dots.

What relationships do you notice?
For lower quality red lined the difference between acetic and citric acid levels is high. For high quality both quantities are the same.
For white wines there is no relationship between acids and quality.

What questions do you have about the data?
I wonder what is the variance of the acid levels.

Is there something you don’t understand in the graphic?
The chart is clear in general with nice interaction. I would add "Median" on the y title, otherwise if you don't interact with the graph you miss this detail. Also increasing a little bit the saturation of the bubbles will make it more readable.
Updated graph has improved. Finding a way to distinguish between the Acetic and Citric bubbles without the need of interaction will be useful (e.g one could be just contour).

#### Feedback 5
It certainly seems red wines are more affected by acid content, and are affected differently depending on the kind of acid. However, the relationship between the different variables was confusing.

If I understand the variables correctly, I think the axes should be switched. Quality would seem to be more of a dependent variable, and the acid content would be independent.
The different measurements (citric and volatile) on the same axis in the same color were confusing to me, and couldn't be determined without hovering over a few points and comparing the description that appears.

#### Feedback 6 (Feedback from my first project review)
The visualization is generally quite clear. I like the choice of colors used for each wine type in your final visualization. The manipulation of color saturation on hover is a good way of comparing acidity values between the two types of wine.

However, as suggested by a comment in Feedback 5 of your Readme file, it is a bit confusing to see two series of points for each wine type in the same symbol. The only way to distinguish between citric acid and volatile acidity is to hover over points and read the text descriptions. It should be possible to see the major trends from the plot as given, without interaction, if you set each acid type with its own symbol. You might want to look at d3.svg.symbolTypes and symbol.type to help provide this functionality; some examples of using different symbols can also be found here and here.

As an optional suggestion, it can be argued that it makes sense to put acidity on the vertical axis and quality on the horizontal axis, as given in your preliminary plots. Since the data has been aggregated by values of quality, it is more intuitive to think of binning operations as having been performed on horizontally-aligned values rather than vertically-aligned values. With the plot as given, the natural inclination is to think that we might want to bin on values of acidity and then take the average quality recorded in each bin. Either choice of axes should be fine, but they do convey different ways of thinking about and interpreting the data.

## References
The video course: Learning to Visualize Data with D3.js
Udacity materials and forum
D3 documentation
http://bl.ocks.org/ZJONSSON/3918369
http://d3-legend.susielu.com/
http://stackoverflow.com/questions/20114508/how-do-i-add-two-different-shapes-to-d3-forced-directed-graph-based-on-shape-fie
