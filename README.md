Summary
===========

I chose the baseball data set and created a visualization that shows differences among the performance of the baseball players. There is a positive relationship between the Number of Home Runs and Batting Average. Most players have a batting average around 0.25, if a player has a batting average below 0.20, he most likely will have a low number of home runs. Moreover, players with good batting average usually have medium heights, and players who are good at hitting home runs are usually of medium weights.

Design
===========

I chose scatter plot because plotting each player as an individual point is straightforward. Scatter plot can show trends clearly. I decided to plot multiple figures because I was interested in several relationships between the continuous variables. I chose to use different colors for three types of handedness so that the differences between these three groups can be seen. I also created interaction that can show or hide each group, which makes it easier to investigate a particular group of players.

The first figure is the relationship between home runs and batting average because I want to find out good players. The second figure is the relationship between height and batting average because I want to know whether height can affect batting average. The figure plot is the relationship between weight and home runs because I want to know whether weight can affect hitting home runs.

The feedbacks I received from my colleagues provided a few recommendations:
1. Summary statistics could be helpful, for example the player counts by handedness.
2. A regression line or loess line would be nice.
3. Some outliers in the data, for example, individuals with the height of 145 in, or both the batting average and home runs are 0.
4. Statistical analysis for testing whether handedness is significant?

My responses are:
1. I made a new histogram to show the player counts by handedness.
2. Dimplejs doesn't have the functionality to fit a regression line or loess line.
3. I removed the outliers.
4. Again, Dimplejs is not a statistical package and this project is mainly for visualization. Hypothesis testing is unnecessary for now.

After this I finished my second version of visualization.

The feedbacks I received from the Udacity tutor helped me improve my visualization further:
1. Charts are severely overplotted. It may be useful to change an opacity of points to show such a lot of them on one chart.
2. For the first chart may be useful to use log x-axis -- it will allow spreading data points more evenly and easier to make comparisons.
3. There is missing units for axes, it is unclear what exactly each axis shows. Also, it may be great to add some explanations for used terms.

I made all the suggested changes and finished my third visualization.

A second feedback from the Udacity tutor included suggestions:
1. Axis labeling a little bit confusing, I can't figure out what "Height of Players (60+ inches)" and number mean. Is it means that the reader has to do mental calc and add 60 to every tick on axis? If so, it is highly confusing and distracting.
2. Also, please provide units directly on the chart and add titles to charts.
3. The last thing, charts still look a little bit overplotted, please reduce opacity further and try to use more advanced techniques to deal with it, like adding jitter.

My responses are:
1. I changed the axes to the original numbers.
2. I added titles to the charts.
3. I reduced the opacity further. As for jitter, I couldn't figure out how to do that in Dimplejs, sorry.

So I have the fourth version of visualization.

A third feedback from the Udacity tutor included required changes:
1. I would definitely limit the x-axis ranges on the height and weight charts so that they are easier to see. For example, height only has values between approximately 60 and 80 inches. Dimple can limit these axes for you.
2. In the home runs versus batting average chart, there are a lot of values at an x-axis value of 0. Log(0) does not exist. I would either make a note somewhere on the visualization telling people that since log(0) doesn't exist, those values are just home runs.
3. The fourth chart still needs a chart title and an explanation of what it represents.

and optional changes and ideas:
4. Many people won't understand how to convert the numbers on the log() based x-axis to actual home runs. Dimple has functionality to make a log axis with myAxis.addLogAxis. So code like x.addLogAxis("x", "HR") will make a log based x-axis that will at least be somewhat easier for people to understand.
5. I highly encourage taking summary statistics and/or plotting trend lines instead of plotting all of the data points.
6. Another idea to consider is how many data points there are on the low and high end of the weight and height ranges.


My responses are:
1. I used the overrideMin and overrideMax properties to limit the X axes for height and weight, making the trends easier to see.
2. I used the x.addLogAxis("x", "HR") function to keep the x axis in the original unit yet still separate the points quite a bit. In this case I don't need to add the note for the 0 home run points.
3. I added titles and explanations to all the charts.
4. I used the aggregate method to plot a histogram comparing the mean batting averages for different handedness. I still want to keep the scatter plot therefore I did not switch to line plot.
5. I remove the comment saying "Players that are too high tend to have medium to low batting average" since there are only 5 points with height greater than 78 inches.

Thus I have the final version of my visualization.



Feedbacks
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

First Feedback from Udacity tutor
------
1. Charts are severely overplotted. It may be useful to change an opacity of points to show such a lot of them on one chart.
2. For the first chart may be useful to use log x-axis -- it will allow spreading data points more evenly and easier to make comparisons.
3. There is missing units for axes, it is unclear what exactly each axis shows. Also, it may be great to add some explanations for used terms.


Second Feedback from Udacity tutor
------
1. Axis labeling a little bit confusing, I can't figure out what "Height of Players (60+ inches)" and number mean. Is it means that the reader has to do mental calc and add 60 to every tick on axis? If so, it is highly confusing and distracting.
2. Also, please provide units directly on the chart and add titles to charts.
3. The last thing, charts still look a little bit overplotted, please reduce opacity further and try to use more advanced techniques to deal with it, like adding jitter.


Third Feedback from Udacity tutor
------
1. I would definitely limit the x-axis ranges on the height and weight charts so that they are easier to see. For example, height only has values between approximately 60 and 80 inches. Dimple can limit these axes for you.
2. In the home runs versus batting average chart, there are a lot of values at an x-axis value of 0. Log(0) does not exist. I would either make a note somewhere on the visualization telling people that since log(0) doesn't exist, those values are just home runs.
3. The fourth chart still needs a chart title and an explanation of what it represents. It might seem obvious what this chart represents, but remember that people seeing this visualization will have never seen this data set before and won't know where it comes from.
4. Many people won't understand how to convert the numbers on the log() based x-axis to actual home runs. Dimple has functionality to make a log axis with myAxis.addLogAxis. So code like x.addLogAxis("x", "HR") will make a log based x-axis that will at least be somewhat easier for people to understand.
5. I highly encourage taking summary statistics and/or plotting trend lines instead of plotting all of the data points.
6. Another idea to consider is how many data points there are on the low and high end of the weight and height ranges.



Resources
===========
https://docs.google.com/document/d/1w7KhqotVi5eoKE3I_AZHbsxdr-NmcWsLTIiZrpxWx4w/pub?embedded=true
http://alignedleft.com/tutorials/d3
http://dimplejs.org/advanced_examples_viewer.html?id=advanced_interactive_legends
https://developer.chrome.com/devtools/docs/console
https://github.com/PMSI-AlignAlytics/dimple/wiki/dimple.chart
http://chimera.labs.oreilly.com/books/1230000000345/ch04.html#_setting_up_a_web_server