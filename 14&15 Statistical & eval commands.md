# 14. Exploring Statistical Commands

## Performing statistical analysis with functions of the stat command
* Return : Provides statistics, grouped optionally by fields.

* Syntax : stats (stats-function(field) [AS field])... [BY field-list]

stats-function(field)
![](image./stats-fun.png)
 
[AS field] [BY field-list]: optional

* ![Document](https://docs.splunk.com/Documentation/Splunk/8.0.3/SearchReference/Stats)

* Example : index=coronavirus sourcetype=auto_test granularite = departement
|stats max(hospitalises), max(deces) by maille_nom
|sort- max(hospitalises)![](images./.png)

![](image./stats.png)
## Using fieldsummary
* Return : statistic table of dataset: count/distinct_count, is_exact, max, min, mean, numeric_count, stdev, values of each and every fields 

* Syntax : fieldsummary [maxvals=int] [wc-field-list]

[maxvals]: Optional args. Specifies the maximum distinct values to return for each field. Default is 100

[wc-field-list]: Optional args. Wildcard excepted: cas_confirmes or cas_*

* ![Document](https://docs.splunk.com/Documentation/Splunk/8.0.2/SearchReference/Fieldsummary)

* Example : index=coronavirus sourcetype=auto_test |fieldsummary

![](images./fieldsummary.png)
## Using appendpipe
* Return : Appends the result of the subpipeline applied to the current result set to results. Subpipeline is not a proper search (can not run individually)

* Syntax : appendpipe [run_in_preview= bool] [ subpipeline ]

[run_in_preview= bool]: Optional arg. Default=true. When it is false, the appendpipe is inactivate.

[subpipeline]: Optional arg. A list of commands that are applied to the current search results.

* ![Document](https://docs.splunk.com/Documentation/Splunk/8.0.3/SearchReference/Appendpipe)

* Example : index=coronavirus sourcetype="auto_test"  granularite = departement 
| stats max(date) by maille_nom, hospitalises,deces, reanimation
| sort 101 -max(date)
| appendpipe run_in_preview=true
    [|stats max(reanimation) by maille_nom, hospitalises,deces]

![](images./appendpipe.png)

index="coronavirus" sourcetype="auto_test" date >"2020-03-30" maille_code=DEP-78
|sort -date 
|dedup date 
| appendpipe
    [|stats first(hospitalises) as current, last(hospitalises) as previous
|eval infected_ratio =round((current/previous -1)*100,2)
|eval hospitalises = 'infected_ratio' + "%"]
|table date,maille_nom,hospitalises,reanimation,deces,gueris,source_nom

![](images./appendpipe2.png)
## Using eventstats
* Return : 

* Syntax : 

[maxvals]: Optional args. Specifies the maximum distinct values to return for each field. Default is 100
 

* ![Document](https://docs.splunk.com/Documentation/Splunk/8.0.2/SearchReference/Eventstats)

* Example : 
![](images./.png)

## Using streamstats

* Return : 

* Syntax : streamstats <stats-agg-term>... [<by-clause>]

Optional args: [reset_on_change=bool] 
		[reset_before="("<eval-expression>")"] 
		[reset_after="("<eval-expression>")"] 
		[current=bool] 
		[window=int] 
		[time_window=span-length] 
		[global=bool] 
		[allnum=bool]

[reset_on_change=bool]: Default is false. Specifies that all of the accumulated statistics are reset when the group by fields change. 

[time_window=span-length] :

[current=bool] :

[window=int] :

[global=bool] :

* ![Document](https://docs.splunk.com/Documentation/Splunk/8.0.2/SearchReference/Streamstats)

* Example : Use streamsstats to create a new col that show the prev values of hospitalises, in order to calculate infection_ratio

index="coronavirus" sourcetype="auto_test" 
| where in  (maille_code,"DEP-75","DEP-77","DEP-78","DEP-91","DEP-92","DEP-93","DEP-94","DEP-95")
|sort 16 -date 
|table date,maille_nom,hospitalises,taux_infection,reanimation,deces,gueris,taux_infection
|sort date
|streamstats first(hospitalises) as prev_h by maille_nom
|eval taux_infection = round(((hospitalises/prev_h -1)*100),2)
|eval taux_infection = 'taux_infection'  +"%"
|sort 8 -date
|sort -hospitalises
|fields - prev_h

![](images./streamsstats1.png)

# Note:
* [custom command video](https://www.youtube.com/watch?v=sJRTIyZZtbM)
* [command by category document] (https://docs.splunk.com/Documentation/Splunk/8.0.3/SearchReference/Commandsbycategory)

append: Appends subsearch results to current results.
selfjoin: Joins results with itself.

# 15. Exploring eval Command Functions

![Here](https://github.com/isabelle-le/Splunk-selflearning/blob/master/5.%20Filtering%20and%20format%20result.md)

* Using conversion functions
* Using data and time functions
* Using string functions
* Using comparison and conditional functions 
* Using informational functions
* Using statistical functions
* Using mathematical functions
* Using cryptographic functions
