---
layout: post
title: '(Work in progress) Mechanical Calculator  with Lego-like Modular Logic Gates'
---
![Solidworks model](/mypage/assets/images/mechanical-calculator/banner.png)

## Concept

Some weeks ago I was following my usual Youtube routine and I came across a really cool [video by Ben Eater](https://www.youtube.com/watch?v=wvJc9CZcvBc) about [adder circuits](https://en.wikipedia.org/wiki/Adder_(electronics)). He also made one with commercial logic gate ICs and that got me thinking: what if I could make mechanical logic gates and connect them together so that I could add something like 2 four bit numbers?

![Adder Circuit diagram](/mypage/assets/images/mechanical-calculator/adder_circuit.png)

A 1 bit full adder circuit. Below, you can see the truth table for each logic gate used, as well as for the whole circuit.


|BIT 1| BIT 2| XOR           | AND          | OR    | FULL ADDER |
|:---:|:----:|:-------------:|:------------:|:-----:|:----------:|
|**0**| **0**|0              | 0            | 0     |0           |
|**1**| **0**|1              | 0            | 1     |1           |
|**0**| **1**|1              | 0            | 1     |1           |
|**1**| **1**|0              | 1            | 1     |10          |

So, I obsessed a little bit about this in the following days and thought it would be really cool to have the logic gates modular, kind of like legos. They would be a small square with two inputs and one output. Inside, the logic operations would be done with levers. An example: one lever is a NOT gate, if you push one end away from you (you could call this a **1**, **True**, **Yes**, etc) the other end will come close to you (**0**, **False**, **No**) and vice-versa.

![lever as NOT gate](/mypage/assets/images/mechanical-calculator/not_gate.png)

Nowadays, with 3D printing, this idea could result in some pretty cool computing projects, so one more constraint was that each module should be easily 3D PRINTABLE so that I could share it on ![Thingiverse](https://www.thingiverse.com/) and hopefully see what crazy things people could do.

## First Sketches

I spent a lot of time thinking about the mechanisms for each gate, and here's what I got so far:
- **OR**

- **AND**

- The **XOR** gate is way more complicated and I have not been able to come up with a simple enough design yet. You can make one with one **OR**, one **NAND**(NOT + AND), and one **AND** and this might be the best solution for now.[(Wikipedia)](https://en.wikipedia.org/wiki/XOR_gate)

![An XOR gate made with OR, NAND, and AND](/mypage/assets/images/mechanical-calculator/xor1.png)
