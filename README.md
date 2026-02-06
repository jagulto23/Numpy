(GENERATIVE AI)

I used generative AI as a learning and development tool to support this project. Generative AI was used to help explain concepts related to basketball analytics, NumPy, and pandas, and to clarify how to structure calculations for player performance metrics. It also assisted in simplifying and refactoring code, understanding while still meeting the project requirements, such as loading data into NumPy ndarrays and performing array-based data manipulation.

In addition, generative AI was used to help write clear explanations of the code and summarize the purpose and functionality of different sections of the project. Rather than generating the dataset or final results, the AI served as a guide for understanding syntax, debugging logic, improving readability, and ensuring the calculations aligned with the project objectives. All final implementation decisions, code execution, and interpretation of results were completed by me, with generative AI acting as a supportive resource similar to a reference tool. I was struggling about installing kaggle, pandas, and numpy but generative AI helped me with my struggles. I also had a few errors like my file won't run and made a simple mistake by missing a parenthesis.



# Numpy
This analysis evaluates player performance by calculating field goal, three-point, and free throw accuracy, average points per minute, overall shooting accuracy, and average blocks and steals per game for each player in each season.

The purpose of this project is to analyze basketball player performance across seasons using real-world data and efficient numerical computation. By aggregating raw game statistics by player and season, the project calculates meaningful performance metrics that describe scoring efficiency, productivity, and defensive impact. These metrics help compare players fairly across different seasons and playing time, supporting data-driven evaluation commonly used in modern sports analytics.

The project is designed procedurally rather than with custom classes, prioritizing clarity, performance, and alignment with the dataset’s tabular structure. Pandas is used for data loading, grouping, and result presentation, while NumPy handles numerical computation. Key attributes include aggregated statistics such as games played (GP), minutes (MIN), shooting makes and attempts, points, steals, and blocks. Metrics are computed through reusable functions like safe_divide, which prevents division-by-zero errors by returning NaN values where data is insufficient. This design choice improves robustness and avoids misleading results.

Each calculated metric—shooting accuracies, points per minute, points per game, blocks per game, and steals per game—is written back to the DataFrame to maintain a single, organized results table. A dictionary-driven approach is used to generate Top 100 rankings for each metric, reducing repetition and improving scalability. Limitations include reliance on season-level aggregates (not per-game variability), exclusion of advanced metrics, and dependency on data completeness and accuracy within the Kaggle dataset.
