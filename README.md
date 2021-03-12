# jhu-phd-life-science-career
An analysis of chosen career sectors for life science PhD programs at Johns Hopkins University

## Background Information
This analysis aims to use a cluster analysis to identify the primary sectors that life science PhD program graduates pursue. in 2017, an article published in [Inside Higher Ed](https://www.insidehighered.com/news/2017/12/15/new-calls-clear-easily-accessible-data-phd-program-outcomes-life-sciences) discusses a commitment that institutions made to provide transparent data about life science PhD programs, specifically about admissions and career outcomes. Many students who graduate will not end up in expected faculty positions, so the purpose of the published data is to allow PhD candidates to understand the likelihood of pursuing careers in a specific sector. The [Next Generation Life Sciences Coalition](https://nglscoalition.org/coalition-data/) has compiled data from many university life science programs, allowing students to compare options and understand the statistics before graduating. As a student at Johns Hopkins University, I am curious to understand the different sectors that different PhD candidates pursue in the life sciences. This analysis will group different fields of study into clusters based on postgraduate career sectors.   

## Business Question
What sectors do different Johns Hopkins University PhD life science program graduates pursue, and how can the career center use this information to improve career outcomes? 

## Open Data
This analysis uses open data from the [Next Generation Life Sciences Coalition](https://nglscoalition.org/coalition-data/), specifically [Johns Hopkins University](https://provost.jhu.edu/wp-content/uploads/sites/4/2020/09/ADA-Tables.pdf), which provides career outcomes for post graduate and PhD graduates. 

The following data set was used for this analysis. The original data used can be found [here](https://github.com/cshah13/jhu-phd-life-science-career/blob/main/Original%20Data.xlsx).
- Johns Hopkins University, Career Outcomes of Life Science PhD Graduates 2003-2020

## Data Analysis Question
Microsoft Office Excel will be used to conduct a cluster analysis to answer the following data question:
1. How can postgraduate career sectors for life science PhD program graduates at Johns Hopkins University be categorized into three clusters?

## Data Answer
### How can postgraduate career sectors for life science PhD program graduates at Johns Hopkins University be categorized into three clusters?
The Microsoft Office Excel Solver tool was used to identify three clusters. The cluster analysis divided the different areas of study for life science PhD programs at Johns Hopkins University into three clusters. These clusters are defined by the average students who pursue a career in specific sectors after graduation; the sectors are academia, for profit, government, non profit, and not found. Cluster 1 is below average in each of these categories; the cluster rod is Program in Molecular Biophysics, which is also the only area of study in this cluster. Cluster 2 is above average in academia, above average in for profit, below average in government, below average in non profit, and below average in sector not found; the cluster rod for this is Biophysics and Biophysical Chemistry, and there are six total areas of study within the cluster. Lastly, Cluster 3 is below average in academia, below average in for profit, above average in government, above average in non profit, and above average in sector not found; the cluster rod is Human Genetics, and there are 20 total areas of study in this cluster. It is important to note that the characteristics described for each cluster are the characteristics of the cluster rod which represents the cluster. The individual areas of the study within each cluster do not share the exact characteristics. The clusters can all be visualized below. The full data analysis with the calculated z scores and cluster analysis can be found [here](https://github.com/cshah13/jhu-phd-life-science-career/blob/main/Cluster%20Analysis.xlsx).
![alttext](https://github.com/cshah13/jhu-phd-life-science-career/blob/main/Cluster%20Visualization.png)
## Business Answer
The analysis indicates that 

## Step by Step Instructions
1. Downloaded raw data from the Next Generation Life Sciences Coalition
2. Converted the PDF into Excel through the Microsoft Excel upload PDF data function
3. Cleaned the data by removing "n" values and only keeping percentages for each category
4. Used excel functions to calculate z scores for the values in each category, identified three sample cluster nods, used VLOOKUP to identify the cluster rod names, and calculated the distance squared for each value
5. Calculated the minimum for each distance squared value, used the MATCH function to identify clusters, and calculated the sum of the minimums
6. Used the Excel solver function to minimze the sum of minimums, identifying three new cluster rods 
7. Color coded the new clusters associated to each area of study
