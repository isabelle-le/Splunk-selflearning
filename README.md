Date: 14/03/2020 

# Objective: 
You want to learn a new bigdata tool for free? Welcome on board!

## Getting started:
Splunk is not an open source but you can enjoy 60 days trial with entrepise version or 30 days with Spunk cloud. So far as I know, Splunk elearning costs $2000/ 1 course. I am a student and eager for adventure travels. I wouls rather spend $2000 for travelling, at the mean time,I will try to learn splunk myself. 

## Stage 1: learn a new bigdata tool Splunk with pratice (at least 1 new topic/ day)

## Stage 2: analyse covid19 data via Splunk 
I am at Yvelines with at least 70 known positive cases in my area. I am still negative to covid-19, but, I am isolated to the outside community. In order to kill my freetime, I am learning Splunk(work required) instead of outdoor activities as normal saturday/sunday time

[Dashboard](http://127.0.0.1:8000/en-US/app/search/coronavirus_v1?form.maille_nom=France) is avaiable until May.05 with log in username=User and pw=$plunkEntr3prise
           
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

           § Search fundamentals review
           § Case sensitivity
           § Using the job inspector to view search performance

[3. Using transforming commands for visualizations](https://github.com/isabelle-le/Splunk-selflearning/blob/master/3.%20Using%20transforming%20commands%20for%20visualizations.md)

           § Explore data structure requirements
           § Explore visualization types
           § Create and format charts and timecharts

[4. Using trendlines, mapping and single value commands](https://github.com/isabelle-le/Splunk-selflearning/blob/master/4.%20Using%20trendlines%2C%20mapping%20and%20Single%20value%20commands.md)

           § The iplocation command 
           § The geostats command 
           § The geom command
           § The addtotals command

[5. Filtering & Formating results](https://github.com/isabelle-le/Splunk-selflearning/blob/master/5.%20Filtering%20and%20format%20result.md)

           § The eval command
           § Using the search and where commands to filter results 
           § The filnull command

[6. Correlating Events](https://github.com/isabelle-le/Splunk-selflearning/blob/master/6.%20Correlating%20Events.md)

           § Identify transactions
           § Group events using fields
           § Group events using fields and time
           § Search with transactions
           § Report on transactions
           § Determine when to use transactions vs. stats

[7. Introduction to Knowledges objects](https://github.com/isabelle-le/Splunk-selflearning/blob/master/7.%20Introduction%20to%20Knowledges%20objects.md)

           § Identify naming conventions 
           § Review permissions
           § Manage knowledge objects

[8. Creating and Managing Fields](https://github.com/isabelle-le/Splunk-selflearning/blob/master/8.%20Create%20and%20manage%20field.md)

           § Perform regex field extractions using the Field Extractor (FX) 
           § Perform delimiter field extractions using the FX

[9. Creating Field Aliases and Calculated Fields](https://github.com/isabelle-le/Splunk-selflearning/blob/master/9.%20Creating%20Field%20Aliases%20and%20Calculated%20Fields.md)

           § Describe, create, and use field aliases
           § Describe, create and use calculated fields

[10. Creating Tags and Event Types](https://github.com/isabelle-le/Splunk-selflearning/blob/master/10.%20Working%20with%20tags%20and%20even%20types.md)

           § Create and use tags
           § Describe event types and their uses 
           § Create an event type

[11. Creating and Using Macros](https://github.com/isabelle-le/Splunk-selflearning/blob/master/11.%20Creating%20and%20Using%20Macros.md)

           § Describe macros
           § Create and use a basic macro
           § Define arguments and variables for a macro 
           § Add and use arguments with a macro

[12. Creating and Using Workflow Actions](https://github.com/isabelle-le/Splunk-selflearning/blob/master/12.Creating%20and%20Using%20Workflow%20Actions.md)

           § Describe the function of GET, POST, and Search workflow actions
           § Create a GET workflow action
           § Create a POST workflow action 
           § Create a Search workflow action

[13. Creating Data Models](https://github.com/isabelle-le/Splunk-selflearning/blob/master/13.Create%20Data%20Models.md)

           § Describe the relationship between data models and pivot 
           § Identify data model attributes
           § Create a data model
           § Use a data model in pivot

## Splunk Fundamentals 3. 

PDF document is not avaiable, thus, learning document based on their course overview

[Course Topics](https://github.com/isabelle-le/Splunk-selflearning/blob/master/Fundamentals3-Description.pdf)

[14. Statistical Commands](https://github.com/isabelle-le/Splunk-selflearning/blob/master/14%2615%20Statistical%20%26%20eval%20commands.md)

           § Performing statistical analysis with functions of the stat command
           § Using fieldsummary
           § Using appendpipe
           § Using eventstats
           § Using streamstats

[15. eval Commands](https://github.com/isabelle-le/Splunk-selflearning/blob/master/5.%20Filtering%20and%20format%20result.md)
           
           § Using conversion functions
           § Using data and time functions
           § Using string functions
           § Using comparison and conditional functions 
           § Using informational functions
           § Using statistical functions
           § Using mathematical functions
           § Using cryptographic functions

[16. Lookups](https://github.com/isabelle-le/Splunk-selflearning/blob/master/16.Exploring%20Lookups.md)

           § Including and excluding events based on lookup values
           § Using KV Store lookups
           § Using external lookups
           § Using geospatial lookups
           § Using database lookups
           § Understanding best practices for lookups

[17. Alert Actions](https://github.com/isabelle-le/Splunk-selflearning/blob/master/17.%20Exploring%20Alerts.md)

           § Referencing lookups in alerts
           § Outputting alert results to a lookup
           § Logging and indexing searchable alert events 
           § Using a webhook alert action

[18. Advanced Field Creation and Management ](https://github.com/isabelle-le/Splunk-selflearning/blob/master/18.%20Advanced%20Field%20Creation%20and%20Management.md)

           § Using regex
           § Using the erex command
           § Using the rex command
           § Identifying regex best practices

[19. Working with Self-Describing Data and Files ](https://github.com/isabelle-le/Splunk-selflearning/blob/master/19.%20Working%20with%20Self-Describing%20Data%20and%20Files.md)

           § Using the spath command
           § Using the eval command with the spath function
           § Extracting fields from table-formatted events with multikv
[20. Advanced Macros](https://github.com/isabelle-le/Splunk-selflearning/blob/master/20.%20Using%20Acceleration%20Options:%20Reports%20and%20Summary%20Indexing.md)

           § Using nested search macros
           § Previewing search macros before executing 
           § Using tags and event types in search macros

[21. Using Acceleration Options](https://github.com/isabelle-le/Splunk-selflearning/blob/master/21.Using%20Acceleration%20Options:%20Data%20Models%20and%20tsidx%20Files.md)

           § Using report acceleration 
           § Using summary indexing
           § Exploring data models using the datamodel command
           § Using data model acceleration
           § Working with tsidx files using the tstats command

## Advanced Searching and Reporting
[Course Topics](https://github.com/isabelle-le/Splunk-selflearning/blob/master/AdvancedSearchingReporting72Description.pdf)

[22. Using Search Efficiently + More Search Tuning](https://github.com/isabelle-le/Splunk-selflearning/blob/master/22.%20Using%20Search%20Efficiently%20+%20More%20Search%20Tuning.md)

           § Review search architecture
           § Understand how the components of a bucket (.tsidx and journal.gz files) are used
           § How bloom filters are used to improve search speed
           § Describe the parts of a search string
           § Understand the use of centralized vs. distributable commands
           § Create better searches
           § Understand how segmenters are used in Splunk
           § Use lispy to reduce the number of events read from disk

[23. Manipulating and Filtering Data](https://github.com/isabelle-le/Splunk-selflearning/blob/master/23.%20Manipulating%20and%20Filtering%20Data.md)

           § Divide search results into different groups, based on values in a specified field, using the bin command
           § Regroup fields of search results using untable and xyseries
           § Create a template for performing additional processing on a set of related fields using foreach

[24. Working with Multivalue Fields](https://github.com/isabelle-le/Splunk-selflearning/blob/master/24.%20Working%20with%20Multivalue%20Fields.md)

           § Use multivalue eval functions to analyze and format data
           § Use the makemv command to convert a single value into a multivalue field
           § Use the mvexpand command to create separate events for each value in a multivalue field

[25. Using Advanced Transactions](https://github.com/isabelle-le/Splunk-selflearning/blob/master/25.%20Using%20Advanced%20Transactions.md)
           
           § Find events logged before or after a particular event occurs
           § Compare complete vs. incomplete transactions
           § Analyze transactions

[26. Working with Time](https://www.hurricanelabs.com/splunk-tutorials/how-to-set-custom-time-range-presets-in-splunk)

           § Use time modifiers
           § Search for events using custom time ranges and time windows 
           § Display and use using relative dates

[27. Combining Searches](https://github.com/isabelle-le/Splunk-selflearning/blob/master/27.%20Combining%20Searches.md)
           
           § Use the append and appendcols commands (and know the differences)
           § Use join and union (and when not to use them)

[28. Using Subsearches](https://github.com/isabelle-le/Splunk-selflearning/blob/master/28.%20Using%20Subsearches.md)

           § Use subsearches to provide filtering and other information to a main search
           § Know when NOT to use subsearches 
           § Troubleshoot subsearches

29. Some Extra Tips

## Creating dashboad with Splunk
[Course Topic](https://github.com/isabelle-le/Splunk-selflearning/blob/master/CreatingDashboards72_CourseDescription.pdf)

[30. Creating a Prototype](https://github.com/isabelle-le/Splunk-selflearning/blob/master/30.%20Creating%20a%20Prototype.md)

           § Define simple syntax for views
           § Use best practices for creating views 
           § Identify transforming commands
           § Troubleshoot views
           
[31. Using Forms (Token)](https://github.com/isabelle-le/Splunk-selflearning/blob/master/31.%20Using%20Forms.md)

           § Explain how tokens work
           § Use tokens with form inputs 
           § Create cascading inputs
           § Define types of token filters
[add timepicker to dashboard and use css to turn off default rendering] (https://www.youtube.com/watch?v=kilsJYpGWAE&list=PLSr58-DJdRyYs9AdSpi7T6N9F22CpnYZg&index=2)

[32. Improving Performance (global searches)](https://github.com/isabelle-le/Splunk-selflearning/blob/master/32.%20Improving%20Performance.md)

           § Identify ways to improve dashboard performance 
           § Accelerate data models
           § Use the tstats command
           § Create global searches
           
[33. Customizing Dashboards](https://github.com/isabelle-le/Splunk-selflearning/blob/master/33.%20Customizing%20Dashboards.md)

           § Customize chart and panel properties 
           § Set panel refresh and delay times
           § Disable search access features
           § Define event annotations
           
[34. Using Drilldowns (dynamic drilldowns)](https://github.com/isabelle-le/Splunk-selflearning/blob/master/34.%20Using%20Drilldowns.md)

           § Define types of drilldowns 
           § Identify predefined tokens 
           § Create dynamic drilldowns

[35. Adding Advanced Behaviors & Visualizations (event handler)](https://github.com/isabelle-le/Splunk-selflearning/edit/master/35.%20Adding%20Advanced%20Behaviors%20&%20Visualizations.md)

           § Identify types of event handlers 
           § Describe event actions
           § Create contextual drilldowns
           § Use simple XML extensions
           § Define Splunk Custom Visualizations

## Analytics and Data Science
[Summary of getting started with MLTK recoding from Splunk](https://github.com/isabelle-le/Splunk-selflearning/blob/master/Getting%20started%20with%20MLTK.md)

[Course Topics](https://github.com/isabelle-le/Splunk-selflearning/blob/master/Splunk%207.0%20for%20Analytics%20%26%20Data%20Science%20MLTK%203.0%20Description.pdf)

[MLTK on SPlunk doc](https://docs.splunk.com/Documentation/MLApp/5.1.0/User/Algorithms)

[36. Analytics Framework + Exploratory data Analysis](https://github.com/isabelle-le/Splunk-selflearning/blob/master/36.%20Analytics%20Framework%20%2B%20Exploratory%20data%20Analysis.md)

           § Analytics Framework
           § Exploratory data Analysis


[37. Machine Learning Workflow](https://github.com/isabelle-le/Splunk-selflearning/blob/master/37.%20Machine%20Learning%20Workflow.md)

           • Define some concepts and terms associated with machine learning
           • Describe the machine learning workflow
           • Split data for training and testing models
           • Fit and apply models in Splunk
           • Use Machine Learning Toolkit Showcases and Assistants
           
[38. Classification](https://github.com/isabelle-le/Splunk-selflearning/blob/master/38.%20Classification.md)
           
           § Define key classification terms
           § Evaluate classifier results
           
[39. Anomaly Detection](https://github.com/isabelle-le/Splunk-selflearning/blob/master/39.%20Anomaly%20Detection.md)

           § Define anomaly detection
           § Identify anomaly detection use cases
           § Describe Splunk anomaly detection solutions    
           
[40. Regressors](https://github.com/isabelle-le/Splunk-selflearning/blob/master/40.%20Regressors.md)

We covered category prediction in section 38. So we consider only regressors in this section.

           § Define estimation and prediction
           § Identify estimation and prediction use cases 
           § Describe Splunk estimation and prediction
           Solutions
     
## Additional:
It will be a miss if we stop learning about ML at this stage. Normally, our data is messy and not ready to apply ML algrs( unlike kaggle prepared dataset). We need to have additional skill sets to manipulate, analyse data. That is being said, we cover as follow:

           1. Preprocessing
           2. Featue Extraction
           3. Utility algorithms
           4. Cross-validation
           5. Clustering algorithms with scoring
           6. Time Series analysis
           7. Configure algorithm performance costs
           8. Statistical functions and testings
[41. Preprocessing](https://github.com/isabelle-le/Splunk-selflearning/blob/master/41.%20Preprocessing%20(Prepare%20Data).md)

           1.Imputer
           2.RobustScaler
           3.StandardScaler
           
[42. Featue Extraction](https://github.com/isabelle-le/Splunk-selflearning/blob/master/42.%20Feature%20Extraction.md)

           1.FieldSelector
           2.HashingVectorizer
           3.ICA
           4.KernelPCA
           5.NPR
           6.PCA
           7.TFIDF
[43. Utility algorithms](https://github.com/isabelle-le/Splunk-selflearning/blob/master/43.%20Utility%20algorithms.md)

           ACF (autocorrelation function)
           PACF (partial autocorrelation function)
           
[44. Time Series analysis](https://github.com/isabelle-le/Splunk-selflearning/blob/master/44.%20Time%20Series%20Analysis.md)
           
          1. Time Series analysis
          2. Kalman filter
          3.ARIMA
          4.StatSpaceForecast
     
[45. Cross-validation](https://github.com/isabelle-le/Splunk-selflearning/blob/master/45.%20Cross%20validationn.md)

           1. k_fold cross validation
           disadvantage : (1) can not used in saved model (2) expensive conputation time with Splunk MLTK
           
[46. Clustering algorithms](https://github.com/isabelle-le/Splunk-selflearning/blob/master/46.%20Clustering%20algorithms.md)
           
           1. Birch
           2. DBSCAN
           3. K-means
           4. SpectralClustering
           5. X-means
           Bonus: 1. Silhouette score (score on categorical data)
                  2. Pairwise distance scoring
     
[47. Configure algorithm performance costs](https://github.com/isabelle-le/Splunk-selflearning/blob/master/47.%20Configure%20algorithm%20performance%20costs.md)
 
[48. Statistical functions](https://github.com/isabelle-le/Splunk-selflearning/blob/master/48.%20Statistical%20functions.md)

           Statistical functions (statsfunctions)
           1. Describe
           2. Moment
           3. Pearson
           4. Spearman
           5. Tmean
           6. Trim
           7. Tvar
  [49, Statistical testing](https://github.com/isabelle-le/Splunk-selflearning/blob/master/49.%20Statistical%20testing.md)
  
           Statistical testing (statstest)
           1. Analysis of Variance (Anova)
           2. Augmented Dickey-Fuller (Adfuller)
           3. Energy distance
           4. Kolmogorov-Smirnov (KS) test (1 sample)
           5. Kolmogorov-Smirnov (KS) test (2 samples)
           6. Kwiatkowski-Phillips-Schmidt-Shin (KPSS)
           7. MannWhitneyU
           8. Normal-test
           9. One-way ANOVA
           10. T-test (1 sample)
           11. T-test (2 independent samples)
           12. T-test (2 related samples)
           13. Wasserstein distance
           14. Wilcoxon
           
## Advanced Dashboards and Visualizations
[Course Topics](https://github.com/isabelle-le/Splunk-selflearning/blob/master/Splunk7.3AdvDashAndViz_CourseDescription.pdf)
