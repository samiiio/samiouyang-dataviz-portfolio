| [home page](https://samiiio.github.io/samiouyang-dataviz-portfolio/) | [data viz examples](dataviz-examples) | [critique by design](critique-by-design) | [final project I](final-project-part-one) | [final project II](final-project-part-two) | [final project III](final-project-part-three) |

# Redesign HPV Vaccine Coverage Visualization

In this assignment, I'm going to critique a visualization by redesign it. I'll include my every step and insights in this page.

## Step one: the visualization

![image](https://github.com/user-attachments/assets/fb445754-c364-49f0-88c5-5bc843089ee5)
source: https://data.world/makeovermonday/coverage-of-the-hpv-vaccine 

The original visualization is showing the changes of HPV vaccince coverage over time for some countires. The reason I choose this visualization is because I actually think this visualilzation is very straightforward to understand, and efficient to convey information. But the design is not beautiful enough, the audience may lost interest or do not want to spend time reading it. So even though I know it would be challenging to make the visualization convey information more efficiently than the orginal one, I would still like to see if I can make this visualization looks better. 

## Step two: the critique

There are few areas of possible improvements for this visualization:
- the whole visualization looks boring, it lacks of color differentiation. Although the it's not necessary in this case to use multiple colors, but I think we can use colors to make the visualization look better.
- the background and y-axis and x-axis labels are too light and subtle, making it difficult for audience to know the exact values.
- there are not labels or numbers of lines, so it would be hard for audience to learn the exact coverge rates.
- there's no sequence or order of all the countries, so it is hard to compare the total 12 countries' coverage on HPV vaccine.
- there are some missing labels (years) on x-axis. 

## Step three: Sketch a solution
I have done 4 sketches overall. I have documented my thoughts when I did each sketch, and also why I think the sketch not works well.

#### Sketch 1
![image](https://github.com/user-attachments/assets/ad302832-ca75-41a7-a648-1c3ce9dd3cc2)

The reason I choose the heatmap is it can shows the vaccine coverage of each year in our selected countries. Since I did not find heatmap in Tableau, so for this sketch I used python to do that. It is hard for audience to read the exact rates from the orignal visualization, but in this heatmap, everything is straightforward. Audiences could learn information without effort. But it seems like that's too much information, and the visualization looks busy, so we will keep working here. 

#### Sketch 2
![Sheet 2](https://github.com/user-attachments/assets/fe2fcfe4-6d2e-499f-a8f8-67b12e0b850b)
Then I think it might be useful to use a treemap, and it turns out treemap is pretty good for showing the ranking on some leve, because the bigger the size of rectangle, and higher vaccine coverage in the country. So audience could simply read the coverage rate and learn the ranking of countries. But the point is, treemap is simple and elegant, it will let us miss the changes over year, one of the important information.

#### Sketch 3
![Sheet 1](https://github.com/user-attachments/assets/84656f84-eecf-44c9-8d32-222d242b75fe)
This is the previous final visualization I got. The reason I choose stacked area chart is:
- It can shows the upward trend of HPV vaccine coverage of different countries over time. While in the original visualization, it is not that obvious to see the overall upward trends of vaccine coverage.
- It can shows the ranking of vaccine coverage conditions of selected countries, therefore it would be easier for audiences to compare that which country doing a better job in HPV vaccine coverage.
But after talking to our TA, I realize this is not a good choice. SO I started to redesign the graph again.

#### Sketch 4
![new_hpv_sketch](https://github.com/user-attachments/assets/b64d950c-7cd4-4dee-b0bf-de6fd3064c43)
Then I narrowed down the slected countries, to focus on the HPV vaccine coverage by continents, instead of random slected countires in the original visualization. Because I think this selection could make more sense for the whole story. By using the stacked bar chart, we can clearly see that which continent has a comparately high vaccine coverage, and their changes from 2010 to 2022. But I think it still takes some time for audience to match the color and countinent names. 

## Step four: Test the solution

*ps. last two graphs were not created when I did the interview. So the results are only for heatmap and treemap sketches.

Results: 

| Question | Interview 1 | Interview 2 |
|----------|-------------|-------------|
| describe to me what this is telling you?| A visualization showing HPV vaccine condition of different countires  | HPV vaccine coverage condition worldwild |
|Which sketch do you prefer?|    Treemap       |     Heatmap        |
|  Is there anything you would change? |      Might change a chart type but cannot come up with any right now       |  Colorplatte of heatmap           |

Synthesis: 

It seems like both interviewees think I can choose a better color platte for no matter which sketch. And both of them think there might be a place to change the chart type, but we did not come up with any. I might try to change a chart type later.

## Step five: build the solution

<div class='tableauPlaceholder' id='viz1739400261998' style='position: relative'><noscript><a href='#'><img alt='HPV Vaccine Coverage Over Time By Continents (2010-2022)* Five Continents with Sub-Saharan Africa area and Australia, Antarcia not included* ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;HP&#47;HPV_Vaccine_Coverage_Overtime_Continents&#47;Sheet3&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='HPV_Vaccine_Coverage_Overtime_Continents&#47;Sheet3' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;HP&#47;HPV_Vaccine_Coverage_Overtime_Continents&#47;Sheet3&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /><param name='filter' value='publish=yes' /></object></div>                
<script type='text/javascript'>                    
  var divElement = document.getElementById('viz1739400261998');                    
  var vizElement = divElement.getElementsByTagName('object')[0];                    
  vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    
  var scriptElement = document.createElement('script');                    
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    
  vizElement.parentNode.insertBefore(scriptElement, vizElement);                
</script>


![Sheet 3](https://github.com/user-attachments/assets/f46de5a0-33e9-40dc-99e9-2579c91d8b00)
*For some reason, the embeded code could not shoe the complete visualization, so I pasted a image here.

My final visualization is a combined bar charts. I re-select the entities (countries) of the visualization. I select the data of continents, so the visualization is trying to show the HPV vaccine coverage over time by continents, which would be a better story than just selected random countires, which is meaningless to compare. And through the new design, audience can first easily see the changes and exact coverage rate number in each continent over time. They can also easily compare the coverage rates between each continent. Also, I used different colors to represent different continents, although it's not necessary in this case, but I have tried using the same color for bar charts and figured out since those bar charts are so close, it would be a little bit hard to distinguish. So I finally decided to use different colors representing continents. 

So overall, the benefits of my new redesign would be:
- A better and make more sense story, by showing HPV coverage by continents, which could let audience see the HPV vaccine condition all over the world.
- audience can know the exact numbers of vaccine coverage rates, so they could not only see the trends by bars and numbers, but also easily comapre the conditions all over the world.
- Also because we are using Gantt bar charts, audience can easily compare the HPV vaccine coverage rates by the length of bars and the numbers.

## References
Data.World. (n.d.). Coverage of the HPV vaccine. Retrieved February 12, 2025, from https://data.world/makeovermonday/coverage-of-the-hpv-vaccine

## AI acknowledgements
N/A

