# Gender-Likeability-IAT

### Table of Contents 
- [Introduction](#introduction)
- [Motivation](#motivation)
  - [What is the Implicit Association Test?](#what-is-the-implicit-association-test)
- [Methods](#methods)
  - [Experiment Overview](#experiment-overview)
  - [Experiment Design Considerations](#experiment-design-considerations)
  - [Experiment Design](#experiment-design)
- [Results](#results)
  - [Participant Demographics](#participant-demographics)
  - [Reaction Time Results](#reaction-time-results)
- [Discussion](#discussion)  
- [Future Directions](#future-directions)  
- [Navigating the Directory](#navigating-the-directory)

## Introduction
The Gender-Likability Implicit Association Test (IAT) is a reaction-time experiment to test for implicit gender bias in professional settings. This experiment won first place in my Big Data in the Psychological Sciences class's research competition for the topic I chose, the methodologies I implemented, and my discussion of the results’ implications and future steps. 
## Motivation
Multiple studies have revealed that women have been described in markedly different terms than men in professional settings. In a previous analysis of 81,000 performance reviews in professional work settings, the majority of the most commonly used descriptors for men were positive, while the majority of the descriptors for women were negative, with the second most frequently used descriptor for women being “inept.” (Smith, Rosenstein, & Nikolov, 2021). 

<p align="center">
  <img src="https://github.com/anke-hao/Gender-Likability-IAT/blob/main/Documentation/Performance%20Eval%20Gender%20Difference.png" style="height: 330px;"/>
</p>

Beyond the patterns found in performance reviews, women were also twice as likely to be branded bossy in the workplace, and “bossy” women were seen as less promotable compared to “bossy” men. Both studies indicate that women are more likely to be viewed in ways that would have a negative impact on their professional success. What these results do not demonstrate, however, is if this is a result of implicit bias. 

This study aims to see if there is a demonstrable implicit bias in favor of linking male-associated words with positive characteristics, and female-associated words with negative characteristics. The experiment is an Implicit Association Test that tests for implicit bias between associations of gender and positive or negative characteristics.

### What is the Implicit Association Test?
The Implicit Association Test (IAT) measures the “strength of associations between concepts (e.g. black people, gay people) and evaluations (good, bad) or stereotypes (e.g. athletic, clumsy)” (About the IAT, 2011). Participants sort stimuli into categories by pressing the corresponding key as fast as they can (usually “e” for left, “i” for right), while their reaction times are recorded. Some of these stimuli would require participants to utilize the top categories to make judgements (e.g. “White” or “Black”), while others would require them to utilize the bottom categories to make judgements (e.g. “Good” or “Bad”). 

If a participant's reaction time for one particular type of association (e.g. White/Good and Black/Bad for the Race IAT) is faster than the other possible association (e.g. Black/Good and White/Bad), the experiment will conclude that they “implicitly” prefer the association they reacted faster to, as opposed to the association they reacted slower to.
## Methods
### Experiment Overview
The study was a Psytoolkit experiment that was coded and embedded into a survey that asked preliminary questions about gender, age, and ethnicity. The Psytoolkit experiment recorded reaction times of two different conditions: 
- Linking Negative characteristics with Male-associated nouns and Positive characteristics with Female-associated nouns (NMPF).
- Linking Positive characteristics with Male-associated nouns and Negative Characteristics with Female-associated nouns (PMNF). 
Examples of the two conditions are shown below:
<p align="center">
  <img src="https://github.com/anke-hao/Gender-Likability-IAT/blob/main/Documentation/Condition%20Examples.png" style="height: 330px;"/>
</p>

### Experiment Design Considerations
In order to account for the effect of “practice” in categorizing words, the participants were randomly assigned an order in which they were tested on the two conditions, referred to as a block order. The two random block orders were PMNF first/NMPF second and NMPF first/PMNF second.

### Experiment Design
Participants each went through 7 “blocks,” or trials, with 4 blocks total in which data was collected and with 3 blocks as training. An overview of the 7 blocks is listed below:
- Block 1: 5 practice rounds for “positive” vs “negative” characteristics
- Block 2: 5 practice rounds for “MALE” vs “FEMALE” associated words
- Blocks 3 & 4: formal data collection rounds, 10 rounds each (e.g. PMNF)
- Block 5: “Positive” and “negative” get switched; 10 practice rounds
- Blocks 6 & 7: formal data collection rounds, 10 rounds each (e.g. NMPF)

Each participant experienced both the PMNF and the NMPF conditions, although the order in which they encountered the conditions were randomized. Their task was to press either the “e” or the “i” key as fast as they could in order to categorize the word they saw in the center of the screen into either the left or right side, depending on the nature of the word.

## Results
A total of 369 participants were recruited from Amazon Mechanical Turk to take part in the experiment and were each paid 30 cents for participation in a 2-3 minute experiment. 68 were excluded from final data analysis after data collection due to: 1) unfinished survey entries (n = 37), 2) incorrect answers to the attention check (n = 4) , 3) having an error rate higher than 40% in either block order or having a total error rate higher than 60% (n = 27). This resulted in a total of 301 participants for data analysis (59.5% female).

### Participant Demographics
Ethnicity | White | Asian/Pacific Islander | Black/African American | Hispanic/Latino | Mixed | Other 
--- | --- | --- | --- |--- |--- |--- 
Percentage | 74.8 | 12.6 | 7.0 | 4.0 | 0.3 | 1.3 

Age | 18-24 | 25-34 | 35-44 | 45-54 | 55-64 | 65-74 | >75 
--- | --- | --- | --- |--- |--- |--- |--- 
Percentage | 8.3 | 29.9 | 23.6 | 20.3 | 10.3 | 7.0 | 0.7

Gender | Female | Male  
--- | --- | --- 
Percentage | 59.5 | 40.5

### Reaction Time Results
There was no significant difference in average reaction times with the PMNF versus the NMPF block order, regardless of assigned block order.

Statistic | NMPF reaction time (ms) | PMNF reaction time (ms) 
--- | --- | --- 
Mean | 1065.6 | 1089.0
Median | 917.8 | 954.3
Sttdev (mean) | 521.7 | 441.2
Sttdev (median) | 327.2 | 337.7
Error rate | 6.1% | 6.6%

## Discussion
As the difference in two means was not significant, the average reaction times of the participants do not conclusively favor one condition over the other (PMNF vs NMPF). There are several factors that may contribute to this, including a high proportion of female participants, a younger demographic among the participants, a small sample size, and non-standardized testing conditions.

## Future Directions
Future experiments with the Gender-Likability IAT, beyond collecting more data, may include new ways of segmenting data, surveying other populations, and enhancing the stimuli.

## Navigating the Directory
- The full research report is located in the `Documentation` folder, and cleaned data from the experiment is located in the `Data` folder.
