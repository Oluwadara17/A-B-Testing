## Title: A/B Testing
# Author: Oluwadara Olamide 
## About Data
I used the Fast-Food Marketing Campaign A\B Test dataset gotten from 
(https://www.kaggle.com/datasets/chebotinaa/fast-food-marketing-campaign-ab-test). 
# Task
Analyze the A/B test and provide recommendations.
Some notes:
- The dataset is aggregated by LocationID, PromotionID and week. I should aggregate by LocationID and PromotionID before conducting the statistical tests.
- Since there are three marketing campaigns and Ihave to select the best-performing one, I will have to conduct several tests, comparing campaigns against one another.. This kind of testing is known as pairwise comparisons and it suffers from the [multiple testing problem](https://en.wikipedia.org/wiki/Multiple_comparisons_problem) - if we run a lot of tests, there’s an increased chance of getting a type I error (false positive). It is therefore suggested to use the confidence level of 99% instead of the traditional 95% in your graded task.
# Evaluation Criteria
- General understanding of the topic
- [A/B Testing] SQL queries are correct and follow SQL best practices.
- [A/B Testing] Metrics are correctly calculated.
- The document with AB test results is clear, concise and follows the required structure.
- [A/B Testing] The results of statistical tests are performed and interpreted correctly.
- Analytical approach to the problem. Did the learner use their analysis to provide justified, useful and actionable insights?

# Additional Resources for this Sprint
Probability, statistical inference and A/B testing are all incredibly rich topics. If you are curious to learn more, jump into the resources below or save them for later use.

- Probability
 - (optional) Harvard course - [Fat Chance](https://www.edx.org/learn/probability/harvard-university-fat-chance-probability-from-the-ground-up?webview=false&campaign=Fat+Chance%3A+Probability+from+the+Ground+Up&source=edx&product_category=course&placement_url=https%3A%2F%2Fwww.edx.org%2Flearn%2Fprobability)
 - (optional) Harvard course - [Introduction to Probability](https://www.edx.org/learn/probability/harvard-university-introduction-to-probability?webview=false&campaign=Introduction+to+Probability&source=edx&product_category=course&placement_url=https%3A%2F%2Fwww.edx.org%2Flearn%2Fprobability)
- Statistical Inference
  - (optional) [Naked Statistics: Stripping the Dread from the Data](https://www.amazon.com/Naked-Statistics-Stripping-Dread-Data-ebook/dp/B007Q6XLF2/ref=sr_1_1?crid=33VPRFJX4VFIL&dib=eyJ2IjoiMSJ9.OKn1Bp9Nz1pH-8oKG1xpCysMkcs3yXSTIrd3esT-pKM339nsXKQBroxUPAVsp7v7WXA35YGdn2TfFza-6QJHobwGY7I8_0WVMY8DVQDSrpx8fRokBVGVN0Q-Yu1w7T5qUYkFBnme9sBo0lOrApsIwTO-0KOlY-WEJdv125Q8xGtZBghb6-aAbVbNr6eP-oRV-BHBV1g2HFqfNvMakj_bC9jtGY2DoG4pDZAsflXVtwc.yesyDDR7bEC7jNqbvhhWcqA9pDJLzycMidMk4fUcO1Q&dib_tag=se&keywords=naked+statistics&qid=1712002647&sprefix=naked+statistic%2Caps%2C163&sr=8-1)
  - (optional) [What is a p-value anyway?](https://www.amazon.com/p-value-Stories-Actually-Understand-Statistics/dp/0321629302/ref=sr_1_1?crid=2J9EWYJPTW73N&dib=eyJ2IjoiMSJ9.gWDvAFBbVRFPWje42tkIfQKHupn_dR73DYfm0eyiQs0bg2pjLjp_WMRDs9fqpDREimG43FJzC6upLsKSJw3OLoyq2ZGJxP4dFcqcHL84Jbg1Sf52HxaAaKNtRy1CQ8JBkvIjOqv4BfkoEBdSj2FSsx-UIdA75L8zRjtruPf_0bjuWPqwkC3AukBW8uzgQk2iRhUuvH_Yv7_o5z3VgvgAbTY2BtSotkCdmtlsx1wCUBQ.KXuyH48qZAfXpa4_QI6qS1crxeyw0J6TeZ94KwWvZZw&dib_tag=se&keywords=what+is+a+p+value+anyway&qid=1712002724&sprefix=what+is+a+p+value%2Caps%2C172&sr=8-1)
  - (optional) [Andrew Gelman Blog](https://statmodeling.stat.columbia.edu/)
  - (optional) [Harvard’s Statistics 110: Probability course](https://projects.iq.harvard.edu/stat110)
  - (optional) [Richard McElreath - Statistical Rethinking](https://xcelab.net/rm/)
  - (optional) [Allen Downey Blog](https://www.allendowney.com/blog/)
- A/B Testing
  - (optional) [Ronny Kohavi, Diane Tang, Ya Xu - Trustworthy Online Controlled Experiments: A Practical Guide to A/B Testing](https://www.amazon.com/Trustworthy-Online-Controlled-Experiments-Practical)


