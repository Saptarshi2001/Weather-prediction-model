Weather-Prediction-Model is a final year research project that involves building a machine learning model for weather prediction.It uses the associative rule mining algorithm for determining the weather of a particular place.

 

# Requirements
- Python 3.6 or higher
- Numpy

# Getting started
- clone the repository `git clone https://github.com//Saptarshi2001/LocalSocial.git`
- Set up an account at Google collab
- Upload the csv file from your local device
- Write out the name of the file over here - ` file_path = 'filename.csv' `
- Run the code
- The code gives the result by giving <br>
i- Support along with the support graph <br>
ii- Confidence along with the confidence graph <br>
iii- Lift along with the lift graph


# Process
- Our research explores the application of association rule mining techniques in weather prediction,
aiming to bridge the research gap in leveraging data mining approaches for meteorological
forecasting. <br>
- Historical weather data is analyzed using the Apriori algorithm to extract frequent
itemsets and association rules, revealing hidden patterns and dependencies among weather
variables. These discovered patterns serve as the foundation for developing predictive models for
weather forecasting, potentially enhancing the accuracy and reliability of existing methods. Through a
comprehensive research methodology encompassing data preprocessing, association rule mining,
model development, and validation, this study offers insights into the feasibility and effectiveness of
association rule mining in improving weather prediction capabilities.<br>
- Association rule mining is a technique used to identify patterns in large data sets. It involves finding
relationships between variables in the data and using those relationships to make predictions or decisions.
The goal of association rule mining is to uncover rules that describe the relationships between different
items in the data set.<br>
- In data mining, Support refers to the relative frequency of an item set in a dataset.<br>
In data mining, Confidence is a measure of the reliability or support for a given association rule. It is
defined as the proportion of cases in which the association rule holds true, or in other words, the
percentage of times that the items in the antecedent (the “if” part of the rule) appear in the same
transaction as the items in the consequent (the “then” part of the rule).<br>

- lift is a measure of the performance of a targeting model (association rule) at predicting or classifying cases
as having an enhanced response (with respect to the population as a whole), measured against a random
choice targeting model. A targeting model is doing a good job if the response within the target (T) is much
better than the baseline (B) average for the population as a whole. Lift is simply the ratio of these values:
target response divided by average response. Mathematically,
Lift=P(T|B)/P(T)=P(T^B)/P(T) P(B). <br>



# Problem Analysis
- Despite advancements in weather forecasting models, there exists a significant research gap in
leveraging association rule mining techniques for weather prediction. Traditional weather
forecasting methods primarily rely on statistical and numerical models, which may overlook subtle
but meaningful relationships between weather variables. 
- Association rule mining offers a novel approach to uncovering hidden patterns and dependencies in weather data, potentially leading to
more accurate and reliable forecasting models.
- However, limited research has been conducted on the application of association rule mining
specifically for weather prediction. Existing studies often focus on other domains, such as market
basket analysis and healthcare, neglecting the potential of this approach in meteorology. By
addressing this research gap and exploring the feasibility of association rule mining in weather
prediction, we can potentially revolutionize the field of meteorology and enhance our ability to
forecast weather events with greater precision and confidence.


# Review of Literature

- Abd Elaty AA, Salem R, Elkader HA(2018) Efficient association rules mining from streaming data with
a fault tolerance. In: 2018 13th international conference on computer engineering and systems
(ICCES), pp 627–632 .
- Abu Daher L, Elkabani I, Zantout R (2018) Identifying influential users on twitter: a case study from
Paris attacks. Appl Math Inf Sci 12:1021–1032.
- Acosta ME, Palaoag TD(2019) Characterization of disaster related tweets according to its urgency: a
pattern recognition. In: Proceedings of the 2019 5th international conference on computing and
artificial intelligence, pp 30–37
- Adedoyin-Olowe M, Gaber M, Stahl F (2014) A survey of data mining techniques for social network
analysis. J Data Min Digit Humanit
- Atsa’am DD, Wario R (2021) Association rules on the Covid-19 variants of concern to guide choices
of tourism destinations. Current Issues in Tourism, pp 1–5
- Agrawal R, Imieliński T, Swami A (1993) Mining association rules between sets of items in large
databases. ACM SIGMOD Rec 22:207–216 (ACM)

# Formulation/Algorithm

- The program starts by reading the dataset from a CSV file. Each row in
the CSV represents a transaction, and each column represents an item.
The frequent itemsets and association rules are printed to the console.
Lastly, a bar graph is plotted to visualize the association rules based on
a specified metric (in this case, confidence).

- Initialization: Initially, the algorithm scans the dataset to
identify individual items and create candidate itemsets.
- Generate Candidate Itemsets: Using the candidate itemsets,
the algorithm iteratively generates larger candidate itemsets
by combining existing itemsets. It generates candidate kitemsets from frequent (k-1)-itemsets.
- Prune Candidate Itemsets: Pruning is done to eliminate
candidate itemsets that have infrequent subsets. If a candidate
itemset does not meet the minimum support threshold, it is
pruned.
- Count Support: The algorithm counts the support for each
candidate itemset by scanning the dataset again.
- Repeat: Steps 2 and 3 are repeated until no new frequent
- For each frequent itemset found by the Apriori algorithm,
association rules are generated.
- Each frequent itemset is split into two parts: antecedent and
consequent.
- Confidence, lift, conviction, and interestingness measures are
calculated for each rule.
- Rules with confidence greater than or equal to the minimum
confidence threshold are selected.
- The frequent itemsets and association rules are printed to the console.
- Lastly, a bar graph is plotted to visualize the association rules based on
a specified metric (in this case, confidence).


# Further Improvements

- While the code does run perfectly,it lacks a lot when it comes to performance
- Multithreading might solve this and will reduce the processing time of it

