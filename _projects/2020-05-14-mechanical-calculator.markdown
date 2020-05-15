---
layout: post
title: 'Mechanical Calculator  with Lego-like Modular  Logic Gates (Work in progress)'
---

Some weeks ago I was following my usual Youtube routine and I came across a really cool [video by Ben Eater](https://www.youtube.com/watch?v=wvJc9CZcvBc) about [adder circuits](https://en.wikipedia.org/wiki/Adder_(electronics)). He also made one with commercial logic gate ICs and that got me thinking: what if I could make mechanical logic gates and connect them together so that I could add something like 2 four bit numbers?

![Adder Circuit diagram](/mypage/assets/images/mechanical-calculator/adder_circuit.png)

A 1 bit full adder circuit. Below, you can see the truth table for each logic gate used, as well as for the whole circuit.


|BIT 1| BIT 2| XOR           | AND          | OR    | FULL ADDER |
|:---:|:----:|:-------------:|:------------:|:-----:|:----------:|
|**0**| **0**|0              | 0            | 0     |0           |
|**1**| **0**|1              | 0            | 1     |1           |
|**0**| **1**|1              | 0            | 1     |1           |
|**1**| **1**|0              | 1            | 1     |10          |

So, thinking about how to make each logic gate mechanically and especially how to connect them, I thought it would be really cool to have them modular, kind of like legos
