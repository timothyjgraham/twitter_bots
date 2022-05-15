# Twitter bots

## Bot analysis of 5000 randomly sampled tweets from the streaming API endpoint

In this repository you will find:

1. CSV file with account Botometer scores and user IDs for 5000 random Twitter accounts.

Botometer is a bot detection system that has been peer-reviewed and scientifically validated: https://botometer.osome.iu.edu/faq.

The bot scores are the Completely Automated Probability (CAP) metric, defined as the probability that an account with this score or greater is controlled by software, i.e., is a bot. A score is 0 is almost certainly human; a score of 1 is almost certainly a bot.

I used a threshold of 0.95 to make a binary classification of accounts, so if an account has a CAP score greater than 0.95 then we classify it as a bot. So we establish a false positive rate of 5%, which seems fairly reasonable and is suggested by the Botometer authors. 
