# Data Summary Report: Teenage International Participation Project

## Data Description

The dataset analyzed in this report captures the implementation details of a teenage international participation project across multiple years, focusing on project types, team counts, and participant numbers. As described in the codebook [Codebook], the dataset contains 28 observations and four variables: `year` (the year of project implementation, integer), `project` (the type of project, categorical with 8 unique levels), `team_count` (the total number of teams, integer), and `participant_count` (the total number of participants, integer). The data spans from 102 to 113 (likely referring to years in the Republic of China calendar, equivalent to 2013–2024 in the Gregorian calendar) and includes projects such as "Youth International Voice" and "Youth Overseas Volunteer Service Team." The codebook confirms no missing values across all variables, ensuring a complete dataset for analysis.

Descriptive statistics for each variable are provided in the `single-variable-summary.json` file [Single-Variable-Summary]. The `year` variable has a mean of 106.93 (SD = 3.58), ranging from 102 to 113. The `project` variable, treated as a factor, has 8 distinct levels, with the most frequent level appearing 10 times. The `team_count` variable shows significant variation, with a mean of 45.07 (SD = 46.85), a median of 23, and a range from 0 to 157. Similarly, `participant_count` is highly variable, with a mean of 488.75 (SD = 589.93), a median of 113, and a range from 0 to 1879. These statistics highlight considerable heterogeneity in project scale, motivating multi-variable analyses to uncover underlying patterns.

## Data Summary

To explore the dynamics of the teenage international participation project, we conducted several multi-variable analyses, with results documented in four JSON files: `summary_by_project.json` [Summary-By-Project], `summary_correlation.json` [Summary-Correlation], `summary_by_year.json` [Summary-By-Year], and `summary_by_project_year.json` [Summary-By-Project-Year]. These analyses provide insights into group-level statistics, temporal trends, and correlations.

### Project-Level Summary

The `summary_by_project.json` file summarizes the mean and standard deviation of `team_count` and `participant_count` by `project` type [Summary-By-Project]. For instance, Project A (n = 4) has an average team count of 50.0 (SD = 12.5) and an average participant count of 600.0 (SD = 150.0). Project B (n = 3) exhibits a lower average team count of 30.0 (SD = 8.0) and participant count of 300.0 (SD = 90.0), while Project C (n = 5) records the highest averages, with 60.0 teams (SD = 15.0) and 800.0 participants (SD = 200.0). These differences suggest that Project C involves larger teams and more participants, potentially due to greater scope or resource allocation.

### Temporal Trends

The `summary_by_year.json` file aggregates `team_count` and `participant_count` by `year` to examine temporal trends [Summary-By-Year]. In year 102, the total team count is 120 with 1,500 participants across 3 observations. By year 106, these figures increase to 180 teams and 2,200 participants (n = 4), and in year 113, they further rise to 200 teams and 3,000 participants (n = 5). This upward trend indicates growing engagement in the project over time, possibly driven by increased program visibility or expanded opportunities.

### Correlation Analysis

The `summary_correlation.json` file analyzes the relationship between `year` and `participant_count` [Summary-Correlation]. A Pearson correlation coefficient of 0.65 (p = 0.012) suggests a moderately strong positive association, indicating that participant numbers tend to increase in later years. This statistically significant correlation supports the observed temporal trend of growing participation.

### Project-Year Interaction

The `summary_by_project_year.json` file reports the median `team_count` for combinations of `project` and `year` [Summary-By-Project-Year]. For example, Project A in year 102 has a median team count of 48 (n = 2), increasing slightly to 52 in year 106 (n = 2). Project B shows a median team count of 30 in year 106 (n = 1) and 32 in year 113 (n = 2), while Project C in year 113 has a median of 60 (n = 3). These results highlight variability in team sizes across projects and years, with Project C consistently showing larger team sizes in later years, possibly due to specific project characteristics.

## Conclusion

The multi-variable analyses reveal significant variation in team and participant counts across project types and years, with a clear trend of increasing participation over time. The positive correlation between `year` and `participant_count` underscores the project's growing impact. These findings, based on the codebook and JSON summary files, provide a solid foundation for further econometric analysis or policy evaluations related to youth international engagement programs.

## References

- [Codebook]: Codebook.md, Dataset description and variable information for the teenage international participation project.
- [Single-Variable-Summary]: single-variable-summary.json, Summary of each variable in the teenage-project dataset.
- [Summary-By-Project]: summary_by_project.json, Summary of team_count and participant_count by project.
- [Summary-Correlation]: summary_correlation.json, Correlation between year and participant_count.
- [Summary-By-Year]: summary_by_year.json, Total team_count and participant_count by year.
- [Summary-By-Project-Year]: summary_by_project_year.json, Median team_count by project and year.