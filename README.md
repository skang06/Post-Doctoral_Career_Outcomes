# Career Outcomes for Post-Doctoral Students
## Background

According to the [National Postdoctoral Association](https://www.nationalpostdoc.org/page/What_is_a_postdoc), a "postdoc" is is an "individual holding a doctoral degree who is engaged in a temporary period of mentored research and/or scholarly training for the purpose of acquiring the professional skills needed to pursue a career path of his or her choosing." In other words, they are engaging in research and/or training at a university while they decide what they want to pursue as a career. Thus, it would be helpful to see what career paths postdocs from different departments at Johns Hopkins University pursue because it could help the career center accommodate current postdoctoral students at Hopkins.

 A look into Johns Hopkins data from [Next Generation Life Science Coalition](http://nglscoalition.org/coalition-data/#close) will elucidate the different career paths that Hopkins postdocs from different departments pursue. There will be a focus on some of the areas that postdocs commonly pursue, such as academia, for-profit, goverment, non-profit, teaching positions or non- science related fields could prove useful for career centers to provide adequate support.

## Business Question

___How can Johns Hopkins University's career center provide different career opportunities and resources for post-doctoral students in different departments?___


## Open Data 

__[Next Generation Life Science Coalition](https://provost.jhu.edu/education/graduate-and-professional-education/cngls/):__ this library contains the different career outcomes for postdocs and doctorul students at Hopkins. [Career outcomes for postdocs](https://provost.jhu.edu/education/graduate-and-professional-education/cngls/postdoctoral-career-outcomes-tabular-format/) was used.

- [Postdoc Career Outcomes Data Part 1](https://github.com/skang06/Post-Doctoral_Career_Outcomes/blob/main/tabula-Postdoc-CareerOutcome-ADATables-083019-2.csv): Dataset containing original data source where the percentage of postdocs from each department or center going into "teaching" and "non-science related" data was gleaned from.

- [Postdoc Career Outcomes Data Part 2](https://github.com/skang06/Post-Doctoral_Career_Outcomes/blob/main/tabula-Postdoc-CareerOutcome-ADATables-083019.csv): Dataset containing original data source where where the percentage of postdocs from each department or center going into "Academia," "for-profit," "goverment," "non-profit" was gleaned from.

## Data Analysis 

___How does the data group itself into separate clusters?___

K-means clustering analysis was used in Excel. The cluster analysis was initally conducted with 3 anchors. As the aim is to find the anchors that minimize the sum of the minimum squared distances between the anchors and the individual data points, a cluster analysis with 4 nodes was also conducted. The 4-cluster analysis had a lower sum than 3 nodes. The 5-cluster analysis also had a lower sum. Nonetheless, there was only 1 department in the 5th anchor, which indicated that 5 anchors was unnecessary. Thus, the 4-cluster model was the best.

A step-by-step Excel data analysis can be found [here](https://github.com/skang06/Post-Doctoral_Career_Outcomes/blob/main/Excel%20Step%20by%20Step_3.docx).

__Clusters and Their Characteristics__
![alt text](https://github.com/skang06/Post-Doctoral_Career_Outcomes/blob/main/chart1.png)
![alt text](https://github.com/skang06/Post-Doctoral_Career_Outcomes/blob/main/factors.png)

_Cluster 1_: It is the only cluster that has an above average going into for- profit and the only cluster with an above average percent going into non-profit institutions, although they are both less than one standard deviation above. On the other hand, it has the greatest below average percent going into academia, government, and teaching among the clusters. For academia and teaching, it is more than one standard deviation below average, which demonstrates their unpopularity with postdocs.

_Cluster 2_: It is the cluster with the most above average percent of postdocs going into teaching, although it is less than one standard deviation above. Interestingly, it has a significantly below average percent going into academia (almost one standard deviation lower). So, perhaps those going into teaching are not pursuing teaching positions in academia, unlike what one would normally expect. 
- Very slightly above average government; significantly below average academia/for- profit/ non science related fields; below average non-profit.

_Cluster 3_: It is the cluster with the most above average percent of postdocs going into academia (nearly one standard deviation above the mean). The percent of postdocs going into government is also above average at .65 standard deviations above. 
- Below average for- profit/ non-profiy; slighty below average teaching.  

_Significantly below average going into non science related fields at almost one standard deviation lower for cluster 1,2, and 3._

_Cluster 4_: This cluster has the most above average percent of postdocs going into government (nearly 2 standard deviations above the average). There is also an above average percent of postdocs going into academia, although it is not nearly as many as cluster 3. Slightly above average teaching. 
- Significantly below average in for- profit. It is tied with Cluster 4 for most below average percent of post docs going into for-profit institutions. Among the four clusters, this cluster has the smallest below average percent of postdocs go into non- science related fields, indicating there is a greater percentage going compared to the other clusters, although it is still below average.  Below average non-profit.


__List of Departments and Their Relevant Cluster__

![alt text](https://github.com/skang06/Post-Doctoral_Career_Outcomes/blob/main/list.png)


## Implementation and Summary
This analysis can help the career center divide up their resources and opportunities to postdoc students in different departments based on which career paths are more prevalent in different groups. This is important since there are many departments at Hopkins that house postdocs, so figuring out an organized method of attack helps them work efficiently. Additionally, postdocs are usually doing research and/or training at a university temporarily before they decide where they want to go next in terms of their career, so an effective career center to help facilitate this transition is important. The career center could divide their center into four different subgroups to accomodate the four categories of departments that tend towards similar career paths. What each subgroup of the career center can focus on and do for each cluster of departments is outlined below based on what were the most popular career outcomes.

__Cluster 1 - For-profit and non-profit__: Reach out and organize for-profit and non-profit institutions to come to career fairs or other events for these departments.

__Cluster 2 - Teaching__: Organize more workshops developing skills for teaching such as public speaking and effective ways to teach for the postdocs, as these are skills not learned as much during studies.

__Cluster 3 - Academia and government (to a lesser extent)__: Send out information about universities and colleges, and reach out to them as well. Given that many in academia go into research, provide more awareness on research opportunities. Information about governmental institutions that are hiring would also be of benefit.

__Cluster 4 - Government__: Reach out to governmental institutions for potential job openings, organize workshops focused on governmental law, etc. The center can also let cluster 3 know about these governmental workshops.

Overall, it would not be most effective for the career center to focus on non-science related fields for all the clusters, but perhaps they can look into it more for cluster 4.

Additional data on what specific kinds of companies within non-profits or for-profits the postdocs pursue would provide more detailed analysis. There are a lot of different kinds of nonprofits and for-profit institutions, so having a detailed division of the percentage that go into each helps career centers figure out which ones to target and get information on.

