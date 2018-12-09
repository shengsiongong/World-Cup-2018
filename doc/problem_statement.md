Overview and Motivation
******************

While soccer is one of the most popular sports in the world, its analytics is lackluster in comparison to other popular sports such as baseball, American football, hockey, and basketball. This is due to the fact that aside from the World Cup, international teams don’t play each other very frequently. Therefore, there is a lack of high quality data that can be immediately fed into models to perform predictions.

The World Cup is composed of 64 matches in total - 48 matches in group stages and 16 matches in knockout (15 + 1 for third place). We plan to predict the outcome of each of the 64 matches independently instead of predicting which teams proceed in each round. This strategy allows our results to be comparable across models. By framing the problem in this way, we plan to approach this problem as a classification problem. Each game can be treated as a multi-class classification problem, where there are three outcomes: win for the home team (or team 1, indicated with 1), win for the away team (or team 2, indicated with -1), or a draw (indicated with 0). In the case of knockouts, we limit the outcome to: win for the home team (or team 1), win for the away team (or team 2), as draws are not allowed.

To validate how accurate FIFA rankings are, we aim to use a baseline model that leverages FIFA rankings and some other simple predictors to predict the World Cup results. We plan to create a more advanced model, without relying on FIFA rankings but instead based on features collected and engineered by us that are proven to be relevant in the initial EDA. Ultimately, our analysis attempts to create a model that can predict the World Cup results as accurately as possible, while offering an insight into the features helpful in soccer analytics.
