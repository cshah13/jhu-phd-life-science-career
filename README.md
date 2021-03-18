# jhu-phd-life-science-career
An analysis of chosen career sectors for life science PhD programs at Johns Hopkins University

## Background Information
This project aims to use a cluster analysis to identify the primary sectors that life science PhD program graduates pursue. In 2017, an article published in [Inside Higher Ed](https://www.insidehighered.com/news/2017/12/15/new-calls-clear-easily-accessible-data-phd-program-outcomes-life-sciences) discusses a commitment that institutions made to provide transparent data about life science PhD programs, specifically about admissions and career outcomes. Many students who graduate will not end up in expected faculty positions, so the purpose of the published data is to allow PhD candidates to understand the likelihood of pursuing careers in a specific sector. The [Next Generation Life Sciences Coalition](https://nglscoalition.org/coalition-data/) has compiled data from many university life science programs, allowing students to compare options and understand the statistics. As a student at Johns Hopkins University, I am curious to understand the different sectors that different PhD candidates pursue in the life sciences. This analysis will group different fields of study into clusters based on immediate postgraduate career sectors.   

## Business Question
What career sectors do different Johns Hopkins University PhD life science program graduates pursue, and how can the career center use this information to improve career outcomes? 

## Open Data
This analysis uses open data from the [Next Generation Life Sciences Coalition](https://nglscoalition.org/coalition-data/), specifically [Johns Hopkins University](https://provost.jhu.edu/wp-content/uploads/sites/4/2020/09/ADA-Tables.pdf), which provides career outcomes for post graduate and PhD graduates. 

The following data set was used for this analysis. The original data used can be found [here](https://github.com/cshah13/jhu-phd-life-science-career/blob/main/Original%20Data.xlsx).
- Johns Hopkins University, Career Outcomes of Life Science PhD Graduates 2003-2020

## Data Analysis Question
Microsoft Office Excel will be used to conduct a cluster analysis to answer the following data question:
1. How can immediate postgraduate career sectors for life science PhD program graduates at Johns Hopkins University be categorized into three clusters?

## Data Answer
### How can immediate postgraduate career sectors for life science PhD program graduates at Johns Hopkins University be categorized into three clusters?
The Microsoft Office Excel Solver tool was used to identify clusters. The cluster analysis divided the different areas of study for life science PhD programs at Johns Hopkins University into three clusters. These clusters are defined by the average students who pursue a career in specific sectors after graduation; the sectors are academia, for profit, government, non profit, and not found. Cluster 1 is above average in academia, below average in for profit, below average in government, below average in non profit, and above average in sector not found; the cluster node is Clinical Investigation, and there is a total of three areas of study in this cluster. Cluster 2 is below average in academia, above average in for profit, below average in government, below average in non profit, and below average in sector not found; the cluster node for this is Chemistry, and there are seven total areas of study within the cluster. Lastly, Cluster 3 is below average in academia, below average in for profit, above average in government, above average in non profit, and above average in sector not found; the cluster node is Human Genetics and Molecular Biology, and there are 17 total areas of study in this cluster. It is important to note that the characteristics described for each cluster are the characteristics of the cluster node which represents the cluster. The individual areas of study within each cluster do not always share the exact characteristics. The clusters can all be visualized below. The full cluster analysis with the calculated z scores for each category can be found [here](https://github.com/cshah13/jhu-phd-life-science-career/blob/main/Cluster%20Analysis.xlsx).

![alttext](https://github.com/cshah13/jhu-phd-life-science-career/blob/main/Visualization%20of%20Clusters.png)
## Business Answer
The analysis indicates that there is a lot of variation in the sectors that life science PhD students at Johns Hopkins University pursue after graduation. This data is important for the Johns Hopkins University career center to best support students. Since the academia sector is above average in Cluster 1, the career center can focus on preparing students for interviews in this sector. The sector not found is also above average, indicating that the career advisors for these areas of study may need to spend more time collecting postgraduate information from students. The students who enter the non profit, for profit, and government sectors are below average; there could either be less opportunities available in these sectors, or students are having difficulty acquiring jobs in these sectors. The career center can utilize this information to spend time preparing students for the sectors that are underrepresented. 

Since for profit is the only sector above average in Cluster 2, the career center can focus outreach efforts on bringing for profit companies to interview students at the university. However, the lower values in the other sectors may mean the students are lacking resources to acquire jobs that are not in the for profit sector, so the career center will need to analyze their efforts to understand if more work is needed to prepare students for other sectors.

Cluster 3 is above average in the government and non profit sectors; the same logic applies in this situation. More resources can be dedicated to these two sectors to help students since it is clear they pursure these sectors, or more resources can be dedicated to preparing students for academic and for profit sectors if they are not prepared to enter those roles. Cluster 3 is above average in sector not found, so the career center and departments can connect with students in the future to gain missing information.

This data is helpful for career centers to identify the trend of sectors that post PhD students pursure in each life science area of study. The high/low numbers could either be attributed to the available resources to prepare for the jobs, or the lack of resources to prepare for a role in the specific sector. Further analysis is needed to make a conclusion; for example, the current programs offered by the career center can be analyzed to understand strengths and gaps. This information will allow the career center to improve their practices and best support life science PhD students.


## Step by Step Instructions
1. Downloaded raw data from the Next Generation Life Sciences Coalition
2. Converted the PDF into Excel through the Microsoft Excel upload PDF data function
3. Cleaned the data by removing "n" values and only keeping percentages for each category
4. Used Excel functions to calculate z scores for the values in each category, identified three sample cluster nodes, used VLOOKUP to identify the cluster node names, and calculated the distance squared for each value
5. Calculated the minimum for each distance squared value, used the MATCH function to identify clusters, and calculated the sum of the minimums
6. Used the Excel Solver function to minimze the sum of minimums, identifying three new cluster rods 
7. Color coded the new clusters associated to each area of study
8. Moved clusters into a visualization chart and created a key to easily identify characteristics
