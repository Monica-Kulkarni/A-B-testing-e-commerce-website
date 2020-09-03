My goal for this project was to perform A/B testing on a product, here being the interface of an e-commerce website.
Here, I've used a database providing details on the conversion rate of two groups(treatment group that holds the new interface and 
control group that holds the old interface), on an e-commerce platform from 1st to 24th January, 2017.
The aim was to decide whether the e-commerce website should keep the old interface or change it to the new one.

![working](https://github.com/Monica-Kulkarni/A-B-testing-e-commerce-website/blob/master/working.png)


I analyzed user conversion rate vs. their landing_pages. Both A/B testing and logistic regression were employed to answer the same question.

(1) In A/B testing, I performed a one-sided hypothesis testing: whether new page leads to more conversion rate. The null is new page is not better than old page. The alternative is new page is better. The resulted p value from my test is 0.9, therefore I failed to reject null, and conclude that new page is not better in leading to conversion.

(2) In the logistic regression method, I intend to prove that conversion rate depends on landing page, therefore it is a two-sided hypothesis test. The null is there is no difference between the conversion rate of old and new page. The alternative is there is a difference. The resulted p value from my test is close to 0.2, therefore I failed to reject null, and conclude that there is no statistically significant difference in conversion rate between old and new landing_page.

(3) Beside landing_page, I also tested whether country matters in conversion rate. I didn't find any statistically significant evidence that country matters. In other words, country does not matter.

(4) I also tried to find out whether day of week matters. When considering all 7 days of weeks, I didn't find statistically significant evidence to support that a specific day of week has better conversion rate. But when comparing Monday and Friday, I did find that Monday conversion rate is statistically better than Friday.

(5) I then tried to find out whether running the test longer time improves conversion rate. Neither old_page nor new_page conversion rate improved with time. From the linear regression of p_new-p_old against day, the R-square=0, and p value is close to 1. Therefore is not any indication that running the test longer will improve test results, and I DO NOT suggest running longer time.
