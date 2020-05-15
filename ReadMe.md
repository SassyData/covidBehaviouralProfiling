
##### File contents:
0 Data folder                   2 .csv data files (responses & variable descriptions)
1 Covid Behaviour, notebook     Analysis and functions
2 ReadMe, md                    Full project writeup, structure, libraries, etc

##### Readme contents:
1. Exploring behavioural response to Covid-19
  a. Needs and affects - topic modelling
  b. Profiling survey respondents
  c. Additional survey questions
2. Further exploration 
  a. Covid-19 intricacies
  b. Project structure
  c. How to talk to people
 
##### Libraries 
numpy 
pandas 
atplotlib.pyplot 
gensim 
nltk
wordcloud
sklearn
bokeh
pyLDAvis.gensim
seaborn
kmodes.kmodes
scipy.stats



# 1. Exploring the behavioural response to Covid-19

This workbook works with survey data of 478 features, in order to explore trends from people from diverse demographics, in their response to Covid-19 and also their general preferences.

### a. Assessing the needs and effects of Covid-19 (from survey free text field, using topic modelling techniques)
This investigation uses topic modelling to extract meaning from two free text fields within the data. A range of topic models were explored, and ultimately LDA was applied.

The effect of the virus can is represented by the following three topics, which appeared most strongly in the data. This produced a coherence score of .27 and well defined clusters (without overlap) when modelled with an intertoptic map.
* Lack of freedom
* Isolation
* Money & job security

The needs that were most cited can be categorised into the following four categories. The coherence score was .37 and well defined clusters.
* Money
* Essentials (food / government help)
* Nothing / lockdown end
* Loved ones

### b. Profiling survey respondents

K-Modes clustering was used to profile respondents, given the majority of categorical data. The result of profiling identified two groups, A and B.
There are strong trends coming through, which reflect the ingrained differenced between generations; millennial (B) and baby boomers (A). Through profiling we can build a rich personas of each and bring statistical rigour to conclusions which might otherwise be dismissed as stereotypes.

##### Group A
* Tend to be older, with the most frequent age band being 55-64
* Living most often in the Midlands and North East
* Favour traditional values to liberal ones
* Take Covid 19 and its consequences, such as lockdown, the most seriously. They strongly stick to the rules and see the current situation as a clear state of emergency
* Ford is the car manufacturer of choice
* M&S and Next are the favoured High St. fashion stores..
* ..whereas Samsung and Sony are the preference in tech
* They prefer to read The Daily Mail and The Sun newspapers
* In terms of social media, they would miss Facebook the most if it were gone

##### Group B
* In contrast, tend to be younger, 25-34 was the most common age band
* Most often from London, and commonly an EU citizen
* Are more balanced in their values, appreciating both liberal and traditional
* Ford is still popular, but BMW is where its at
* Budget 'fast fashion' stores such as Primark and H&M are the preference
* ..and in tech they're more likely to stick to Apple and Samsung
* Sticking with the more liberal theme, they prefer to read The Guardian
* In terms of social media, they identify with Instagram, as well as the Facebook titan

### c. Additional survey question ideas
Given the breadth of this survey, it would be interesting to include other divisive topics:
* Brexit
* Women's rights and equal pay
* Transgener in sport
* Religion
Maybe even lighter topics such as:
* ‘Scon’ vs ‘scOne’
* Dogs or cats
* Liking of Piers Morgan

# 2. Further exploration
### a. Covid-19 intricacies
One disadvantage of the strong signal from the generational differences is that it may have suppressed any more subtle similarities we might have found between Covid-19 responses, such as ‘worriers’ versus ‘optimists’. This would be my first question to explore given more time. By removing some of these strongly divergent features, which helped to define groups A and B above, or by weighting in favour of the the Covid-19 response features, next steps would seek to uncover these more nuanced relationships. Telling us something new about how people are coping, how to communicate with them, and how to help them.

### b. Project structure
With more time, I would restructure the project into a number of notebooks: 
* Functions (specific to the project) 
* Need and effect topic modelling 
* Profiling

### c. Another use - how to talk to people
This data could provide deep insight into people in terms of wants, desires and preferences. There is an opportunity from the skew of the questions towards understanding how people could best be communicated with. Taking into account literal signposts such as where they get their news from (which paper, which channel or media) and which brands they have awareness of, but also in terms of more subtle and potentially more powerful indicators, such as what types of communication resonate, who they trust to receive information from, and whether they are “move towards” or “move away from” [types](https://coachcampus.com/coach-portfolios/power-tools/elle-wilks-moving-away-from-vs-moving-towards/). 
