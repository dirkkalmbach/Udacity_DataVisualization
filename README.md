# Summary
*Population pyramids are widely used visualizations of demographic variables. They provide a compact view of how a population is composed and how it changes according to other variables (e.g. over time).
I used age pyramids to show the demographic structure of the 1st, 2nd and 3rd passenger classes of the Titanic and how they differ according to death-rate. The reader can see that passengers of the poor classes (2nd and 3rd) had a lower chance to survive the tragedy and that in addition, the death-rate of minorities (women, children, elderly) differ between passenger classes. As this is an often ocurring social phenomena and sometimes named as "the two sides of social inequality", I let it open to the reader to generalize this finding to present-day social phenomena.*

# Design

The goal is to show how the death-rate (chance not to survive) changes between sociodemographic groups and subgroups. 

I used a population pyramid as this is a widely used diagram in Germany. Population pyramids show the age distribution divided by male and female and are normally used to show the age structure of the society, and how it changes over time *("Ageing society" is a big topic in Europe)*. The horizontal bars show the number of victims. With the help of stack bars I added another variable: the total number of passengers. This quickly allows the reader to identify the death-rate for different age-groups. 

I designed three diagrams. The reader could swith between them by clicking a button. I positioned the buttons directly at the top of the diagram, so that the reader will see it directly *(Often interactive elements are in the corner and people hardly recognize them.)*.

To communicate the main message, I used a double encoding:

1. the diagram itself which changes on button click

2. statistics showing the death-rates for all the subgroups. This numbers and font size changes according to the size of the numbers on button click. *(So, actually a triple encoding.)*

A smooth transition rate was implemented to give the reader the time to identify the change.

A conclusion at the buttom of the page summarizes the main message again. It appears only after clicking on the 3rd class-button - making sure that she saw at least the 1st and the 3rd class.

## Visual encodings
I used colors to differentiate between male (blue) and female (red). As this was one of my main messages, and did not want to distract the reader with other colors, I therefore only used black and grey colors for text and background image. Additionally, the use of colors would have been impious.

So rather than chosing another color to visualize the total passengers in the stacked bars, I used hue, respectively a more transparent red and blue version.

A background image showing the sinking ship helps the reader to quickly interpret what this graphic is about. Another aim of the background image was to communicate emotional aspects of the tragedy. *In my opinion, pure diagrams are too rational and not approbriate to communicate bad findings.* However, a high transparency rate was chosen to avoid distraction.
 
## Other design decisions

At the beginning I did not implemented axis labels. I thought that population trees are easy to interpret. However, as this was criticized during the survey, I added them.  

I also added a legend as some interviewees did not intuitivley understand the total-passenger-bar.

The first draft contained a table for the statistics. During the main survey I recognized that these figures were mostly ignored by the reader (according to font-size and its statistical appearance.) As a result, I changed them to text (explained above).

I also corrected some style issues with the background image which was mentioned by one interviewee, added an conclusion at the end to provoke further thinking (*I would let it open to the reader if he wants to generalize the main message or not.*), and changed the heading from the first version and decided to use this to communicate the main message. _Rather than the neutral heading **Victims of the Titanic**, the title now is **The poorest among the poorest are the real victims**._

The lack of the word Titanic in the title and experiences from the survey let me change the description of the passenger classes.

Finally, I changed the button design.

# Feedback
## Pre-Survey
I began with building population trees with excel *("quick-and-dirty-approach")* with the aim to proof whether this kind of visualization is understandbable. I was not sure if the reader knows the concept of age pyramids (although it is a widely used diagram type in Germany). To eliminate education bias, I asked people without college degree. The following Table shows the results:


| No   | Age | Sex | Education                 | *What do you see here?* | 
| :--: |:---:| :--:| :-------------:| :--:| :--:|
| 1    | 74  | m   | lower secundary education | *I'm not sure, but it looks like an age pyramid. (..) Red is for women and blue is men? What's the light color for?* | 
| 2    | 61  | f   | lower secundary education | *I don't know. (..) The left scale is age (..) It shows age classes for men and women -  A What is 1st class?* | 
| 3    | 17  | m   | high school | *I know this from school. It's an age pyramid. Red is woman, blue is man? You know that normaly man are left and woman are on the right.*| 



I concluded that people are able to identify the age structure. The y-axis should be mirrored (with male on the left and female on the right as this seems to be standard). Victims and survivors should be double coded (e.g. with additional pie charts). One interviewee argued that people in the past were not gettting as old as today and that I should cut the y-axis at the top. *(I therefore changed the last category from 75+ to 70+.)*
 
## Survey

I used a family reunion to ask my parents, my brother, his wife, and my uncle for feedback on how they interpret the visulization according to the questions provided in the project rubric. I developed a german version of the visualization as well and showed it to the interviewees locally on my labtop. 

Most interviewees correctly identified the diagram as an age pyramid (although only 2 knew the name of this diagram type). One interviewee answered that he does not know what the graphic is about as labels for the axis are missing. 
Some also argued they are missing a legend. Almost one half of the interviewees interpreted the bold red and blue bars as victims of the titanic (according to the title) and light bars as total passengers (with some uncertainty, e.g. *"Do the light bars stand for all passengers?"*). The other half wasn't sure and answered *"I don't know!"* on my request what they think the bars stand for.  

Everybody (except of two) identified the buttons as clickable and did so (In the beginning, I introduced the visualization as interactive and motivated them to use the trackpad and interact with the diagram). Two persons *(older, no computer natives)* used the buttons only after I showed it them. 

Some had problems understanding intuitively that "1st, 2nd, 3rd class" stands for passenger class. 

The table on the right with the death-rate statistics was mostly ignored. Some interviewees did not even recognize that the figures are changing on button click. 

Everybody interpreted the main message that the death-rate increases according to passenger class. Most people also understood that the survival (or death) rate changes between the subgroups. Some explicitely mentioned that. (One interviewee: *"Oh see, every second woman in 3rd class died. But in 1st class only one or two."*)

The lack of axis labels was mentioned explicitely by one interviewee.

# Resources

[1] [How to build Age Pyramids in Excel](http://www.stallwanger.net/wordpress/excel-beispiel-alterspyramide-erstellen-personalcontrolling/) (in german)

[2] [Stack Overflow: Creating Population Pyramid with D3.js](http://stackoverflow.com/questions/25044997/creating-population-pyramid-with-d3-js)

[3] [Design modules for css](http://purecss.io)

[4] Murray, Scott. Interactive Data Visualization for the Web, O'Reilly, 2013
