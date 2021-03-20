# Stock-Analysis
Performing analysis on stocks to calcualte the daily total volumen and return

## Table of Contents
- [1.0 Introduction](#Introduction)
  * 1.1 Purpose
  * 1.2 Tools
- [2.0 Analysis and Challanges](#Analysis-and-Challenges)
  * 2.1 Stock Performance 2017 and 2018
- [3.0 Results](#Results)
  * 3.1 Stock Performance 2017 and 2018
- [4.0 Resources](#Resources)

<a name="Introduction"></a>
## 1.0 Introduction

### 1.1 Purpose
Steve wants to know how the stocks performed in 2017 and 2018 with a click of a button. This code should run efficiently and also provide the yearly information needed for the year requested.  He wants to know the yearly return as well as volume. 

### 1.2 Tools
- Excel
  - VBA
 
<a name="Analysis-and-Challenges"></a>
## 2.0 Analysis and Challenges
### 2.1 Theater Outcomes by Launch Date
#### 2.1.1 Analysis
The analysis for “Theater Outcomes by Launch Date” was created by first editing the time stamps from Unix to a short date, and then creating a pivot table to aggregate the data.  By translating the Unix time stamp to short date using the following formula: 

`=((("Unix Date"/60)/60)/24)+DATE(1970,1,1)`. 

A pivot table was created to display the outcome of the theaters based off of the month that they were launched. This way you can filter on the year the theater was launched to see if there is a trend in the data, as well as to see if there is an overall trend over the years.   
![alt text](Resources/Pivot_Table.png)
#### 2.1.2 Challenges
The main challenges faced in this module was understanding how an index should be written in VBA.  The module did not clearly explain this, so therefore days were spent trying to understand how an index should be written in VBA. Another challenge faced was understanding what the code was exactly doing.  After attending many office hours it was clear how to interpret the code.  I also had a challenge outputting the yearly percentage return for every stock, but did not have an issue outputting the yearly volume.  This was unclear as to why the volumes were outputting correctly, but the start and end ticker prices were not. 
(Resources/Challenge_return.png)

<a name="Results"></a>
## 3.0 Results
### 3.1 Theater Outcomes by Launch Date
The peak months, April to August, are when the most theaters met or exceeded their goal. The maximum number of plays is in the month of May, and the ratio of successful vs failed is also the greatest in May and June.  From 2009 - 2013 all the plays were successful and then there is a sharp increase in the total number of plays after that.
![alt test](Resources/Theater_Outcomes_vs_Launch.png)

The availability of data limited the analysis, as data from 2009 to 2013 only contianed successful plays.  The data could also be displayed in a bar chart.

<a name="Resources"></a>
## 4.0 Resources
Office Hours
