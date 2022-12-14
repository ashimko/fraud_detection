# Fraud detection homework [OTUS MlOps course](https://otus.ru/lessons/ml-bigdata/)
## Project goals
* Decrease share of fraudelent operations by 7% within a year.

## Project metrics
A fraud detection system aims at optimizing two conflicting goals. On the one hand, the system should maximize the detection of fraudulent transactions, a metric known as recall. On the other hand, it should also minimize the number of false positives, that is, the number of genuine transactions which are incorrectly predicted as frauds. Unless a perfect classifier can be designed, maximizing the recall comes at a cost in terms of false positives. The cost structure of a fraud detection system is however complex, if not impossible, to determine.

A common approach to circumvent this conflicting goal is to assess the recall and false positive rates for all possible decision thresholds. The resulting function is the **Receiving Operating Characteristic (ROC) curve**. The area under the ROC curve (known as **AUC ROC**) is the most widely used metric to assess the performance of fraud detection systems. This chapter highlighted that the AUC ROC is however poorly adapted to class imbalanced problems such as fraud detection. Two other metrics, the **Average Precision (AP)**, and the daily **Card Precision top- (CP@k)** were motivated to better characterize the performances of a Credit card fraud detection (CCFD).

**The AUC ROC, AP, and CP@k** are complementary. The AUC ROC reflects the accuracy of the detection system for all possible thresholds. The AP also reflects the accuracy of the detection system for all possible thresholds but gives more importance to regions of the decision thresholds where the precision remains high. Finally, the CP@k provides a more concrete metric for CCFD, by assessing the average daily precision of the system, assuming that a maximum of  cards can be checked daily by investigators.

**Due to their complementarity, we recommend assessing the performance of a fraud system by using these three performance measures.** (c) [fraud detection handbook](https://fraud-detection-handbook.github.io/fraud-detection-handbook/Chapter_4_PerformanceMetrics/Summary.html)
