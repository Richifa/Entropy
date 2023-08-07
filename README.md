
# ![maxresdefault](https://github.com/Richifa/Entropy/assets/67483410/e8a9014e-fd54-4c0f-b53c-9759ee1d02e7)
Entropy
What Is Cross-Entropy?
Cross-entropy is a measure of the difference between two probability distributions for a given random variable or set of events.

You might recall that information quantifies the number of bits required to encode and transmit an event. Lower probability events have more information, higher probability events have less information.

In information theory, we like to describe the “surprise” of an event. An event is more surprising the less likely it is, meaning it contains more information.

Low Probability Event (surprising): More information.
Higher Probability Event (unsurprising): Less information.
Information h(x) can be calculated for an event x, given the probability of the event P(x) as follows:

h(x) = -log(P(x))
Entropy is the number of bits required to transmit a randomly selected event from a probability distribution. A skewed distribution has a low entropy, whereas a distribution where events have equal probability has a larger entropy.

A skewed probability distribution has less “surprise” and in turn a low entropy because likely events dominate. Balanced distribution are more surprising and turn have higher entropy because events are equally likely.

Skewed Probability Distribution (unsurprising): Low entropy.
Balanced Probability Distribution (surprising): High entropy.
Entropy H(x) can be calculated for a random variable with a set of x in X discrete states discrete states and their probability P(x) as follows:

H(X) = – sum x in X P(x) * log(P(x))
If you would like to know more about calculating information for events and entropy for distributions see this tutorial:

A Gentle Introduction to Information Entropy
Cross-entropy builds upon the idea of entropy from information theory and calculates the number of bits required to represent or transmit an average event from one distribution compared to another distribution.

… the cross entropy is the average number of bits needed to encode data coming from a source with distribution p when we use model q …



The intuition for this definition comes if we consider a target or underlying probability distribution P and an approximation of the target distribution Q, then the cross-entropy of Q from P is the number of additional bits to represent an event using Q instead of P.

The cross-entropy between two probability distributions, such as Q from P, can be stated formally as:

H(P, Q)
Where H() is the cross-entropy function, P may be the target distribution and Q is the approximation of the target distribution.

Cross-entropy can be calculated using the probabilities of the events from P and Q, as follows:

H(P, Q) = – sum x in X P(x) * log(Q(x))
Where P(x) is the probability of the event x in P, Q(x) is the probability of event x in Q and log is the base-2 logarithm, meaning that the results are in bits. If the base-e or natural logarithm is used instead, the result will have the units called nats.

This calculation is for discrete probability distributions, although a similar calculation can be used for continuous probability distributions using the integral across the events instead of the sum.

The result will be a positive number measured in bits and will be equal to the entropy of the distribution if the two probability distributions are identical.
