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

This semester, I will be researching Markov Models with a potential mounted topic analysis to improve the coherency of low-level Markov Models. In the face of developing long-term memory systems, like [GPT-2.0](https://github.com/openai/gpt-2), Microsoft's new [DeepSpeed](https://venturebeat.com/2020/02/10/microsoft-trains-worlds-largest-transformer-language-model/) library and [Transformer-based model](https://venturebeat.com/2020/02/10/microsoft-trains-worlds-largest-transformer-language-model/), and Google's latest DeepMind [PG19 model] (https://github.com/deepmind/pg19), Markov Models seem a bit out of place for enterprise-level text generation. 

This research project will seek to balance Markov Models with topic analysis to improve coherency using Dracula's letters from Jonathan Harker and Mina Harker. The expected result will be a coherent letter to and from each actor with a lightweight model. The generated text will not be as coherent as the enterprise models above, nor will it have the same memory, but it could still be useful for systems without access to strong computing hardware. This page will be updated with code, results, and examples once our models are trained and sufficient letters are generated.

Initially, the letters will be generated with 1st and 2nd level Markov Models. Then, we will compare them to models with mounted topic analysis.
