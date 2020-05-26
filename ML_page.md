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

## [Markov Model with Mounted Topic Analysis](https://gist.github.com/homealone944/7c886a3a8d29ca42d4a98a70cabae917)

This semester, I will be researching Markov Models with a potential mounted topic analysis to improve the coherency of low-level Markov Models. In the face of developing long-term memory systems, like [GPT-2.0](https://github.com/openai/gpt-2), Microsoft's new [DeepSpeed](https://github.com/microsoft/DeepSpeed) library and [Transformer-based model](https://venturebeat.com/2020/02/10/microsoft-trains-worlds-largest-transformer-language-model/), and Google's latest DeepMind [PG19 model](https://github.com/deepmind/pg19), Markov Models seem a bit out of place for enterprise-level text generation. 

This research project will seek to balance Markov Models with topic analysis to improve coherency using Dracula's letters from Jonathan Harker and Mina Harker. The expected result will be a coherent letter to and from each actor with a lightweight model. The generated text will not be as coherent as the enterprise models above, nor will it have the same memory, but it could still be useful for systems without access to strong computing hardware. Additionally, our chosen corpus is small enough to warrant further study for small models.

We will generate letters first by a single-level Markov Model, then through second-level and bigrams, and finally by integrating topic analysis and comparing it to a Recurrent Neural Network. Current results show our Markov Models to be more coherent than RNN models. We believe this to be the case due to the size of the dataset, as nerual nets require large sets to train off of. Below are resulting sentences from each stage:

1st level:
> Jon:  We traveled night , " Look ! Me and I had not been seen the bloated face with a monster . 

Bigrams:
> Jon: I who marked Galatz .\_The other dogs_, who_had served his coat leisurely and neck of_the strange land .\_He certainly did so having just such_a stench would_have to face I_had to rush 

2nd Level and Bigrams: 
> Jon: Here_I am noble .\_I am_a Boyar .\_The common people know me_, and_I could_see that_his forehead was covered_with great beads of perspiration .\_Mina opened her_eyes ,\_but she\_did

2nd Level and Bigrams with Mounted LDA topic analysis and grouping:
> Jon: As I leaned from_the window and begin to crawl down the_castle wall over_the dreadful abyss , face down with his cloak spreading out around him like great wings .

TPU accelerated RNN:
> Jon: One of them aboot their return, or the window or some later I felt so many moment. He said, "Juint more than usual instructions were stream shakes, then a might not wait for myself. The world was a love back to take the lock, my friend. Nook!

Even with this simple uncleaned output, the Markov Models are performing better than the neural net. Further introduction of knowledge bleeding from other texts and weighting responses could prove to be a better model for smaller inputs.


## [Expectus, a Joustus AI](https://github.com/HugheZ/Expectus)
Expectus is an AI implemented to play Joustus, a card minigame from Yacht Club Game's Shovel Knight: King of Cards. Since a deck and hand game structure removes the perfect information requirement for minimax, we used expectiminimax, a minimax implementation for nondeterministic games. This AI currently forms a strategy for the basic single-arrow push cards and 3x3 board structure. The AI runs on top of a basic unity version of Joustus and supports player-vs-AI, player-vs-player, and AI-vs-AI games.

Additionally, implementing alpha-beta pruning saw a drastic reduction in time despite only being able to calculate out to 5-ply games (including chance nodes as a ply). This culminated in a 30x faster response speed than without pruning. 
