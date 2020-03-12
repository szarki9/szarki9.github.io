---
layout: post
title: "going forward with a little cryptography vol 2"
author: "szarki9"
categories: other
tags: [other]
image: nature-2.jpg
---
<p>Muy buenas chicos :)</p><p align="justify">After theory comes an application! What is the paradox actually saying to us? That after appropriate math calculations (promise you will see them!) number of <i>n</i> elements (people in that case) needed to solve our problem statement <i>rises in a line with a square root of the number of all possible cases (365 for us)</i>. And thanks to the name of the paradox, cryptographists have created the <b>birthday attack</b>. But before that a little background info:</p><p align="justify">Do you remember the hash function from the previous post? I have mentioned that hash function should be an injective function and it should be impossible to find two arguments for one value (this characteristic is called the second preimage resistant and this is one of the characteristics that good hash function supposes to have). So what is one part of cryptoanalysts job is to try to prove that one of the valuable characteristics is breakable. A case that I want to bring to light is the case of finding the hash function’s collisions, which is having two different messages and one encrypted value for both of them. In general, there is a finite number of values that hash function might return and there is an infinite number (or for sure greater) of messages that may be encrypted. So it should not surprise that collisions may appear somewhere and depend on how we are able to find them the quality of hash function may differ. </p><p align="justify">How birthday paradox is useful for finding collisions? One way to look for collisions is just go with brute-force attack and check every possibility that we might have, but when the number of all possibilities is 2^128 it is a quite big and time-consuming challenge. Thanks to the outcome of the paradox we know, that in order to find collision we only need to check the square root of all possible cases and then we should get the second argument for the same value. So funny thing and they say it works.</p><p align="justify">Okay, I think this is it for now (regarding cryptography), hope you have found it interesting in the same way as I haha.</p><p><br></p><p>xoxo,</p><p>szarki9</p>