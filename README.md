# smarkz01



<h2> BAYESIAN LEARNING</h2>


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



<p id="gdcalert1" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image1.jpg). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert2">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image1.jpg "image_tooltip")




<p id="gdcalert2" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image2.jpg). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert3">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image2.jpg "image_tooltip")




<p id="gdcalert3" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image3.jpg). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert4">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image3.jpg "image_tooltip")


<h2>Introduction to Bayesian Learning</h2>


Imagine a situation where your friend gives you a new coin and asks you the fairness of the coin (or the probability of observing heads) without even flipping the coin once. In fact, you are also aware that your friend has not made the coin biased. In general, you have seen that coins are fair, thus you expect the probability of observing heads is 0.5. In the absence of any such observations, you assert the fairness of the coin only using your past experiences or observations with coins.

Suppose that you are allowed to flip the coin 10 times in order to determine the fairness of the coin. Your observations from the experiment will fall under one of the following cases:



*   **Case 1**: observing _5_ heads and_ 5_ tails.
*   **Case 2**: observing _h_ heads and 10-_h _tails, where _h_ ≠ _10_−_h_.

If case 1 is observed, you are now more certain that the coin is a fair coin, and you will decide that the probability of observing heads is 0.5 with more confidence. If case 2 is observed, you can either:



1. Neglect your prior beliefs since now you have new data and decide the probability of observing heads is _h/10_ by solely depending on recent observations.
2. Adjust your belief accordingly to the value of _h_ that you have just observed, and decide the probability of observing heads using your recent observations.

The first method suggests that we use the frequentist method, where we omit our beliefs when making decisions. However, the second method seems to be more convenient because _10_ coins are insufficient to determine the fairness of a coin. Therefore, we can make better decisions by combining our recent observations and beliefs that we have gained through our past experiences. It is this thinking model that uses our most recent observations together with our beliefs or inclination for critical thinking that is known as Bayesian thinking.

Moreover, assume that your friend allows you to conduct another _10_ coin flips. Then, we can use these new observations to further update our beliefs. As we gain more data, we can incrementally update our beliefs increasing the certainty of our conclusions. This is known as incremental learning, where you update your knowledge incrementally with new evidence.

Bayesian learning comes into play on such occasions, where we are unable to use frequentist statistics due to the drawbacks that we have discussed above. We can use Bayesian learning to address all these drawbacks and even with additional capabilities (such as incremental updates of the posterior) when testing a hypothesis to estimate unknown parameters of a machine learning model. Bayesian learning uses Bayes' theorem to determine the conditional probability of a hypothesis given some evidence or observations.

<h2>Bayes' theorem</h2>


 Describes how the conditional probability of an event or a hypothesis can be computed using evidence and prior knowledge. It is similar to concluding that our code has no bugs given the evidence that it has passed all the test cases, including our prior belief that we have rarely observed any bugs in our code. However, this intuition goes beyond that simple hypothesis test where there are multiple events or hypotheses involved.

The Bayes' theorem is given by:



<p id="gdcalert4" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image4.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert5">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image4.png "image_tooltip")


Consider the hypothesis _θ_ and _X_ is the dataset AND  _θ_ and _X_ denote that our code is bug-free and passes all the test cases respectively.

**_P(θ)_** — Prior Probability is the probability of the hypothesis _θ _being true before applying the Bayes' theorem. Prior represents the beliefs that we have gained through past experience, which refers to either common sense or an outcome of Bayes' theorem for some past observations. For the example given, prior probability denotes the probability of observing no bugs in our code. However, since this is the first time we are applying Bayes' theorem, we have to decide the priors using other means (otherwise we could use the previous posterior as the new prior). Let us assume that it is very unlikely to find bugs in our code because rarely have we observed bugs in our code in the past. With our past experience of observing fewer bugs in our code, we can assign our prior _P(θ)_ with a higher probability. However, for now, let us assume that _P(θ) = p_.



*   **_P(X|θ)_** — Likelihood is the conditional probability of the evidence given a hypothesis. The likelihood is mainly related to our observations or the data we have. If it is given that our code is bug-free, then the probability of our code passing all test cases is given by the likelihood. Assuming we have implemented these test cases correctly, if no bug is presented in our code, then it should pass all the test cases. Therefore, the likelihood _P(X|θ)_ = 1.
*   **_P(X)_** — Evidence term denotes the probability of evidence or data. This can be expressed as a summation (or integral) of the probabilities of all possible hypotheses weighted by the likelihood of the same.

Therefore, we can write _P(X)_ as:



<p id="gdcalert5" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image5.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert6">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image5.png "image_tooltip")


ϴ is the set of all the hypotheses.

For the continuous _θ,_ we write _P(X)_ as an integration:

1) observing no bugs in our code or 2) observing a bug in our code. Therefore we can denotes evidence as follows:



<p id="gdcalert6" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image6.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert7">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image6.png "image_tooltip")


<p id="gdcalert7" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image7.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert8">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image7.png "image_tooltip")


¬_θ_ denotes observing a bug in our code. Therefore, _P(X|¬θ)_ is the conditional probability of passing all the tests even when there are bugs present in our code. This term depends on the test coverage of the test cases. Even though we do not know the value of this term without proper measurements, in order to continue this discussion let us assume that _P(X|¬θ) = 0.5_. Accordingly,



<p id="gdcalert8" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image8.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert9">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image8.png "image_tooltip")




*   **_P(θ|X) —_** Posteriori probability denotes the conditional probability of the hypothesis _θ_ after observing the evidence _X._ This is the probability of observing no bugs in our code given that it passes all the test cases. Since we now know the values for the other three terms in the Bayes' theorem, we can calculate the posterior probability using the following formula:



<p id="gdcalert9" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image9.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert10">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image9.png "image_tooltip")
We can also calculate the probability of observing a bug, given that our code passes all the test cases _P(¬θ |X)_.



<p id="gdcalert10" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image10.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert11">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image10.png "image_tooltip")


We now know both conditional probabilities of observing a bug in the code and not observing the bug in the code. Yet how are we going to confirm the valid hypothesis using these posterior probabilities?

<h2>Maximum a Posteriori (MAP)</h2>


We can use _MAP_ to determine the valid hypothesis from a set of hypotheses. According to _MAP_, the hypothesis that has the maximum posterior probability is considered as the valid hypothesis. Therefore, we can express the hypothesis _θMAP_ that is concluded using MAP as follows:



<p id="gdcalert11" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image11.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert12">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image11.png "image_tooltip")


The _argmaxθ_ operator estimates the event or hypothesis _θi _that maximizes the posterior probability P(_θi_|X). Let us apply _MAP_ to the above example in order to determine the true hypothesis:



<p id="gdcalert12" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image12.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert13">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image12.png "image_tooltip")




<p id="gdcalert13" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image13.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert14">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image13.png "image_tooltip")


Figure 1 — _P(X|θ)_ and _P(X|¬θ)_ when changing the _P(θ)_ = _p_

Figure 1 illustrates how the posterior probabilities of possible hypotheses change with the value of prior probability. Unlike frequentist statistics, where our belief or past experience had no influence on the concluded hypothesis, Bayesian learning is capable of incorporating our belief to improve the accuracy of predictions. Assuming that we have fairly good programmers and therefore the probability of observing a bug is _P(θ)_ = _0.4_ , then we find the _θMAP_:



<p id="gdcalert14" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image14.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert15">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image14.png "image_tooltip")
However, _P(X)_ is independent of _θ_, and thus _P(X)_ is the same for all the events or hypotheses. Therefore, we can simplify the _θMAP_ estimation, without the denominator of each posterior computation as shown below:



<p id="gdcalert15" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image15.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert16">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image15.png "image_tooltip")


Notice that MAP estimation algorithms do not compute the posterior probability of each hypothesis to decide which is the most probable hypothesis. <span style="text-decoration:underline;">Assuming that our hypothesis space is continuous</span> (i.e. fairness of the coin encoded as probability of observing heads, coefficient of a regression model, etc.), where endless possible hypotheses are present even in the smallest range that the human mind can think of, or for even a discrete hypothesis space with a large number of possible outcomes for an event, we do not need to find the posterior of each hypothesis in order to decide which is the most probable hypothesis. <span style="text-decoration:underline;">Therefore, the practical implementation of _MAP_ estimation algorithms uses approximation techniques, which are capable of finding the most probable hypothesis without computing posteriors or only by computing some of them.</span>

Using the Bayesian theorem, we can now incorporate our belief as the prior probability, which was not possible when we used _frequentist statistics_. However, we still have the problem of deciding a sufficiently large number of trials or attaching a confidence to the concluded hypothesis. This is because the above example was solely designed to introduce the Bayesian theorem and each of its terms. Let us now gain a better understanding of Bayesian learning to learn about the full potential of Bayes' theorem.

<h2>Bayesian Learning</h2>


So far, we have discussed Bayes' theorem and gained an understanding of how we can apply Bayes' theorem to test our hypotheses. However, when using single point estimation techniques such as _MAP_, we will not be able to exploit the full potential of Bayes' theorem. With Bayesian learning, we are dealing with random variables that have probability distributions. Let us try to understand why using exact point estimations can be misleading in probabilistic concepts.

Consider the prior probability of not observing a bug in our code in the above example. We defined that the event of not observing bugs is _θ_ and the probability of producing a bug-free code _P(θ)_ was taken as _p_. However, the event _θ_ can actually take two values — either _true _or _false_ — corresponding to not observing a bug or observing a bug respectively. Therefore, observing a bug or not observing a bug are not two separate events, they are two possible outcomes for the same event _θ_. Since all possible values of _θ_ are a result of a random event, we can consider _θ_ as a random variable. Therefore, _P(θ) _is not a single probability value, rather it is a discrete probability distribution that can be described using a probability mass function.



<p id="gdcalert16" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image16.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert17">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image16.png "image_tooltip")


Figure 2 — Prior distribution _P(θ)_ and Posterior distribution _P(θ|X)_ as a probability distribution

Figure 2 illustrates the probability distribution _P(θ)_ assuming that _p = 0.4_. Therefore, _P(θ)_ can be either _0.4_ or _0.6,_ which is decided by the value of _θ_ (i.e. whether _θ_ is_ true_ or _false_). If we apply the Bayesian rule using the above prior, then we can find a posterior distribution _P(θ|X)_ instead of a single point estimation for that. Figure 2 also shows the resulting posterior distribution. You may recall that we have already seen the values of the above posterior distribution and found that _P(θ = true|X) = 0.57_ and _P(θ=false|X) = 0.43_. Notice that I used _θ = false_ instead of _¬θ_. This is because we do not consider _θ_ and _¬θ _as two separate events — they are the outcomes of the single event _θ_. Even though _MAP_ only decides which is the most likely outcome, when we are using the probability distributions with Bayes' theorem, we always find the posterior probability of each possible outcome for an event.

You may wonder why we are interested in looking for full posterior distributions instead of looking for the most probable outcome or hypothesis. If we use the _MAP_ estimation, we would discover that the most probable hypothesis is discovering no bugs in our code given that it has passed all the test cases. Remember that _MAP_ does not compute the posterior of all hypotheses, instead, it estimates the maximum probable hypothesis through approximation techniques. In fact, _MAP_ estimation algorithms are only interested in finding the mode of full posterior probability distributions. However, if we compare the probabilities of _P(θ = true|X)_ and _P(θ = false|X)_, then we can observe that the difference between these probabilities is only _0.14_. Hence, there is a good chance of observing a bug in our code even though it passes all the test cases. According to the posterior distribution, there is a higher probability of our code being bug-free, yet we are uncertain whether or not we can conclude our code is bug-free simply because it passes all the current test cases. We can now observe that due to this uncertainty we are required to either improve the model by feeding more data or extend the coverage of test cases in order to reduce the probability of passing test cases when the code has bugs. We can perform such analyses incorporating the uncertainty or confidence of the estimated posterior probability of events only if the full posterior distribution is computed instead of using single point estimations. To further understand the potential of these posterior distributions, let us now discuss the coin flip example in the context of Bayesian learning.

I will define the fairness of the coin as _θ_. We can use the probability of observing heads to interpret the fairness of the coin by defining _θ_ = _P(heads)_. Hence, _θ_ = _0.5_ for a fair coin and deviations of _θ_ from _0.5_ can be used to measure the bias of the coin. Since the fairness of the coin is a random event, _θ_ is a continuous random variable. As such, the prior, likelihood, and posterior are continuous random variables that are described using probability density functions.

Let us now attempt to determine the probability density functions for each random variable in order to describe their probability distributions.

<h2>Binomial Likelihood</h2>


The likelihood for the coin flip experiment is given by the probability of observing heads out of all the coin flips given the fairness of the coin. As we have defined the fairness of the coins (_θ_) using the probability of observing heads for each coin flip, we can define the probability of observing heads or tails given the fairness of the coin _P(y|θ)_ where _y = 1_ for observing heads and _y = 0_ for observing tails. Accordingly:

Now that we have defined two conditional probabilities for each outcome above, let us now try to find the _P(Y=y|θ)_ joint probability of observing heads or tails:

Note that _y_ can only take either _0_ or _1_, and _θ_ will lie within the range of _[0,1]_. We can rewrite the above expression in a single expression as follows:

The above equation represents the likelihood of a single test coin flip experiment. Interestingly, the likelihood function of the single coin flip experiment is similar to the Bernoulli probability distribution. The Bernoulli distribution is the probability distribution of a single trial experiment with only two opposite outcomes. As the [Bernoulli probability distribution](https://en.wikipedia.org/wiki/Bernoulli_distribution) is the simplification of [Binomial probability distribution](https://en.wikipedia.org/wiki/Binomial_distribution) for a single trail, we can represent the likelihood of a coin flip experiment that we observe _k_ number of heads out of _N_ number of trials as a Binomial probability distribution as shown below:

<h2>Maximum Likelihood (ML) Hypothesis, h<sub>ML</sub> </h2>


• If we assume that every hypothesis in H is equally probable i.e. P(h<sub>i</sub>) = P(h<sub>j</sub>) for all hindi jhin H 

We can only consider P(D|h) to find the most probable hypothesis. 

• P(D|h) is often called the likelihood of the data D given h • Any hypothesis that maximizes P(D|h) is called a maximum likelihood  (ML) hypothesis, h<sub>ML</sub>.



<p id="gdcalert17" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image17.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert18">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image17.png "image_tooltip")


                                Example - Does the patient have cancer or not? 

• The test returns a correct positive result in only 98% of the cases in which the disease  is actually present, and a correct negative result in only 97% of the cases in which the  disease is not present. 

• Furthermore, .008 of the entire population have cancer. 

P(cancer) = .008 P(not cancer) = .992 

P(+|cancer) = .98 P(-|cancer) = .02 

P(+|not cancer) = .03 P(-|not cancer) = .97 

• A patient takes a lab test and the result comes back positive. 

P(+|cancer) P(cancer) = .98 * .008 = .0078 

P(+|not cancer) P(not cancer) = .03 * .992 = .   h<sub>MAP </sub>is not cancer 

• Since P(cancer|+) + P(not cancer|+) must be 1 

P(cancer|+) = .0078 / (.0078+.0298) = .21 

P(not cancer|+) = .0298 / (.0078+.0298) = .79

<h2>
                                     Brute-Force Bayes Concept Learning </h2>



        • A Concept-Learning algorithm considers a finite hypothesis space H defined over an instance space X 


        • The task is to learn the target concept (a function) c : X  {0,1}. • The learner gets a set of training examples ( <x<sub>1</sub>,d<sub>l</sub>> . . . <x<sub>m</sub>,d<sub>m</sub>> ) where x<sub>i</sub>is an instance from X and d<sub>i</sub>is its target value (i.e. c(x<sub>i</sub>) = d<sub>i</sub>).

<h2>
                                         Brute-Force MAP Learning Algorithm </h2>



        1. For each hypothesis h in H, calculate the posterior probability 


        2. Output the hypothesis h<sub>MAP </sub>with the highest posterior probability 

<p id="gdcalert18" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image18.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert19">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image18.png "image_tooltip")



        • This algorithm may require significant computation, because it applies Bayes theorem to each hypothesis in H to calculate P(h|D ) .  


        – While this is impractical for large hypothesis spaces,  


        – The algorithm is still of interest because it provides a standard against which we  may judge the performance of other concept learning algorithms. 


        • BF MAP learning algorithm must specify values for P(h) and P(D|h). • P(h) and P(D|h) must be chosen to be consistent with the assumptions: 1. The training data D is noise free (i.e., d<sub>i </sub>= c(x<sub>i</sub>)). 


        2. The target concept c is contained in the hypothesis space H 


        3. We have no a priori reason to believe that any hypothesis is more probable than any other. 


        • With these assumptions: 


        

<p id="gdcalert19" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image19.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert20">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image19.png "image_tooltip")



        

<p id="gdcalert20" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image20.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert21">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image20.png "image_tooltip")



         • So, the values of P(h|D) will be: 


        

<p id="gdcalert21" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image21.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert22">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image21.png "image_tooltip")
where VS<sub>H,D </sub>is the version space of H with respect to D.


        

<p id="gdcalert22" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image22.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert23">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image22.png "image_tooltip")



        .

<h2>
                                                        Version Space</h2>



         • Given a set of training examples, The set of concepts consistent with a set of training examples is called a version space (for that set of examples)


         • Version space method involves identifying all concepts consistent with a set of training examples • Can be implemented incrementally, one example at a time 


        • Start with a given set of hypothesis of allowable concepts


        • Process the training examples sequentially 


        • As each example is seen, the set of concepts consistent with all the training data so far is narrowed down • After seeing enough examples, may converge to a unique concept and learning is complete • Even if the process hasn’t yet converged to a single hypothesis, may still be able to find the appropriate hypothesis.


        • P(D) = |VS<sub>H,D</sub>| / |H| because 


        - the sum over all hypotheses of P(h|D) must be one and  


        the number of hypotheses from H consistent with D is |VS<sub>H,D</sub>| , or 


        - we can derive P(D) from the theorem of total probability and  


        the fact that the hypotheses are mutually exclusive (i.e., (i≠ j)(P(h<sub>i </sub> h<sub>j</sub>) = 0) 

<p id="gdcalert23" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image23.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert24">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image23.png "image_tooltip")


<p id="gdcalert24" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image24.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert25">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image24.png "image_tooltip")



        ##Evolution of posterior probabilities P(h|D)  with increasing training data. 


        

<p id="gdcalert25" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image25.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert26">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image25.png "image_tooltip")


<p id="gdcalert26" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image26.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert27">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image26.png "image_tooltip")



        (a) Uniform priors assign equal probability to each hypothesis.  As training data increases first to Dl (b), then to Dl to the power  D2 (c), 


        the posterior probability of inconsistent hypotheses becomes zero, while posterior  probabilities increase for hypotheses remaining in the version space.

<h2>
        Maximum Likelihood and  Least-Squared Error Hypotheses </h2>



        • Many learning approaches such as neural network learning, linear  regression, and polynomial curve fitting try to learn a continuous-valued  target function. 


        • Under certain assumptions any learning algorithm that minimizes  the squared error between the output hypothesis predictions and  the training data will output a MAXIMUM LIKELIHOOD  HYPOTHESIS.  


        • The significance of this result is that it provides a Bayesian justification  (under certain assumptions) for many neural network and other curve  fitting methods that attempt to minimize the sum of squared errors over  the training data. 


                           The Normal Distribution


        The **normal distribution** refers to a family of [continuous probability distributions](https://stattrek.com/statistics/dictionary.aspx?definition=Continuous%20probability%20distribution) described by the normal equation.


        The Normal Equation


        The normal distribution is defined by the following equation:


        **The Normal Equation**. The value of the random variable _Y_ is:


        Y = { 1/[ σ * sqrt(2π) ] } * e-(x - μ)2/2σ2


        where _X_ is a normal random variable, μ is the mean, σ is the standard deviation, π is approximately 3.14159, and _e_ is approximately 2.71828.


        

<p id="gdcalert27" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image27.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert28">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image27.png "image_tooltip")



        The random variable _X_ in the normal equation is called the **normal random variable**. The normal equation is the [probability density function](https://stattrek.com/statistics/dictionary.aspx?definition=Probability%20density%20function) for the normal distribution.


        The Normal Curve


        The graph of the normal distribution depends on two factors - the mean and the standard deviation. The mean of the distribution determines the location of the center of the graph, and the standard deviation determines the height and width of the graph. All normal distributions look like a symmetric, bell-shaped curve, as shown below.


        **Smaller standard deviation**


        

<p id="gdcalert28" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image28.gif). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert29">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image28.gif "image_tooltip")


<p id="gdcalert29" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image29.gif). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert30">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image29.gif "image_tooltip")



        **Bigger standard deviation**


        When the standard deviation is small, the curve is tall and narrow; and when the standard deviation is big, the curve is short and wide (see above)


        Probability and the Normal Curve


        The normal distribution is a continuous probability distribution. This has several implications for probability.



*   The total area under the normal curve is equal to 1.
*   The probability that a normal random variable _X_ equals any particular value is 0.
*   The probability that _X_ is greater than _a_ equals the area under the normal curve bounded by _a_ and plus infinity (as indicated by the _non-shaded_ area in the figure below).
*   The probability that _X_ is less than _a_ equals the area under the normal curve bounded by _a_ and minus infinity (as indicated by the _shaded_ area in the figure below).

        

<p id="gdcalert30" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image30.gif). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert31">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image30.gif "image_tooltip")



        Additionally, every normal curve (regardless of its mean or standard deviation) conforms to the following "rule".

*   About 68% of the area under the curve falls within 1 standard deviation of the mean.
*   About 95% of the area under the curve falls within 2 standard deviations of the mean.
*   About 99.7% of the area under the curve falls within 3 standard deviations of the mean.

        Collectively, these points are known as the **empirical rule** or the **68-95-99.7 rule**. Clearly, given a normal distribution, most outcomes will be within 3 standard deviations of the mean.

<h2>
        Calculating h<sub>ML</sub></h2>


*   Given that the noise ei obeys a Normal distribution with zero mean and unknown variance 2 ,each di must also obey a Normal distribution with variance 2 centered around the true target value f (xi ) rather than zero. 

     • p(di |h) can be written as a Normal distribution with variance 2 and mean  = f (xi ). 

                         

<p id="gdcalert31" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image31.jpg). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert32">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image31.jpg "image_tooltip")
                    

<h2>           Discussions:</h2>



        • The maximum likelihood hypothesis h<sub>ML </sub>is the one that minimizes the sum of the  squared errors between observed training values d<sub>i</sub>and hypothesis predictions h(x<sub>i</sub>).  • This holds under the assumption that the observed training values d<sub>i</sub>are generated by  adding random noise to the true target value, where this random noise is drawn  independently for each example from a Normal distribution with zero mean.  • Similar derivations can be performed starting with other assumed noise distributions,  producing different results. 


            • Why is it reasonable to choose the Normal distribution to characterize noise? – One reason is that it allows for a mathematically straightforward analysis.  – A second reason is that the smooth, bell-shaped distribution is a good approximation to  many types of noise in physical systems. 


        • Minimizing the sum of squared errors is a common approach in many neural network,  curve fitting, and other approaches to approximating real-valued functions

<h2>
                                                      Bayes Optimal Classifier </h2>



            • Consider a hypothesis space containing three hypotheses, hl, h2, and h3.  – Suppose that the posterior probabilities of these hypotheses given the training data are .4, .3,  and .3 respectively.  


            – Thus, hl is the MAP hypothesis.  


            – Suppose a new instance x is encountered, which is classified positive by _hl, _but negative by  _h2 _and h3.  


            – Taking all hypotheses into account, the probability that x is positive is .4 (the probability  associated with _h1), _and the probability that it is negative is therefore .6.  


            – The most probable classification (negative) in this case is different from the classification  generated by the MAP hypothesis. 


        • The most probable classification of the new instance is obtained by  combining the predictions of all hypotheses, weighted by their posterior  probabilities. 


        • If the possible classification of the new example can take on any value _v<sub>j</sub>_from some set V, then the probability P(v<sub>j</sub>| D) that the correct  classification for the new instance is _v<sub>j</sub>_: 


        

<p id="gdcalert32" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image32.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert33">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image32.png "image_tooltip")


Disadvantages:

• Although the Bayes optimal classifier obtains the best performance that  can be achieved from the given training data, it can be quite costly to  apply.  

– The expense is due to the fact that it computes the posterior  probability for every hypothesis in H and then combines the  predictions of each hypothesis to classify each new instance. 

• An alternative, less optimal method is the Gibbs algorithm: 

<h2>Gibbs Sampling</h2>


1. Choose a hypothesis _h _from H at random, according to the posterior  probability distribution over H. 

2. Use _h _to predict the classification of the next instance _x. _

Disadvantages:

The h is chosen at random so gives a large error

The error of Gibbs sampling => 2(The error of Bayes Classifier)

<h2><p style="text-align: right">
Naive Bayes Classifier </p>
</h2>



        • One highly practical Bayesian learning method is Naive Bayes Learner (_Naive Bayes Classifier). _


        • The naive Bayes classifier applies to learning tasks where each instance  _x _is described by a conjunction of attribute values and where the target  function f (x) can take on any value from some finite set V.  


        • A set of training examples is provided, and a new instance is presented,  described by the tuple of attribute values _(al, a2 ...an).  _


        • The learner is asked to predict the target value (classification), for this  new instance. 


        The Bayesian approach to classifying the new instance is to assign the  most probable target value v<sub>MAP</sub>, given the attribute values (al, a2 ... an) that describe the instance. 


        

<p id="gdcalert33" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image33.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert34">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image33.png "image_tooltip")



        • It is easy to estimate each of the P(v<sub>j</sub>) simply by counting the frequency with which  each target value v<sub>j </sub>occurs in the training data.  


        • However, estimating the different P(al,a2…an | v<sub>j</sub>) terms is not feasible unless we have  a very, very large set of training data.  


            – The problem is that the number of these terms is equal to the number of possible instances  times the number of possible target values.  


            – Therefore, we need to see every instance in the instance space many times in order to obtain  reliable estimates. 


        • The naive Bayes classifier is based on the simplifying assumption that the attribute  values are conditionally independent given the target value. 


        • For a given the target value of the instance, the probability of observing conjunction  _al,a2...an, _is just the product of the probabilities for the individual attributes: 

<p id="gdcalert34" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image34.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert35">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image34.png "image_tooltip")


<h2>
                                      Gaussian Naive Bayes</h2>



            

<p id="gdcalert35" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image35.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert36">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image35.png "image_tooltip")



              

<p id="gdcalert36" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image36.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert37">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image36.png "image_tooltip")


<h2>                                                   Maximum Likelihood Estimate </h2>



        [Maximum Likelihood Estimation](https://en.wikipedia.org/wiki/Maximum_likelihood_estimation) involves treating the problem as an optimization or search problem, where we seek a set of parameters that results in the best fit for the joint probability of the data sample (X).


        First, it involves defining a parameter called theta that defines both the choice of the probability density function and the parameters of that distribution. It may be a vector of numerical values whose values change smoothly and map to different probability distributions and their parameters.


        In Maximum Likelihood Estimation, we wish to maximize the probability of observing the data from the joint probability distribution given a specific probability distribution and its parameters, stated formally as:



*   P(X | theta)

        This conditional probability is often stated using the semicolon (;) notation instead of the bar notation (|) because theta is not a random variable, but instead an unknown parameter. For example:

*   P(X ; theta)

        or

*   P(x1, x2, x3, …, xn ; theta)

        This resulting conditional probability is referred to as the likelihood of observing the data given the model parameters and written using the notation L() to denote the [likelihood function](https://en.wikipedia.org/wiki/Likelihood_function). For example:

*   L(X ; theta)

        The objective of Maximum Likelihood Estimation is to find the set of parameters (theta) that maximize the likelihood function, e.g. result in the largest likelihood value.

*   maximize L(X ; theta)

        We can unpack the conditional probability calculated by the likelihood function.


        Given that the sample is comprised of n examples, we can frame this as the joint probability of the observed data samples x1, x2, x3, …, xn in X given the probability distribution parameters (theta).

*   L(x1, x2, x3, …, xn ; theta)

        The joint probability distribution can be restated as the multiplication of the conditional probability for observing each example given the distribution parameters.

*   product i to n P(xi ; theta)

        Multiplying many small probabilities together can be numerically unstable in practice, therefore, it is common to restate this problem as the sum of the log conditional probabilities of observing each example given the model parameters.

*   sum i to n log(P(xi ; theta))

        Where log with base-e called the natural logarithm is commonly used.


                       Examples:


        

<p id="gdcalert37" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image37.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert38">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image37.png "image_tooltip")



        

<p id="gdcalert38" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image38.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert39">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image38.png "image_tooltip")



        

<p id="gdcalert39" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image39.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert40">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image39.png "image_tooltip")


<h2>
        Gaussian Mixture Models (GMMs)</h2>


                    Introduction to Clustering


        Clustering refers to grouping similar data points together, based on their attributes or features.


        For example, if we have the income and expenditure for a set of people, we can divide them into the following groups:



*   First – Earn high, spend high
*   Second – Earn high, spend low
*   Third – Earn low, spend low
*   Fourth – Earn low, spend high

        Each of these groups would hold a population with similar features and can be useful in pitching the relevant scheme/product to the group. Think of credit cards, car/property loans, and so on. In simple words:


        The idea behind clustering is grouping data points together, such that each individual cluster holds the most similar points.


        There are [various clustering algorithms](https://www.analyticsvidhya.com/blog/2016/11/an-introduction-to-clustering-and-different-methods-of-clustering/?utm_source=blog&utm_medium=gaussian-mixture-models-clustering) out there. One of the most popular clustering algorithms is k-means. Let us understand how the k-means algorithm works and what are the possible scenarios where this algorithm might come up short of expectations.


         


        Introduction to k-means Clustering


        k-means clustering is a distance-based algorithm. This means that it tries to group the closest points to form a cluster.


        Let’s take a closer look at how this algorithm works. This will lay the foundational blocks to help you understand where Gaussian Mixture Models will come into play later in this article.


        So, we first define the number of groups that we want to divide the population into – that’s the value of k. Based on the number of clusters or groups we want, we then randomly initialize k centroids.


        The data points are then assigned to the closest centroid and a cluster is formed. The centroids are then updated and the data points are reassigned. This process goes on iteratively until the location of centroids no longer changes.


        Check out the [below gif](https://gfycat.com/softenragedhypsilophodon) which represents the whole process of initializing and updating clusters. The number of clusters is assigned to be 10:


        Here is an in-depth guide: [The Most Comprehensive Guide to k-means you’ll Ever Need!](https://www.analyticsvidhya.com/blog/2019/08/comprehensive-guide-k-means-clustering/?utm_source=blog&utm_medium=gaussian-mixture-models-clustering)


         


        Drawbacks of k-means Clustering


        We noticed that all the clusters created have a circular shape. This is because the centroids of the clusters are updated iteratively using the mean value.


        Now, consider the following example where the distribution of points is not in a circular form. What do you think will happen if we use k-means clustering on this data? It would still attempt to group the data points in a circular fashion. That’s when k-means fails to identify the right clusters:


        

<p id="gdcalert40" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image40.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert41">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image40.png "image_tooltip")



        Hence, we need a different way to assign clusters to the data points. So instead of using a distance-based model, we will now use a distribution-based model. And that is  Gaussian Mixture Models. 


         


        Introduction to Gaussian Mixture Models (GMMs)


        Gaussian Mixture Models (GMMs) assume that there are a certain number of Gaussian distributions, and each of these distributions represent a cluster. Hence, a Gaussian Mixture Model tends to group the data points belonging to a single distribution together.

<h3>
        Definitions</h3>



        A Gaussian Mixture is a function that is comprised of several Gaussians, each identified by k ∈ {1,…, K}, where K is the number of clusters of our dataset. Each Gaussian k in the mixture is comprised of the following parameters:

*   A mean μ that defines its centre.
*   A covariance Σ that defines its width. This would be equivalent to the dimensions of an ellipsoid in a multivariate scenario.
*   A mixing probability π that defines how big or small the Gaussian function will be.

        Let us now illustrate these parameters graphically:


        

<p id="gdcalert41" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image41.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert42">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image41.png "image_tooltip")



        Here, we can see that there are three Gaussian functions, hence K = 3. Each Gaussian explains the data contained in each of the three clusters available. The mixing coefficients are themselves probabilities and must meet this condition:


        

<p id="gdcalert42" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image42.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert43">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image42.png "image_tooltip")



        Let’s say we have three Gaussian distributions (more on that in the next section) – GD1, GD2, and GD3. These have a certain mean (μ1, μ2, μ3) and variance (σ1, σ2, σ3) value respectively. For a given set of data points, our GMM would identify the probability of each data point belonging to each of these distributions.


         Gaussian Mixture Models are probabilistic models and use the soft clustering approach for distributing the points in different clusters.Here, we have three clusters that are denoted by three colors – Blue, Green, and Cyan. Let’s take the data point highlighted in red. The probability of this point being a part of the blue cluster is 1, while the probability of it being a part of the green or cyan clusters is 0.


        

<p id="gdcalert43" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image43.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert44">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image43.png "image_tooltip")



        Now, consider another point – somewhere in between the blue and cyan (highlighted in the below figure). The probability that this point is a part of cluster green is 0, right? And the probability that this belongs to blue and cyan is 0.2 and 0.8 respectively.


        

<p id="gdcalert44" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image44.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert45">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image44.png "image_tooltip")



         


        The Gaussian Distribution


        A bell-shaped curve, with the data points symmetrically distributed around the mean value.


        The below image has a few Gaussian distributions with a difference in mean (μ) and variance (σ2). Remember that the higher the σ value more would be the spread:


        

<p id="gdcalert45" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image45.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert46">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image45.png "image_tooltip")



        Source: Wikipedia


        In a one dimensional space, the [probability density function](https://courses.analyticsvidhya.com/courses/applied-machine-learning-beginner-to-professional?utm_source=blog&utm_medium=gaussian-mixture-models-clustering) of a Gaussian distribution is given by:


        

<p id="gdcalert46" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image46.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert47">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image46.png "image_tooltip")



        where μ is the mean and σ2 is the variance.


        But this would only be true for a single variable. In the case of two variables, instead of a 2D bell-shaped curve, we will have a 3D bell curve as shown below:


        

<p id="gdcalert47" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image47.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert48">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image47.png "image_tooltip")



        The probability density function would be given by:


        

<p id="gdcalert48" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image48.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert49">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image48.png "image_tooltip")



        where x is the input vector, μ is the 2D mean vector, and Σ is the 2×2 covariance matrix. The covariance would now define the shape of this curve. We can generalize the same for d-dimensions.


        Thus, this multivariate Gaussian model would have x and μ as vectors of length d, and Σ would be a d x d covariance matrix.


        Hence, for a dataset with d features, we would have a mixture of k Gaussian distributions (where k is equivalent to the number of clusters), each having a certain mean vector and variance matrix. But wait – how is the mean and variance value for each Gaussian assigned?


        These values are determined using a technique called Expectation-Maximization (EM). We need to understand this technique before we dive deeper into the working of Gaussian Mixture Models.


         


         \


<h3>
        Expectation-Maximization</h3>



        Expectation-Maximization (EM) is a statistical algorithm for finding the right model parameters. We typically use EM when the data has missing values, or in other words, when the data is incomplete.


        These missing variables are called latent variables. We consider the target (or cluster number) to be unknown when we’re working on an [unsupervised learning](https://www.analyticsvidhya.com/blog/2017/09/common-machine-learning-algorithms/?utm_source=blog&utm_medium=gaussian-mixture-models-clustering) problem.


        It’s difficult to determine the right model parameters due to these missing variables. Think of it this way – if you knew which data point belongs to which cluster, you would easily be able to determine the mean vector and covariance matrix.


        Since we do not have the values for the latent variables, Expectation-Maximization tries to use the existing data to determine the optimum values for these variables and then finds the model parameters. Based on these model parameters, we go back and update the values for the latent variable, and so on.


        Broadly, the Expectation-Maximization algorithm has two steps:

*   E-step: In this step, the available data is used to estimate (guess) the values of the missing variables
*   M-step: Based on the estimated values generated in the E-step, the complete data is used to update the parameters

        Expectation-Maximization is the base of many algorithms, including Gaussian Mixture Models. So how does GMM use the concept of EM and how can we apply it for a given set of points? Let’s find out!


         


        Expectation-Maximization in Gaussian Mixture Models


        Let’s understand this using another example. I want you to visualize the idea in your mind as you read along. This will help you better understand what we’re talking about.


        Let’s say we need to assign k number of clusters. This means that there are k Gaussian distributions, with the mean and covariance values to be μ1, μ2, .. μk and Σ1, Σ2, .. Σk . Additionally, there is another parameter for the distribution that defines the number of points for the distribution. Or in other words, the density of the distribution is represented with Πi.


        Now, we need to find the values for these parameters to define the Gaussian distributions. We already decided the number of clusters, and randomly assigned the values for the mean, covariance, and density. Next, we’ll perform the E-step and the M-step!


         


        E-step:


        For each point xi, calculate the probability that it belongs to cluster/distribution c1, c2, … ck. This is done using the below formula:


        

<p id="gdcalert49" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image49.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert50">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image49.png "image_tooltip")



        This value will be high when the point is assigned to the right cluster and lower otherwise.


         


        M-step:


        Post the E-step, we go back and update the Π, μ and Σ values. These are updated in the following manner:

1. The new density is defined by the ratio of the number of points in the cluster and the total number of points: \


<p id="gdcalert50" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image50.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert51">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image50.png "image_tooltip")

2. The mean and the covariance matrix are updated based on the values assigned to the distribution, in proportion with the probability values for the data point. Hence, a data point that has a higher probability of being a part of that distribution will contribute a larger portion:

        

<p id="gdcalert51" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image51.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert52">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image51.png "image_tooltip")



        Based on the updated values generated from this step, we calculate the new probabilities for each data point and update the values iteratively. This process is repeated in order to maximize the [log-likelihood function](https://www.analyticsvidhya.com/blog/2018/07/introductory-guide-maximum-likelihood-estimation-case-study-r/). <span style="text-decoration:underline;">Effectively we can say that the k-means only considers the mean to update the centroid while GMM takes into account the mean   as well as the variance of the data!</span>


<span style="text-decoration:underline;">                    [The In Depth Maths behind GMMS](https://docs.google.com/document/d/1ilgP3l38Dhb0RyHrV5HAs05ZbDMYVdAv96NGhwoPfJ0/edit?usp=sharing)</span>


        [Python implementation from scratch](https://github.com/ocontreras309/ML_Notebooks/blob/master/GMM_Implementation.ipynb)

<h5>
        Pros</h5>



        **Speed **It is the fastest algorithm for learning mixture models


        **Agnostic **As this algorithm maximizes only the likelihood, it will not bias the means towards zero, or bias the cluster sizes to have specific structures that might or might not apply.

<h5>                        Cons</h5>



        **Singularities **When one has insufficiently many points per mixture, estimating the covariance matrices becomes difficult, and the algorithm is known to diverge and find solutions with infinite likelihood     unless one regularizes the covariances artificially.


        **Number of components **This algorithm will always use all the components it has access to, needing held-out data or information theoretical criteria to decide how many components to use in the absence of external cues.

<h2>                  Topic Modeling</h2>



        Topic modeling is a method for unsupervised classification of documents, similar to clustering on numeric data, which finds some natural groups of items (topics) even when we’re not sure what we’re looking for.These topics will only emerge during the topic modelling process (therefore called latent). 


        A document can be a part of multiple topics, kind of like in soft clustering in which each data point belongs to more than one cluster.

<h3>
        Uses</h3>



        Topic modeling provides methods for automatically organizing, understanding, searching, and summarizing large electronic archives.


        It can help with the following:



*   discovering the hidden themes in the collection.
*   classifying the documents into the discovered themes.
*   using the classification to organize/summarize/search the documents.
<h2>
    Latent Dirichlet Allocation</h2>



        Latent Dirichlet Allocation (LDA) is a “generative probabilistic model” used for Topic Modelling.


        Each document contains a set of words which can be described as a distribution of topics and each topic can be described by a distribution of words


        The Algorithm


        LDA is a form of unsupervised learning that views documents as bags of words (ie order does not matter). LDA works by first making a key assumption: the way a document was generated was by picking a set of topics and then for each topic picking a set of words. 


                    To do this it does the following for each document m:



1. Assume there are k topics across all of the documents
2. Distribute these k topics across document m (this distribution is known as α and can be symmetric or asymmetric, more on this later) by assigning each word a topic.
3. For each word w in document m, assume its topic is wrong but every other word is assigned the correct topic.
4. Probabilistically assign word w a topic based on two things: \
- what topics are in document m \
- how many times word w has been assigned a particular topic across all of the documents (this distribution is called β, more on this later)
5. Repeat this process a number of times for each document and you’re done!

<h3>                          Model definition</h3>




*   
*   

<p id="gdcalert52" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image52.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert53">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image52.png "image_tooltip")

*   Each document is a collection of words.
*   We have 5 documents each containing the words listed in front of them( ordered by frequency of occurrence).
*   What we want to figure out are the words in different topics, as shown in the table below. Each row in the table represents a different topic and each column a different word in the corpus. Each cell contains the probability that the word(column) belongs to the topic(row).
*   
*   

<p id="gdcalert53" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image53.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert54">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image53.png "image_tooltip")

*   Each topic contains a score for all the words in the corpus.
*   Finding Representative Words for a Topic
*   We can sort the words with respect to their probability score. \
The top x words are chosen from each topic to represent the topic. If x = 10, we’ll sort all the words in topic1 based on their score and take the top 10 words to represent the topic. \
This step may not always be necessary because if the corpus is small we can store all the words in sorted by their score.
*   Alternatively, we can set a threshold on the score. All the words in a topic having a score above the threshold can be stored as its representative, in order of their scores.

         


        

<p id="gdcalert54" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image54.jpg). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert55">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image54.jpg "image_tooltip")



                   Above is what is known as a plate diagram of an LDA model where:

<h3>
             Definitions and notations</h3>




*   k — Number of topics a document belongs to (a fixed number)
*   V — Size of the vocabulary
*   M — Number of documents
*   N — Number of words in each document
*   w — A word in a document. This is represented as a one hot encoded vector of size V (i.e. V — vocabulary size)
*   w (bold w): represents a document (i.e. vector of “w”s) of N words
*   D — Corpus, a collection of M documents
*   z — A topic from a set of k topics. A topic is a distribution words

        α is the per-document topic distributions,


        β is the per-topic word distribution,


        θ is the topic distribution for document m,


        φ is the word distribution for topic k,


        z is the topic for the n-th word in document m, and  w is the specific word


<h3>                        [Dirichlet Distribution](https://towardsdatascience.com/dirichlet-distribution-a82ab942a879)</h3>


<h3>
    

<p id="gdcalert55" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image55.gif). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert56">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image55.gif "image_tooltip")
</h3>



               Animation above are iterations of taking 1000 samples from a Dirichlet distribution using an  increasing alpha value.


        The Dirichlet distribution takes a number (called alpha in most places) for each topic (or category). In the GIF (and for our purposes), every topic is given the same alpha value you see displayed. Each dot represents some distribution or mixture of the three topics like (1.0, 0.0, 0.0) or (0.4, 0.3, 0.3). Remember that each sample has to add up to one.


        At low alpha values (less than one), most of the topic distribution samples are in the corners (near the topics). For really low alpha values, it’s likely you’ll end up sampling (1.0, 0.0, 0.0), (0.0, 1.0, 0.0), or (0.0, 0.0, 1.0). This would mean that a document would only ever have one topic, if we were building a three topic probabilistic topic model from scratch.


        At alpha equal to one, any space on the surface of the triangle (or if you prefer, ‘2-simplex’) is fair game (in other words, uniformly distributed). You could equally likely end up with a sample favoring only one topic, a sample that gives an even mixture of all the topics, or something in between.


        For alpha values greater than one, the samples start to congregate in the center of the triangle. This means that as alpha gets bigger, your samples will more likely be uniform — that is, represent an even mixture of all the topics.


        The GIF demonstrates the sampling of topic mixtures for the documents, but the Dirichlet distribution is also assumed the source (the [Bayesian prior](https://en.wikipedia.org/wiki/Prior_probability)) for the mixture of parts per topic.


        Three topics were used, as that works well when plotting in three dimensions. But typically, it is better to use more than three topics, depending on the number of documents you have.


        If you look at the [LDA tool](https://lettier.com/lda-topic-modeling/) mentioned earlier, you’ll see an alpha and beta slider.


        These two [hyperparameters](https://en.wikipedia.org/wiki/Hyperparameter_(machine_learning)) are required by LDA. The alpha controls the mixture of topics for any given document. Turn it down, and the documents will likely have less of a mixture of topics. Turn it up, and the documents will likely have more of a mixture of topics.


        The beta hyperparameter controls the distribution of words per topic. Turn it down, and the topics will likely have less words. Turn it up, and the topics will likely have more words.


        Ideally, we want our composites to be made up of only a few topics and our parts to belong to only some of the topics. With this in mind, alpha and beta are typically set below one.

<h3>
        Tweaking the Model</h3>



        In the plate model diagram above, you can see that w is grayed out. This is because it is the only observable variable in the system while the others are latent. Because of this, to tweak the model there are a few things you can mess with and below I focus on two.


        α is a matrix where each row is a document and each column represents a topic. A value in row i and column j represents how likely document i contains topic j. A symmetric distribution would mean that each topic is evenly distributed throughout the document while an asymmetric distribution favors certain topics over others. This affects the starting point of the model and can be used when you have a rough idea of how the topics are distributed to improve results.


        β is a matrix where each row represents a topic and each column represents a word. A value in row i and column j represents how likely that topic i contains word j. Usually each word is distributed evenly throughout the topic such that no topic is biased towards certain words. This can be exploited though in order to bias certain topics to favor certain words. For example if you know you have a topic about Apple products it can be helpful to bias words like “iphone” and “ipad” for one of the topics in order to push the model towards finding that particular topic.

<h3>                  An Example</h3>



        Suppose you have various photographs(documents) with captions(words). You want to display them in a gallery so you decide to categorize the photographs on various themes(topics) based on which you will create different sections in your gallery.


        

<p id="gdcalert56" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image56.jpg). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert57">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image56.jpg "image_tooltip")



        Photo by [Soragrit Wongsa](https://unsplash.com/@invictar1997?utm_source=medium&utm_medium=referral) on [Unsplash](https://unsplash.com/?utm_source=medium&utm_medium=referral)


        You decide to create k=2 sections in your album — nature and city. Naturally, the classification isn’t so clear as some photographs with city have trees and flowers while the nature ones might have some buildings in it. You, as a start, decide to assign the photographs which only have nature or city elements in them into their respective categories while you randomly assigned the rest.


        You notice that a lot of photographs in nature have the word tree in their captions. So you concluded that the word tree and topic nature must be closely related.


        Next, you pick the word building and check how many photographs are in nature because they have the word building in their caption. You don’t find many and now are less sure about building belonging to the topic nature and associate it more strongly with the topic city.


        You then pick a photograph which has the caption “The tree is in front of the building and behind a car” and see that it is in the category nature currently.


        You then chose the word tree, and calculate the first probability p(topic t | document d): other words in the caption are building and car, most photographs having captions with building or car in it are in city, so you get a low probability.


        Now the second probability p(word w| topic t): we know that a lot of photographs in nature have the word trees in it. So you get a high score here.


        You update the probability of tree belonging in nature by multiplying the two. You get a lower value than before for tree in topic nature because now you have seen that tree and words such as building/car in the same caption, implying that trees can also be found in cities.


        For the same reason, when you update the probability for tree belonging in topic city, you will notice that it will be greater than what it was before.


        After multiple iterations over all the photographs and for each topic, you will have accurate scores for each word with respect to each topic. Your guesses will keep getting better and better because you’ll conclude from the context that words such as buildings, sidewalk, subway appear together and hence must belong to the same topic, which we can easily guess is city.


        Words such as mountains, fields, beach which might not appear together in a lot of captions but they do appear often without city words and hence will have higher scores for nature.


        While words such as trees, flowers, dogs, sky will have almost the same probability of being in either as they occur in both topics.


        As for the photograph, you see that it has 1 word (with average probability) from category nature and 2 words (with high probability) from city, you conclude, it belongs to city more strongly than it does to nature and hence you decide to add it in city.


        <span style="text-decoration:underline;">Resources:</span>


        [Python Implementation](https://colab.research.google.com/drive/16wWtsr4mBkQu-haAvXfrEokVBePrVqxV?usp=sharing)


                	

                       

     
