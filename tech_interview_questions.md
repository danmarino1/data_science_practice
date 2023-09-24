# Data Science Interview Questions

## Probability
1. Two teams play a series of games (best of 7) in which each team has a 50% chance of winning any given round. What is the probability that the series goes to 7 games?
- If they played 7 games, there are 7 * 7 different outcomes, and there's only two cases in which 7 games are played. therefore, the answer is 2/49 or .0408.
  
2. Say you roll a die three times. What is the probability of getting two sixes in a row?
- 6 * 6 * 6 different possibilities, with two chances to get 2 sixes in a row. 2/216 or 0.00925

3. You roll three dice, one after another. What is the probability that you obtain three numbers in a strictly increasing order?
- 6 * 6 * 6, is the number of total combinations, but the first number cannot be greater than 4. Therefore, it is 4 * 1 * 1, so 4 chances out of 212, or 0.0188

4. Assume you have a deck of 100 cards with values ranging from 1 to 100, and you draw two cards at random without replacement. What is the probability that the number of one card is precisely double that of the other?
- For the first card, we can have 100 to choose from. To satisfy the requirements, we need a number whose double is less than 100 (there are 50 of these). first thing (50/50). Then, for the second pull, we have only 1 card out of 99 that will satisfy the requirement. The answer, therefore, is (.5*.01), which is 0.005. It will happen one out of every 200 attempts.

5. Imagine you are in a 3D space. From (0,0,0) to (3,3,3), how many paths are there if you can move only up, right, and forward?


6. One in a thousand people have a particular disease, and the test for the disease is 98% correct. If someone tests positive, what are the odds they have the disease?
- This is a Bayes Theorem question, since we can gain insight on an event given prior events.
- Formula is P(A∣B)= P(B∣A) × P(A) / P(B)
- Where:
   - P(A∣B) is the probability of having the disease given a positive test result.
   - P(B∣A) is the probability of a positive test result given that you have the disease, which is 98% or 0.98.
   - P(A) is the prior probability of having the disease, which is 0.1% or 0.001.
   - P(B) is the total probability of getting a positive test result.

- Calculating  P (B) P(B) To find  P ( B ) P(B), we consider two scenarios:  You have the disease and test positive:  P ( A ) × P ( B ∣ A ) = 0.001 × 0.98 = 0.00098 P(A)×P(B∣A)=0.001×0.98=0.00098 You don't have the disease but still test positive (false positive):  P ( ¬ A ) × P ( B ∣ ¬ A ) = 0.999 × 0.02 = 0.01998 P(¬A)×P(B∣¬A)=0.999×0.02=0.01998 So,  P ( B ) = 0.00098 + 0.01998 = 0.02096 P(B)=0.00098+0.01998=0.02096
- Calculating P(A∣B) P(A∣B): P(A∣B)= (0.02096 / 0.00098) ≈ 0.0468
- The probability of actually having the disease given a positive test result is approximately 0.0468 or 4.68%.

7. Assume two coins, one fair and the other unfair. You flip it five times and get tails all five times. What is the probability that you are flipping the unfair coin?
- This is also a Bayes' Theorem question. 

8. Players A and B are playing a game where they flip a biased coin. What is the probability that A wins?
- If the coin were unbiased, it would be 50/50 or a .5 probability that A wins. Since the coin is biased, it would be .5+- the bias (we'll call that b). Essentially p(A winning) = .5 +- b.

9. Three friends in Seattle each say it is rainy, and each has a 1/3 probability of lying. What is the probability that it is actually rainy?


10. You draw a circle and choose two chords at random. What is the probability that those chords will intersect?

11. You and your friend toss a coin until the sequence HH or TH shows up. What is the probability of you winning?

12. You roll a 6-sided die up to two times. How much are you willing to pay to play this game?
- Hmm this question is vague, so I will answer in terms of units. This is an expected value problem, one in which (I will assume) we are trying to get 1 outcome of a possible 12. That said, probability of winning is .08. It will need a payout of more than 12x my intial investment to be a game worth playing.

13. Given that a rater has labeled four pieces of content as good, what is the probability that this rater is diligent?

14. A couple has two children. You discover one is a boy. What is the probability the other is also a boy?
- Well these events are likely independent, unless they are identical twins. Assuming fraternal twins (or any siblings, for that matter) each have a 50% chance of being males or females, and assuming there is an i% chance of twins being identical, the probability of having another boy is P(other is a boy) = (1−i) ×0.5 + i × 1
- **1 - i:** This term represents the probability that the twins are not identical. If i is the probability that they are identical, then 1 - i is the probability that they are not.
- **\* .5:** This is the probability that the other child is a boy, assuming that the children are not identical twins. Since the events are independent in this case, the probability remains 0.5 (or 50%).
- **\* 1:** This represents the certainty (probability of 1 or 100%) that the other child is a boy if the twins are identical, and you know one of them is a boy.
- **(1−i)×0.5+i×1:** The formula combines these two scenarios. It calculates the weighted sum of the probabilities for each case (non-identical and identical), based on how likely each case is (1−i and i, respectively).
 
15. You open the first 7 drawers of a desk and find them empty. What is the probability the 8th drawer has a letter?

16. Two players are at deuce in a tennis match. What is the probability that the first player wins the match?

17. You have a deck of 50 cards in 5 different colors. What is the probability that two cards you pick are not the same color and number?

18. You have ten fair dice. What is the probability that the sum of all the top faces is divisible by 6?

19. A fair coin is tossed twice. What is the probability that heads show up given that at least one toss was heads?

20. Three ants are sitting at the corners of a triangle. What is the probability that none of the ants meet?

21. A biased coin is tossed. What is the probability that the total number of heads after r tosses is even?

22. Alice and Bob play a series of rounds until one wins two more rounds than the other. What is the probability that Bob wins?

23. You have three draws of uniformly distributed random variables. What is the probability that the median is greater than a certain value?

24. A and B play a game with a die. How much is A willing to pay to play first?

25. You have an unfair coin. How can you generate fair odds?

26. You have a white cube broken into 27 pieces. What is the probability that the bottom face of a randomly picked piece is also white?

27. You break a stick of length 1 into three parts. What is the probability that the pieces can form a triangle?

28. What is the probability that, in a random sequence of H's and T's, HHT shows up before HTT?

29. You have 150 friends, and 3 have phone numbers with some permutation of the digits 0, 1, 4, and 9. Is this just a chance occurrence?

30. A fair die is rolled n times. What is the probability that the largest number rolled is, for each r in 1,..,6?

31. You have a jar with a single amoeba. What is the probability that there will eventually be no living amoeba?

32. A fair coin is tossed n times. What is the probability that the first toss was heads given that there were k heads?

33. You have Ni.i.d. draws of numbers following a normal distribution. What is the probability that k of those draws are larger than some value Y?

34. You pick three random points on a unit circle. What is the probability that the triangle includes the center?

35. You have r red balls and w white balls in a bag. What is the probability that you run out of white balls first?

## Statistics

### Easy
1. Explain the Central Limit Theorem. Why is it useful?
- The central limit theorem notes that given a statistically significant sample, when surveying a particular attribute, most values will fall towards the middle, ie, the central limit. Values across sample will usually drift towards the middle, and distant values will taper off, creating what we know as the bell curve. 
- This is one of the most important phenomenon in statistics, as we can gain many insights on a population (and on samples therein) using the Central Limit Theorem

2. How would you explain a confidence interval to a non-technical audience?
- Confidence intervals are incredibly important, as they highlight that we can never know precisely what an answer will be. For example, if you're investing in your retirement and expect to have $1,000,000 in your account by forty, you may be upset to find out that you only have $850,000 when that day comes. With a bit of tolerance through the use of a confidence interval, we can say that it's 95% likely that the account's value will be between $850,000 and $1,000,000. This helps decision makers and stakeholders plan better, as they can be much more flexible in their expectations, allowances, and risk tolerance. 
- Confidence intervals recognize that statistics is merely a tool for guessing. It will never be precise. Therefore, confidence intervals highlight the imperfections of our analyses and allow us to plan for ranges and contingencies.

3. What are some common pitfalls encountered in A/B testing?
- A/B testing is extremely valueable, but some pitfalls could render it ineffective or counterproductive. Firstly, we need to control all variables except those for which we are testing. If we want to know how a new user interface (UI) affects click-through-rate, we want to test users who are sampled properly. We would not want to give our highest spenders one UI and our lookey-loos another then compare the two cohorts. We'll see different behaviors, and we wouldnt be able to isolate that the UI was the reason.

4. Explain both covariance and correlation formulaically, and compare and contrast them.

5. Say you flip a coin 10 times and observe only one heads. What would be your null hypothesis and p-value for testing whether the coin is fair or not?

6. Describe hypothesis testing and p-values in layman's terms?

7. Describe what Type I and Type II errors are, and the trade-offs between them.

8. Explain the statistical background behind power.

9. What is a Z-test and when would you use it versus a t-test?

10. Say you are testing hundreds of hypotheses, each with a t-test. What considerations would you take into account when doing this?


### Medium
11. How would you derive a confidence interval for the probability of flipping heads in a series of coin tosses?

12. What is the expected number of coin flips needed to get two consecutive heads?

13. What is the expected number of rolls needed to see all 6 sides of a fair die?

14. Say you're rolling a fair six-sided dice. What is the expected number of rolls until you roll two consecutive 5s?

15. A coin was flipped 1000 times, and 550 times it showed heads. Do you think the coin is biased? Why or why not?

16. You are drawing from a normally distributed random variable. What is the approximate expected number of days until you get a value greater than 2?

17. Say you have two random variables X and Y, each with a standard deviation. What is the variance of aX + bY for constants a and b?

18. Say we have X ~ Uniform(0, 1) and Y ~ Uniform(0, 1) and the two are independent. What is the expected value of the minimum of X and Y?

19. Say you have an unfair coin which lands on heads 60% of the time. How many coin flips are needed to detect that the coin is unfair?

20. Say you have n numbers 1..n, and you uniformly sample from this distribution without replacement n times. What is the expected number of distinct values you would get?

21. There are 100 noodles in a bowl. What is the expectation on the number of loops formed?

22. What is the expected value of the max of two dice rolls?

23. Derive the mean and variance of the uniform distribution U(a, b).

24. How many cards would you expect to draw from a standard deck before getting the first ace?


### Hard
25. Assume you are drawing from an infinite set of iid random variables that are uniformly distributed from (0, 1). What is the expected length of the sequence you draw?

26. There are two games involving dice. Which has the higher expected value and why?

27. What does it mean for an estimator to be unbiased? What about consistent?

28. What are MLE and MAP? What is the difference between the two?

29. Say you are given a random Bernoulli trial generator. How would you generate values from a standard normal distribution?

30. Derive the expectation for a geometric random variable.

31. Say we have a random variable X ~ D, where D is an arbitrary distribution. What is the distribution F(X) where F is the CDF of X?

32. Describe what a moment generating function (MGF) is. Derive the MGF for a normally distributed random variable X.

33. Say you have N independent and identically distributed draws of an exponential random variable. What is the best estimator for the parameter X?

34. Assume that log X ~ N(0, 1). What is the expectation of X?

35. Say you have two distinct subsets of a dataset for which you know their means and standard deviations. How do you calculate the blended mean and standard deviation of the total dataset? Can you extend it to K subsets?

36. Say we have two random variables X and Y. What does it mean for X and Y to be independent? What about uncorrelated? Give an example where X and Y are uncorrelated but not independent.

37. Say we have X ~ Uniform(-1, 1) and Y = 2. What is the covariance of X and Y?

38. How do you uniformly sample points at random from a circle with radius R?

39. Say you continually sample from some i.i.d. uniformly distributed (0, 1) random variables until the sum of the variables exceeds 1. How many samples do you expect to make?


## Machine Learning

### Easy
1. Say you are building a binary classifier for an unbalanced dataset. How do you handle this situation?

2. What are some differences you would expect in a model that minimizes squared error versus a model that minimizes absolute error?

3. When performing K-means clustering, how do you choose k?

4. How can you make your models more robust to outliers?

5. Say that you are running a multiple linear regression and that you have reason to believe that several of the predictors are correlated. How will the results be affected?

6. Describe the motivation behind random forests.

7. Given a large dataset of payment transactions, how would you deal with missing values?

8. What are some ways you might improve your model if logistic regression is unsatisfactory?

9. Say you were running a linear regression but you accidentally duplicated every data point. What happens to your beta coefficient?

10. Compare and contrast gradient boosting and random forests.

11. Do you have enough training data to create an accurate ETA model based on 10,000 deliveries?


### Medium
12. How would you supply reasons for loan rejection in a binary classification model?

13. How would you identify synonyms in a large corpus of words?

14. What is the bias-variance tradeoff?

15. Define the cross-validation process.

16. How would you build a lead scoring algorithm?

17. How would you approach creating a music recommendation algorithm?

18. Define what it means for a function to be convex.

19. Explain information gain and entropy in decision trees.

20. What is L1 and L2 regularization?

21. Describe gradient descent.

22. How would the ROC curve change if you take the square root of each application's score?

23. What is the entropy of X?

24. How would you build a model to calculate a customer's propensity to buy a particular item?

25. Compare Gaussian Naive Bayes and logistic regression.


### Hard
26. What loss function is used in k-means clustering?

27. Describe the kernel trick in SVMs.

28. What are your best guesses for the parameters of a Gaussian distribution?

29. Describe the model setup for a Gaussian mixture model (GMM) for anomaly detection.

30. Walk me through how you'd build a model to predict whether a Robinhood user will churn.

31. Show that maximizing the likelihood is equivalent to minimizing the sum of the squared residuals in linear regression.

32. Describe the idea behind Principle Components Analysis (PCA).

33. Describe the model formulation behind logistic regression.

34. How would you approach creating a music recommendation algorithm for Discover Weekly?

35. Derive the variance-covariance matrix of the least squares parameter estimates.


## SQL

### Easy Problems

1. **Facebook**: Write a query to get the click-through rate per app in 2019.
   - Table: `events`
   - Columns: `app_id (integer), event_id (string: "impression", "click"), timestamp (datetime)`

2. **Robinhood**: Write a query to list the top three cities that had the most number of completed orders.
   - Table: `trades`
   - Columns: `order_id (integer), user_id (integer), price (float), quantity (integer), status (string: "complete", "cancelled"), timestamp (datetime)`
   - Table: `users`
   - Columns: `user_id (integer), email (string), signup_date (datetime)`

3. **New York Times**: Write a query to compare the viewership on laptops versus mobile devices.
   - Table: `viewership`
   - Columns: `user_id (integer), device_type (string), view_time (datetime)`

4. **Amazon**: Write a query to calculate the cumulative spend so far by date for each product over time in chronological order.
   - Table: `total_transactions`
   - Columns: `product_id (string), spend (float), transaction_date (datetime)`

5. **eBay**: Write a query to obtain the names of the ten customers who have ordered the highest number of products among those customers who have spent at least $1000 total.
   - Table: `user_transactions`
   - Columns: `transaction_id (integer), user_id (integer), spend (float), transaction_date (datetime)`

6. **Twitter**: Write a query to obtain a histogram of tweets posted per user in 2020.
   - Table: `tweets`
   - Columns: `tweet_id (integer), user_id (integer), msg (string), tweet_date (datetime)`

7. **Stitch Fix**: Write a query to obtain the number of people who purchased at least one or more of the same product on multiple days.
   - Table: `purchases`
   - Columns: `purchase_id (integer), user_id (integer), product_id (integer), quantity (integer), price (float), purchase_time (datetime)`

8. **LinkedIn**: Write a query to get the total number of duplicate job listings.
   - Table: `job_listings`
   - Columns: `job_id (integer), company_id (integer), title (string), description (string), post_date (datetime)`

9. **Etsy**: Write a query to obtain a list of customers whose first transaction was valued at $30 or more.
   - Table: `user_transactions`
   - Columns: `transaction_id (integer), product_id (integer), user_id (integer), spend (float), transaction_date (datetime)`

10. **Twitter**: Calculate the 7-day rolling average of tweets by each user for every day.
    - Table: `tweets`
    - Columns: `msg (string), user_id (integer), tweet_date (datetime)`

11. **Uber**: Write a query to obtain the third transaction of every user.
    - Table: `transactions`
    - Columns: `user_id (integer), spend (float), transaction_date (datetime)`

12. **Amazon**: Identify the top three highest-grossing categories in 2020.
    - Table: `product_spend`
    - Columns: `transaction_id (integer), category (integer), product_id (integer), user_id (integer), spend (float), transaction_date (datetime)`

13. **Walmart**: Write a query to obtain the number of users who made a purchase and the total number of products bought for each transaction date.
    - Table: `user_transactions`
    - Columns: `transaction_id (integer), user_id (integer), spend (float), transaction_date (datetime)`

14. **Facebook**: What is a database view? What are some advantages views have over tables?

15. **Expedia**: How would your decision to create indices be affected if most of the queries made were UPDATEs, INSERTs, DELETEs versus mostly SELECTs and JOINs?

16. **Microsoft**: What is a primary key? What characteristics does a good primary key have?

17. **Amazon**: Describe some advantages and disadvantages of relational databases vs. NoSQL.

18. **Capital One**: Describe the steps in the shuffle operator's algorithm for a MapReduce job, where the input is a dataset and the output is a randomly ordered version of that dataset.

19. **Amazon**: Name one major similarity between the WHERE clause and the HAVING clause in SQL.

20. **KPMG**: Describe what a foreign key is and how it relates to a primary key.

21. **Microsoft**: Describe what a clustered index and a non-clustered index are. Compare and contrast the two.

### Medium Problems

22. **Twitter**: Write a query to count existing users on 2021-01-01 that did not follow any topic in the 100 most popular topics on that day.
   - Table: `user_topics`
   - Columns: `user_id (integer), topic_id (integer), follow_date (datetime)`
   - Table: `topic_rankings`
   - Columns: `topic_id (integer), ranking (integer), ranking_date (datetime)`

23. **Facebook**: Write a query to obtain active user retention by month. An active user is defined as someone who took an action (sign-in, like, or comment) in the current month.
   - Table: `user_actions`
   - Columns: `user_id (integer), event_id (string: "sign-in", "like", "comment"), timestamp (datetime)`

24. **Twitter**: Write a query that ranks users according to their total session durations for each session type between the start date (2021-01-01) and the end date (2021-02-01).
   - Table: `sessions`
   - Columns: `session_id (integer), user_id (integer), session_type (string), duration (integer), start_time (datetime)`

25. **Snapchat**: Write a query to obtain a breakdown of the time spent sending vs. opening snaps for each of the different age groups.
   - Table: `activities`
   - Columns: `activity_id (integer), user_id (integer), activity_type (string: 'send', 'open'), time_spent (float), activity_date (datetime)`
   - Table: `age_breakdown`
   - Columns: `user_id (integer), age_bucket (string)`

26. **Fiverr**: Write a query to obtain the user session that is concurrent with the largest number of other user sessions.
   - Table: `sessions`
   - Columns: `session_id (integer), start_time (datetime), end_time (datetime)`

27. **Yelp**: Write a query to obtain the number and percentage of businesses that are top-rated.
   - Table: `reviews`
   - Columns: `business_id (integer), user_id (integer), review_text (string), review_stars (integer), review_date (datetime)`

28. **Google**: Write a query to obtain the sum of the odd-numbered measurements and the sum of the even-numbered measurements by date.
   - Table: `measurements`
   - Columns: `measurement_id (integer), measurement_value (float), measurement_time (datetime)`

<i>Nick Singh and Kevin Huo,</i> "Ace the Data Science Interview: 201 Real Interview Questions Asked By FAANG, Tech Startups, & Wall Street", ISBN: 9780578973838, Available on Amazon: https://www.amazon.com/Ace-Data-Science-Interview-Questions/dp/0578973839
