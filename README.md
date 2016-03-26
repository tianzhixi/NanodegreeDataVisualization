Summary
===========

I chose the baseball data set and created a visualization that shows differences among the performance of the baseball players. We can see that the handedness does not affect the performance of baseball players very much. Height has no effect on batting average as well as weight does not influence the number of home runs.

Design
===========

I chose scatter plot because plotting each player as an individual point is straightforward. Scatter plot can show trends clearly. I decided to plot multiple figures because I was interested in several relationships between the continuous variables. I chose to use different colors for three types of handedness so that the differences between these three groups can be seen. I also created interaction that can show or hide each group, which makes it easier to investigate a particular group of players.

The first figure is the relationship between home runs and batting average because I want to find out good players. The second figure is the relationship between height and batting average because I want to know whether height can affect batting average. The figure plot is the relationship between weight and home runs because I want to know whether weight can affect home runs since heavy people usually run slower.

The feedbacks I received provided a few recommendations:
1. Summary statistics could be helpful, for example the player counts by handedness.
2. A regression line or loess line would be nice.
3. Some outliers in the data, for example, individuals with the height of 145 in, or the batting average is 0.
4. Statistical analysis for testing whether handedness is significant?

My response are:
1. I made a new histogram to show the player counts by handedness.
2. Dimplejs doesn't have the functionality to fit a regression line or loess line.
3. Although some outliers don't make sense, since I don't know much about the data, I decided to keep the outliers for now.
4. Again, Dimplejs is not a statistical package and this project is mainly for visualization. Hypothese testing is unnecessary for now.


Feedback
===========

Feedback 1
------
1. What do you notice in the visualization?
It is very readable (it's easy to see what is going on) and the interactive nature of the plot makes it interesting.
2. What questions do you have about the data?
I'm interested in the summary statistics (player count by handedness)
3. What relationships do you notice?
It seems like left handers have a slight advantage batting average and homeruns.
4. What do you think is the main takeaway from this visualization?
The above relationship as well as where most players are clumped.
5. Is there something you don't understand in the graphic?
No.

Feedback 2
------
1. What do you notice in the visualization?
Very straightforward and easy to understand description of the graphs. However, it is difficult to discern differences without some sort of visual summary, like a loess line. To see similarities, on the other hand, we'd like the points not to lie on top of each other. It is useful that they can be layered interactively.
2. What questions do you have about the data?
Were the data collected over several seasons or just one? If several seasons, what years? How were the data collected? Is this a random sample?
3. What relationships do you notice?
I notice similar shapes among the three groups. Are ambidextrous players shorter than those who prefer to use a single hand? Do lefties have a higher batting average? I think the answers to these questions might be yes, based on the graphs.
4. What do you think is the main takeaway from this visualization?
That statistical analysis should accompany the graphics that give rise to these questions.
5. Is there something you don't understand in the graphic?
Why does the horizontal scale change in the graphs when I click to remove a group?

Feedback 3
------
1. What do you notice in the visualization?
Comparing two groups was a little hard. It would have been a little easier had they been side by side graphs for me.makes it interesting.
2. What questions do you have about the data?
There are some clear erroneous points, such as the individual with the height of 145 in.... over 10ft tall. Why are they still in there?
3. What relationships do you notice?
The best batting average for home runs peaks out at a little over .25. Having a better batting average is not better, possibly because you aren't swinging for the fences taking more controlled swings.
4. What do you think is the main takeaway from this visualization?
Handedness does not affect stats that much.
5. Is there something you don't understand in the graphic?
What does it mean to have a batting average of 0? There were a few individuals with this recorded.




Resources
===========
https://docs.google.com/document/d/1w7KhqotVi5eoKE3I_AZHbsxdr-NmcWsLTIiZrpxWx4w/pub?embedded=true
http://alignedleft.com/tutorials/d3
http://dimplejs.org/advanced_examples_viewer.html?id=advanced_interactive_legends
https://developer.chrome.com/devtools/docs/console
https://github.com/PMSI-AlignAlytics/dimple/wiki/dimple.chart
http://chimera.labs.oreilly.com/books/1230000000345/ch04.html#_setting_up_a_web_server