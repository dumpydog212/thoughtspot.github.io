---
title: [Comparative Analysis]
tags: [spotiq]
keywords: SpotIQ, comparative analysis, complex measures
summary: "With SpotIQ competitive analysis, you can compare two data points for complex measures."
last_updated: 07/26/2019
sidebar: mydoc_sidebar
permalink: /:collection/:path.html
---
With SpotIQ competitive analysis, you can compare two data points for simple or complex measures:  
  * _Sum_
  * _Count_
  * _Sum over sum_, which generate a pinboard that has 'what-if' percentage insights
  * _Average_, which generate a pinboard that has 'what-if' percentage insights
  * _Unique count_, which uses a 'versus' analysis to show the absolute change grouped by different drill attributes

## Basic Comparative Analysis in SpotIQ ##

To perform this analysis, follow these steps:  

1. On a column chart, hold down the command key \(Mac OS\) or control key \(Linux or Windows\).  

2. Click the two columns you plan to compare. Here, we are comparing the results for _San Francisco_ and _Atlanta_ stores.

3. Right-click to see the drop-down menu, and select **SpotIQ Analyze**.  
   ![]({{ site.baseurl }}/images/comparative-analysis-1.png "Starting comparative analysis")

4. In the SpotIQ information modal, click **Got it**.  
   ![]({{ site.baseurl }}/images/comparative-analysis-2.png "Got it")

5. In the window modal, under **Columns**, select the columns for SpotIQ to compare. By default, all columns appear selected.  

   Here, we selected _Department_, _Age Group_, and _Store Region_.  

   Click **Analyze**.   

  ![]({{ site.baseurl }}/images/comparative-analysis-3.png "Analyze selected columns")


## Viewing Results ##

Notice that ThoughtSpot saves the results of SpotIQ analysis for 24 hours.

To view the results of your analysis, follow these steps:  

1. On the top navigation bar, click **SpotIQ**.  
   ![]({{ site.baseurl }}/images/click-spotiq.png "Click SpotIQ")

2. Select the **Results** tab, and the locate your analysis under **All** or **Yours**.  

   Your analysis may be in progress. Wait until its **Status** changes to _Done_.

    Click _View Results_ to open the report.
    ![]({{ site.baseurl }}/images/comparative-analysis-5.png "Opening the Analysis Results")

3. In the report, SpotIQ prepared a visualization for comparing each of the columns identified in the analysis request. In this example, these columns are _Department_, _Age Group_, and _Store Region_.
    ![]({{ site.baseurl }}/images/comparative-analysis-6.png "Analysis Results")

4. You can now examine each visualization in the analysis for details of comparison, give feedback on its usefulness, and so on.  
  ![]({{ site.baseurl }}/images/comparative-analysis-7.png "Possible actions on SpotIQ visualizations")


   | Legend | Action |
   | --- | --- |
   | 1. | **Give feedback**. SpotIQ learns how to improve its feedback based on the information you provide. |
   | 2. | **Add to a pinboard**. You can add the specific visualization to an existing pinboard, or create a new pinboard and add it there. |
   | 3. | **Get the name of the algorithm** |
   | 4. | **More options**, including another round of SpotIQ analysis, download of data as a CSV file, editing this visualization, or editing a copy of the visualization. |

## Advanced Comparative Analysis in SpotIQ ##

ThoughtSpot ships with a number of comparative algorithms. Using the **Advanced** option of SpotIQ, you can adjust the parameters of the analysis, or choose a different comparative algorithm for your data.  

After selecting the relevant analysis columns, click the **Advanced** tab.  

Under **Select Algorithms**, select the name of the algorithm. You may have several options available, or only a single one. In this example, the only valid option is **Change Analysis**.  

Under **Customize algorithm for comparative analysis**, adjust the options. In this example, the algorithm parameters are __Max Diff Elements__, __Max Fraction__, __Min Abs Change Ratio__, and __Min Change Ratio__.

![]({{ site.baseurl }}/images/comparative-analysis-4.png "Advanced analysis Options")


On the SpotIQ Feedback tab, you can see all SpotIQ feedback you have given. Insights that you disliked are pushed to the bottom of the list.

![]({{ site.baseurl }}/images/insight-feedback.png)