# Sun Savers: Sun Country Transactional Analysis
This SCA repository consists of the analyses carried out on the official customer transactions dataset by Sun Country Airlines
Sun Country, a unique airline carrier that is enduring the threat of intense competition from large national brands. The company hopes to know if online booking channels meet their expectations, and how to drive enrolment of ufly reward program and some other questions. To answer the business questions, our data team analysed Sun Country’s transactional data to provide robust insights and understand different segments of customer profiles. These insights will allow Sun Country to know if online booking channels meet the expectations, enhance their customer experience to churn more customers become their members, introduce targeted programs to said customers, and in turn drive their revenue.

This repository consists of EDA, Data preparation, Clustering techniques implemented in an effort to obtain a higher level understanding of the customer profiles followed by enlisting our recommendations.


![image](https://user-images.githubusercontent.com/102503431/210298836-70bb7faf-8245-4116-a81b-5b1526777475.png)

Noting that all of our clustering findings used a sample size of 7218, which is 0.5% of the total data.
Q) Why do we choose K-medoids as our clustering technique?
Firstly, K-medoids, coupled with Gower distance can successfully handle both categorical and numerical types of data. K-medoids is also less sensitive to outliers than other partitioning algorithms as there are outliers in our dataset that might distort our results, thus applying K-medoid will address this problem. Additionally, there is no statistical and distribution assumption about the data, making K-medoids a good choice. It is easy to interpret, considering the Data background of the management hierarchy of Sun Country, this method can help the management better comprehend the conclusions produced.
Q) Are there natural groups of clients based on flight purchase characteristics?
We utilized the K-medoids clustering to cluster our clients into three big groups:
 - Cluster 1 - Prospective members
This segment consists of customers that belong only to the Non-member category (without any Elite or Standard members) and primarily booked flight tickets using the Sun Country Airline(SCA) website. They also have the least mean base fare amongst three segments($260).
- Cluster 2 - Retention Members
This segment consists of a slightly older (average age of 45)highest spending group(mean base fare of $290), which consists of 49.3% of First-class Booked in sample, and highest median Base fare($265). Also, this cluster consists of the highest number of standard members(3064), additionally all of the Elite members belong to this cluster as well.
- Cluster 3 - Tough Nut Customer
This segment consists of the youngest (mean age of 36) non-members. Although these non-members((3064 in total) spent significantly($273 mean base fare), they booked all their tickets via outside booking channels(100%) .
Q ) Do online booking channels meet the expectations?
Most customers book through the SCA website, which accounts for 42.47%. 67.98% of customers among standard members and 71.5% of customers among elite members book via the SCA website. Among nonmembers, 35.98% of customers book tickets through the SCA website, and 48.5% of customers book using outside bookings. This is in line with Sun Country’s expectations.
    
Recommendations
1) Prioritizing targeted marketing efforts to drive enrollment based on cluster specific needs will lead to marketing cost reduction.
● “Retention Members” (Cluster 2) has higher spending, highest number of standard members, and all of the Elite group are in this segment. We can target these people who are likely to be open to become a member but not a member yet in this group through getting main customers’ characteristics of cluster 2.
● “Tough Nut” customer cluster(Cluster 3) is mostly booking coach-booked classes with an outside booking channel. Outside Booking is through the third party and is harder to target these customers to sign up for a reward program.
● So through prioritizing non-member in the “Retention Members” group and not prioritizing “Tough Nut” customers can lead to a cost effective marketing strategy.
2) Making the UflyMember enrollment process more visible and easier on SCA website can increase member enrollment of “Prospective Members '' who are not members but make flight bookings on SCA website.
Most of the “Prospective Members ''(cluster 1) booked their flight on the SCA website, but not enrolled as a member. In the checkout process, SCA can make the enrollment process easier through simply becoming a member button, with an incentive of discount for their flight ticket. Also on the website itself, they can put a UflyMember banner to make the enrollment process visible and easy.
