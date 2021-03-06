---
layout: post
title: "probability distributions - Intro"
author: "szarki9"
categories: statistics
tags: [distributions]
image: netherlands9.JPG
---
<p>Hello All!</p>
<p align = "justify">I haven’t been there for quite some time, sorry about that. But cutting to the important stuff… In a number of next posts, I would like to describe the application of more or less common probability distributions. I have spent lately quite some time on it, as in order to understand what distribution you should use, firstly you need to understand what each distribution means. So… starting from basic definitions and basing distributions I will try to demonstrate here the more advanced ones!</p>
<p align = "justify">First of all, what a probability distribution is? By <b>distribution of a probability</b>, we call <ins>the function that assigns the probability of having a particular value of a random variable to its values</ins>. Given that, the values of that function will be located between 0 and 1. When I think about probability distribution I try to think about something easy and basic, like the distribution of people’s height in Poland. Let’s take into consideration only men. The average height of men in Poland is 180 cm. What does it mean? That if you take a random man on the street this is a high probability that he will be around that. What exact probability it will be? It will be 50% exactly (you can check my previous post about descriptive statistics) and that means that most of the men in Poland are “distributed” around that number. Later on, I will depict a couple of examples so stay with me!
</p>
<p align = "justify"> Now, as a distribution of a probability is a function, it can take discrete values or continuous values. In the first instance, I will focus on discrete distributions 😊. By discrete function, we call a function that has a finite or countable number of values that (in distributions) take non-zero probability as an outcome of the function. 
</p>
### Bernoulli distribution (binomial distribution)
<p align = "justify"> All of you probably have heard about the Bernoulli scheme, which is a model of a situation where we have an experiment with a binary outcome. A binary outcome is assigned to the success or a failure, where a probability of success has a value of <b>p</b> (what gives the probability of failure equal to <b>1-p</b>). <p><b>Bernoulli distribution</b> function tells you what is <ins>a probability of <b>k</b> successes among <b>n</b>-times Bernoulli trial</ins>, having <b>p</b>, as a probability of success. Look below on a distribution formula:
</p> </p>
<p align = "center"> $$x_k = k,\; p_k = P(X=k) = {n\choose k} p^k (1-p)^{n-k} \sim B(n,p)$$ 
$$k \in \{0,1,...,n\},\; n\in \mathbb{N},\; p \in(0,1)$$
</p>
### Geometric distribution
<p align = "justify"> But having a Bernoulli scheme we might want to ask a bit different question. For example, <ins>what is the probability of having success after <b>k-1</b> failures</ins>, when the probability of success equals <b>p</b>? We will consider it as waiting time for a first success to come. In that case, k might be any natural number from 0. Look below on a distribution formula:
</p>
<p align = "center">
$$x_k=k,\; p_k = P(X=k)=p(1-p)^{k-1} \sim Geo(p)$$ 
$$ k \in \{0,1,...\},\; p \in(0,1)$$
</p>
### Negative binomial distribution
<p align = "justify"> Extension of the question from the last paragraph is question about <ins>the probability of waiting time for <b>m</b>-th success after <b>k</b> failures, where m is previously defined number </ins>. When m is an integer, then we call this distribution as <b>Pascal distribution</b> and when m is a real-value case then we call it <b>Polya distribution</b>. Probability mass function is:
</p>
<p align = "center">    
$$ x_k=k, \; p_k=P(X=k)={m-1\choose n-1}p^m(1-p)^{k-m} \sim NB(m,p)$$
$$k \in \{m,m+1,...\},\; p \in(0,1) $$
</p>
### Multinomial distribution
<p align = "justify"> Another useful distribution is a generalization of the binomial distribution. We can apply it to an experiment which we repeat <b>n</b> times. Each trial of the experiment can have different results, is independent and let’s say that there are <b>r</b> distinct results. The probability of each result is the same in every experiment and we call it by <b>pi</b> for i from 1 to r. Then if we assign to random variables from 1 to r, the number of occurrence for each distinct result we will have a random vector with a probability given by the below mass function:
</p>
<p align = "center">
$$ P(X_1=k_1,X_2=k_2,...,X_r=k_r)=\frac{n!}{k_1!k_2!...k_r!}p_1^{k_1}...p_r^{k_r} \sim Mult(n,p)$$
$$ \sum_{i=1}^{r}k_i = n,\;\sum_{i=1}^{r}p_i = 1,\; p_i \in (0,1),\; n\in \mathbb{N}$$
</p>
### Hypergeometric distribution
<p align = "justify">
When doing first probability classes exercises we often come across random draws of balls from an urn. We can have a draw with a return or without and so on. Let’s assume that we carry out an experiment when we draw <b>n</b> balls from an urn with <b>m</b> balls of one type and <b>N-m</b> balls of different types then that (and in total, we have <b>N</b> balls in our urn). We want to <ins>investigate the probability of drawing <b>k</b> balls from the first type of elements in our urn</ins>. The probability mass function for that is as below:
</p>
<p align = "center">
$$ P(X=k) = \frac{ {m\choose k}  {N-m\choose n-k} }{N\choose n} \sim HGeo(N,m,n)$$
$$ N \in \mathbb{N},\; m\in\{0,1,...,N\} ,\; n\in\{0,1,...,N\},$$
$$ k\in \{ max(0,n+m-N),..., min(n,m) \}$$
</p>
<p align = "justify">
<b>To sum up</b>, all of those distributions cover different situations that we want to model. Like you see, for each of them, probability distribution function looks a bit different and when you dive deeper into the expected values or variances you might see other relationships. </p>
<p align = "justify">
Hope it clarifies a little, whenever you have some feedback or questions you are more than welcome to contact me.
</p>
<p>xoxo,<br>
szarki9</p>
