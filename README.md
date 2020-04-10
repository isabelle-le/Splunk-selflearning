Date: 14/03/2020 

# Objective: 
You want to learn a new bigdata tool for free? Welcome on board!

## Getting started:
Splunk is not an open source but you can enjoy 60 days trial with entrepise version or 30 days with Spunk cloud. So far as I know, Splunk elearning costs $2000/ 1 course. I am a student and eager for adventure travels. I wouls rather spend $2000 for travelling, at the mean time,I will try to learn splunk myself. 

## Stage 1: learn a new bigdata tool Splunk with pratice (at least 1 new topic/ day)

## Stage 2: analyse covid19 data via Splunk 
I am at Yvelines with at least 70 known positive cases in my area. I am still negative to covid-19, but, I am isolated to the outside community. In order to kill my freetime, I am learning Splunk(work required) instead of outdoor activities as normal saturday/sunday time

Dashboard is avaiable with log in username=User and pw=$plunkEntr3prise
http://localhost:8000/en-US/app/search/coronavirus_v1?form.time.earliest=0&form.time.latest=


## Stage 3: record visual learning material(video on youtube) to help others. 
           
# Why Splunk? 
Beside the job requirement, Splunk is a big data tool which is good for anykinds of data. The basic processing components are like any other big data tool. Which are:
1. Indexer : its input is raw data (log file, IoT..), storage as events(think of event as row in your struture database). The output is index under directory by time frame(think as table in your structure database). 
2. Search Head: you will use SPL commands to search and visualize your data. At the high level, SPL have 7 types, which are
streaming, non-streaming, orchestrating, dataset processing, generating, transforming and custom commands.
3. Forwarder:  In the real application, you will use forwarder to comsume data and forward them in Indexer (Like AWS Kinesis )

# How:
## Step 1: Splunk Fundamentals 1 - FREE - Splunk User Cert
As I mentioned above, Splunk is not an open source tool and its course is expensive(yes, it is. Splunk CEO, it is your job to make e-learning course avaiable as 20% of your current price). However, there is one beginner course you should take which is ![Splunk Fundamentals 1 Free - link](https://www.splunk.com/en_us/training.html). 

           Price: Free
           How long will it take? 2 days for me with all quizz and lab pratices and final exam to have a cert.
           What for? If you finished this course + pay less then $150 and pass exam. You will have Splunk User Cert

Advance: If you have a AWS account and familiar with EC2 instances. You can install Splunk Entreprise to your EC2 instance. 
[Command line is avaiable here](https://github.com/isabelle-le/Splunk-selflearning/blob/master/Install%20Splunk%20Entreprise%20on%20EC2.md)

## Step 2: Splunk Fundamentals 2. 
Based on its PDF material, I will do self learning and continue posting my learning progress and lab practices.

![PDF material is avaiable here](https://github.com/isabelle-le/Splunk-selflearning/blob/master/Splunk%206.X%20Fundamentals%20Part%202%20(eLearning)%20.pdf)

           [2. Beyond saerch fundamentals](https://github.com/isabelle-le/Splunk-selflearning/blob/master/2.%20Beyond%20search%20fundamentals.md)

           3. Using transforming commands for visualizations

           4. Using trendlines, mapping and single value commands

           5. Filtering & Formating results

           6. Correlating Events

           7. Introduction to Knowledges objects

           8. Creating and Managing Fields

           9. Creating Field Aliases and Calculated Fields

           10. Creating Tags and Event Types

           11. Creating and Using Macros

           12. Creating and Using Workflow Actions

           13. Creating Data Models

# Step 3: Splunk Fundamentals 3. 

PDF document is not avaiable, thus, learning document based on their course overview

![Course Topics](https://github.com/isabelle-le/Splunk-selflearning/blob/master/Fundamentals3-Description.pdf)

           14. Statistical Commands

           15. eval Commands

           16. Lookups

           17. Alert Actions

           18. Advanced Field Creation and Management 

           19. Working with Self-Describing Data and Files 

           20. Advanced Macros

           21. Using Acceleration Options


