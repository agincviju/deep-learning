Experiment 2 – Outlier Detection using Z-score and IQR

1.Problem Statement The goal of this experiment is to identify outliers in a dataset using statistical methods. Outliers can significantly affect the performance of data analysis and machine learning models. This experiment applies two common techniques — Z-score and Interquartile Range (IQR) — to detect outliers in a given dataset.

2.Deep Learning Methods & Description Although this experiment focuses on statistical methods rather than deep learning, it is an important preprocessing step before applying deep learning models. The methods are: Z-score Method Calculates how many standard deviations a data point is from the mean. If the absolute value of the Z-score is above a certain threshold, the point is considered an outlier. IQR Method Uses the first quartile (Q1) and third quartile (Q3) to measure the spread of the middle 50% of data. Any point lying outside the range [Q1 - 1.5IQR, Q3 + 1.5IQR] is flagged as an outlier.

3.Methods Applied to Solve the Problem In this experiment: A dataset of 9 values was analyzed. Z-score method was applied with a threshold of 1 to find points far from the mean. IQR method was applied to find points beyond the whiskers in a boxplot. Both methods identified potential outliers for removal.

4.Results Detected Outliers (Z-score method): Values with |Z| > 1 were identified. Detected Outliers (IQR method): Values greater than Q3 + 1.5IQR or less than Q1 - 1.5IQR were flagged. Boxplot Visualization: Clearly shows the distribution and highlights the outliers.

5.Conclusion Outlier detection is crucial for improving the quality of datasets before applying machine learning or deep learning algorithms. In this experiment, both Z-score and IQR successfully identified the extreme values. Removing these values can lead to better model accuracy and reliability.
