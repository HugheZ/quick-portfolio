# ML and AI Projects

Although I'm new to ML and AI applications, I'm learning new models for application in business and consumer life. My primary interest is in NLP, but other applications, like market basket analysis, are also interesting.

## Dota 2 Wins by Team Composition and Pairs, Comparing Two Logistic Regression Implementations

This project used two black-box logistic regressions in MatLab, glmfit and lassoglm, to predict win likelihood in Dota 2 games by team composition and by pairs on a team. Both models were trained from a dataset taken from the UCI machine learning database, found [here](https://archive.ics.uci.edu/ml/datasets/Dota2+Games+Results). 

Our resulting models were only slightly better than random guessing (50% accuracy), but one model tended towards pessimism while the other tended towards optimism for teams. This result made sense, since player, skill, opposing composition, and latency were not factored into the model. However, that we were able to improve over guessing by simply observing which of the 117 heroes are on a 5-person team is noteworthy. Similarly, we found out more about the playerbase by analyzing the game statistics.

[Slideshow can be found here](https://docs.google.com/presentation/d/1CNnkYb4wQc5Dp6Y48MPp7x1WoInAb9u2sAGKoHoKkxw/edit?usp=sharing)

## Markov Model Movie Scripts

Although not cutting-edge, below are the results of running a hand-implemented Markov model on movie scripts:
* [Bee Movie](markov/beeMovie.md)
* [Shrek](markov/shrek.md)

## Markov Model with Mounted Topic Analysis

This semester, I will have the opportunity to take part in a research project in which I will mount topic analysis onto a higher-dimension Markov model with the hopes of improving coherence. The resulting model will be used to simulate character conversations on a given primer topic. Further application of character datatypes, grammar trees, and sentiment analysis may be out of scope but could be interesting.

This section will be updated with a link or removal pending project approval.
