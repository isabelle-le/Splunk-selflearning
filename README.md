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
## Splunk Fundamentals 1 - FREE - Splunk User Cert
As I mentioned above, Splunk is not an open source tool and its course is expensive(yes, it is. Splunk CEO, it is your job to make e-learning course avaiable as 20% of your current price). However, there is one beginner course you should take which is ![Splunk Fundamentals 1 Free - link](https://www.splunk.com/en_us/training.html). 

           Price: Free
           How long will it take? 2 days for me with all quizz and lab pratices and final exam to have a cert.
           What for? If you finished this course + pay less then $150 and pass exam. You will have Splunk User Cert

Advance: If you have a AWS account and familiar with EC2 instances. You can install Splunk Entreprise to your EC2 instance. 
[Command line is avaiable here](https://github.com/isabelle-le/Splunk-selflearning/blob/master/Install%20Splunk%20Entreprise%20on%20EC2.md)

## Splunk Fundamentals 2. 
Based on its PDF material, I will do self learning and continue posting my learning progress and lab practices.[PDF material is avaiable here](https://github.com/isabelle-le/Splunk-selflearning/blob/master/Splunk%206.X%20Fundamentals%20Part%202%20(eLearning)%20.pdf)

[2. Beyond saerch fundamentals](https://github.com/isabelle-le/Splunk-selflearning/blob/master/2.%20Beyond%20search%20fundamentals.md)

[3. Using transforming commands for visualizations](https://github.com/isabelle-le/Splunk-selflearning/blob/master/3.%20Using%20transforming%20commands%20for%20visualizations.md)

[4. Using trendlines, mapping and single value commands](https://github.com/isabelle-le/Splunk-selflearning/blob/master/4.%20Using%20trendlines%2C%20mapping%20and%20Single%20value%20commands.md)

[5. Filtering & Formating results](https://github.com/isabelle-le/Splunk-selflearning/blob/master/5.%20Filtering%20and%20format%20result.md)

[6. Correlating Events](https://github.com/isabelle-le/Splunk-selflearning/blob/master/6.%20Correlating%20Events.md)

[7. Introduction to Knowledges objects](https://github.com/isabelle-le/Splunk-selflearning/blob/master/7.%20Introduction%20to%20Knowledges%20objects.md)

[8. Creating and Managing Fields](https://github.com/isabelle-le/Splunk-selflearning/blob/master/8.%20Create%20and%20manage%20field.md)

[9. Creating Field Aliases and Calculated Fields](https://github.com/isabelle-le/Splunk-selflearning/blob/master/9.%20Creating%20Field%20Aliases%20and%20Calculated%20Fields.md)

[10. Creating Tags and Event Types](https://github.com/isabelle-le/Splunk-selflearning/blob/master/10.%20Working%20with%20tags%20and%20even%20types.md)

[11. Creating and Using Macros](https://github.com/isabelle-le/Splunk-selflearning/blob/master/11.%20Creating%20and%20Using%20Macros.md)

[12. Creating and Using Workflow Actions](https://github.com/isabelle-le/Splunk-selflearning/blob/master/12.Creating%20and%20Using%20Workflow%20Actions.md)

[13. Creating Data Models](https://github.com/isabelle-le/Splunk-selflearning/blob/master/13.Create%20Data%20Models.md)

## Splunk Fundamentals 3. 

PDF document is not avaiable, thus, learning document based on their course overview

[Course Topics](https://github.com/isabelle-le/Splunk-selflearning/blob/master/Fundamentals3-Description.pdf)

[14. Statistical Commands](https://github.com/isabelle-le/Splunk-selflearning/blob/master/14%2615%20Statistical%20%26%20eval%20commands.md)

[15. eval Commands]()

[16. Lookups](https://github.com/isabelle-le/Splunk-selflearning/blob/master/16.Exploring%20Lookups.md)

[17. Alert Actions](https://github.com/isabelle-le/Splunk-selflearning/blob/master/17.%20Exploring%20Alerts.md)

[18. Advanced Field Creation and Management ](https://github.com/isabelle-le/Splunk-selflearning/blob/master/18.%20Advanced%20Field%20Creation%20and%20Management.md)

[19. Working with Self-Describing Data and Files ](https://github.com/isabelle-le/Splunk-selflearning/blob/master/19.%20Working%20with%20Self-Describing%20Data%20and%20Files.md)

[20. Advanced Macros](https://github.com/isabelle-le/Splunk-selflearning/blob/master/20.%20Using%20Acceleration%20Options:%20Reports%20and%20Summary%20Indexing.md)

[21. Using Acceleration Options](https://github.com/isabelle-le/Splunk-selflearning/blob/master/21.Using%20Acceleration%20Options:%20Data%20Models%20and%20tsidx%20Files.md)

## Advanced Searching and Reporting
[Course Topics](https://github.com/isabelle-le/Splunk-selflearning/blob/master/AdvancedSearchingReporting72Description.pdf)

[22. Using Search Efficiently + More Search Tuning](https://github.com/isabelle-le/Splunk-selflearning/blob/master/22.%20Using%20Search%20Efficiently%20+%20More%20Search%20Tuning.md)

[23. Manipulating and Filtering Data](https://github.com/isabelle-le/Splunk-selflearning/blob/master/23.%20Manipulating%20and%20Filtering%20Data.md)

[24. Working with Multivalue Fields](https://github.com/isabelle-le/Splunk-selflearning/blob/master/24.%20Working%20with%20Multivalue%20Fields.md)

[25. Using Advanced Transactions](https://github.com/isabelle-le/Splunk-selflearning/blob/master/25.%20Using%20Advanced%20Transactions.md)

[26. Working with Time](https://www.hurricanelabs.com/splunk-tutorials/how-to-set-custom-time-range-presets-in-splunk)

[27. Combining Searches](https://github.com/isabelle-le/Splunk-selflearning/blob/master/27.%20Combining%20Searches.md)

[28. Using Subsearches](https://github.com/isabelle-le/Splunk-selflearning/blob/master/28.%20Using%20Subsearches.md)

29. Some Extra Tips

## Analytics and Data Science
[Course Topics](https://github.com/isabelle-le/Splunk-selflearning/blob/master/Splunk%207.0%20for%20Analytics%20%26%20Data%20Science%20MLTK%203.0%20Description.pdf)
## Advanced Dashboards and Visualizations
[Course Topics](https://github.com/isabelle-le/Splunk-selflearning/blob/master/Splunk7.3AdvDashAndViz_CourseDescription.pdf)
