# Vanguard Web Design A/B Testing

This project evaluates if Vanguard's new web design is more effective than the previous one based on specific Key Performance Indicators (KPIs). The assumption is that a more intuitive and modern User Interface (UI) could enhance the online experience for clients.

In this project, data from an A/B testing study lasting 100 days was analyzed to determine if the new website design is more user-friendly than the previous design.

## Workflow

1. **EDA & Data Cleaning**
2. **Explore Samples (Test & Control Group)**
3. **Calculate KPIs**
4. **Hypothesis Testing**
5. **Tableau Visualization:** https://public.tableau.com/app/profile/luna.tissera/viz/ab_testing_17157028006550/Historia1 

**Note:** You will find a jupyter notebook with the entire workflow.

## A/B Testing Process

The A/B testing process divided the company's customers into two representative groups:
- **Control Group**: Tested the old website design.
- **Test Group**: Tested the new website design.

## Datasets

- **Client Profiles**: Demographics such as age, gender, and account details.
- **Digital Footprints**: Detailed trace of client interactions online, divided into two parts.
- **Experiment Roster**: List of clients who were part of the experiment.

**Note**: You'll find the datasets in the `data` folder. The `raw_data` contains the original datasets, and `cleaned_data` contains the datasets after the cleaning process.

## Objective

**Key Question**: Would these changes encourage more clients to complete the process?

## KPIs

Three KPIs were defined to evaluate the success of the new design:

### 1. Completion Rate
The proportion of users who reach the final ‘confirm’ step.

- **Control**: 73.67%
- **Test**: 94.93%

With this result, we can assume that the new web design is more intuitive and user-friendly, making it easier for users to complete the process to the final confirmation step.

### 2. Error Rates
The frequency of users going back to a previous step, indicating confusion or errors.

- **Control**: 6.82%
- **Test**: 9.19%

The higher error rate for the test group (9.19%) compared to the control group (6.82%) suggests that there are aspects of the new design that may cause confusion or difficulty for users. This indicates a need for further optimization of the new design.

### 3. Time Spent on Each Step
The average duration users spend on each step.

The time spent by users in each step indicates that test users initially have a harder time starting but proceed through the process to completion. In contrast, control group users spend more time at the start but are less likely to finish the process.

## Hypothesis Testing

To determine if the difference in completion rates is statistically significant:

- **Null Hypothesis (H0)**: The completion rate for the Test group (new design) is equal to the Control group (old design).
- **Alternative Hypothesis (H1)**: The completion rate for the Test group (new design) is not equal to the Control group (old design).

Using a significance level of 0.05, the p-value was calculated to be 4.41. Since the significance value is greater than the p-value, we reject the null hypothesis and conclude that the completion rates for the Test and Control groups are significantly different.

## Conclusions

The new design shows promising results with a significantly higher completion rate and potentially improved efficiency in certain steps. However, it also has a slightly higher error rate, indicating areas for optimization. Further analysis and user feedback will be crucial for refining the new design.
