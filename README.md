# smarkz01



<h2> BAYESIAN LEARNING</h2>(https://docs.google.com/document/d/1RTMat4DHvvAurDg_bFXoxL8oUjQqEtx83jDjaYFwk4g/edit?usp=sharing)


<h2>What is Bayesian Learning ?</h2>


Bayesian Learning deals with probabilistic methods mainly including bayes theorem where we are unable to use frequentist statistics

LET'S TAKE THE EXAMPLE OF A COIN TOSS Experiment;

When we flip a coin, there are two possible outcomes — heads or tails. Of course, there is a third rare possibility where the coin balances on its edge without falling onto either side, which we assume is not a possible outcome of the coin flip for our discussion. We conduct a series of coin flips and record our observations i.e. the number of the heads (or tails) observed for a certain number of coin flips. In this experiment, we are trying to determine the fairness of the coin, using the number of heads (or tails) that we observe using Frequentist statistics

<h2>What is Frequentist statistics?</h2>


Testing whether a hypothesis is true or false by calculating the probability of an event in a prolonged experiment is known as frequentist statistics. As such, determining the fairness of a coin by using the probability of observing the heads is an example of frequentist statistics (a.k.a. frequentist approach).

Once we have conducted a sufficient number of coin flip trials, we can determine the frequency or the probability of observing the heads (or tails). If we observed heads and tails with equal frequencies or the probability of observing heads (or tails) is_ 0.5_, then it can be established that the coin is a fair coin. Failing that, it is a biased coin. Let's denote _p_ as the probability of observing the heads. Consequently, as the quantity that _p_ deviates from _0.5_ indicates how biased the coin is, _p_ can be considered as the degree-of-fairness of the coin.

we flip the coin _10_ times, we observe the heads 6 times. Therefore, the _p_ is _0.6_ . Hence, according to frequencies statistics, the coin is a biased coin — which opposes our assumption of a fair coin.Lets say we do the experiment 100 times, we observe heads _55_ times, which results in a different _p_ with _0.55_.

We cannot find out the exact answers to the first is a fair coin.So, we see frequentist statistics is highly dependent on frequency and shows a lot of variance .  three questions using frequentist statistics. We may assume that the true value of _p_ is closer to _0.55_ than _0.6_ because the former is computed using observations from a considerable number of trials compared to what we used to compute the latter. Yet there is no way of confirming that hypothesis. However, if we further increase the number of trials, we may get a different probability from both of the above values for observing the heads and eventually, we may even discover that the coin 

.

<h2>Basic Terminology</h2>




*   [Random variable (Stochastic variable)](https://en.wikipedia.org/wiki/Random_variable) — In statistics, the random variable is a variable whose possible values are a result of a random event. Therefore, each possible value of a random variable has some probability attached to it to represent the likelihood of those values.
*   [Probability distribution](https://en.wikipedia.org/wiki/Probability_distribution) — The function that defines the probability of different outcomes/values of a random variable. The continuous probability distributions are described using <span style="text-decoration:underline;">probability density functions </span>whereas discrete probability distributions can be represented using <span style="text-decoration:underline;">probability mass functions.</span>
*   [Conditional probability](https://en.wikipedia.org/wiki/Conditional_probability) — This is a measure of probability P(A|B) of an event A given that another event B has occurred.
*   [Joint probability distribution](https://en.wikipedia.org/wiki/Joint_probability_distribution) -- Joint probability is a statistical measure that calculates the likelihood of two events occurring together and at the same point in time. Joint probability is the probability of event A occurring at the same time that event X occurs.

     Notation for joint probability can take a few different forms. The following formula represents the probability of events intersection:​


 P (X⋂Y)    **where: **X,Y=Two different events that intersectP(X and Y),P(XY)=The joint probability of X and Y

​



 <span style="text-decoration:underline;">Resources:</span>

[Python Implementation](https://colab.research.google.com/drive/16wWtsr4mBkQu-haAvXfrEokVBePrVqxV?usp=sharing)


                	

                       

     
