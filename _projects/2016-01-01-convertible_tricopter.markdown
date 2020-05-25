---
layout: post
title: 'A Wooden Convertible Tricopter'
description: 'Tricopters are cool!'

---
![A convertible tricopter](/mypage/assets/images/tricopter/convert.gif)

This is a project I made between my last year in the brazilian equivalent of High School and the first year at college. I was really into UAVs and multirotors then, especially tricopters.

## Why a tricopter?

Tricopters were never the most popular, and nowadays quadcopters are even more standard than they were in 2015, when I made this. But tricopters are really cool. I personally think they are the prettiest multirotors and they have some advantages:
- Lower cost - you will have to buy one less motor and one less ESC.
- The arms are separated by 120 degrees, so finding a spot where the propellers be in your cameras field of view is usually easier
- The rear motor can be "steered" to compensate for the odd number of propellers and for yaw commands
- It is easier to design a tricopter with foldable arms than it is to design a quadcopter with this feature

## The project

I designed this mostly before I started college, so the very little I knew about engineering and designing something I learned from Youtube. Because of this and budget restrictions, I decided to make a wooden frame and it ended up working very well. The main frame is 3mm laser cut MDF and the arms are 12mm square balsa rods. It will break if you hit the ground too hard but, because it is wood, maintenance is really inexpensive.

## Components and a brief explanation

Assembling a multirotorcan be confusing at first because of names and units we don't know but here are the parts I chose and some explanation of why I chose them and how it works.

- Motor: iPower IQSeries 2212 1000kv

The motors will usually have these two numbers. The first (2212) is just dimensions, it meands the motor has a 22mm diameter and 12mm height. The second (1000kv) means that the motors rotation increases 1000rpm per volt applied. So 1kv just means 1 RPM/V. Motor manufacturers usually suggest a size of propeller to use with each one and there is usually a table for maximum traction for each propeller choice, and that can be a very good estimation of what motor you need and what your maximum weight can be.

- Propellers: 1045

The number of a propeller is composed of its diameter and pitch in inches. In this case, it has a diameter of 10 inches and a pitch of 4.5 inches.

- ESC: EMAX 12A for 3S

ESCs are the electronics that drive your motors and you will need one for each motor. In my understanding, an ESC is like a Variable Frequency Drive in the sense that it turns DC into 3 phase power for the motor but I could be wrong. The 12A means the maximum frequency it can handle is 12A. It is always good practice to have a reasonable margin of safety.

- Battery: 2200mAh 3S LiPO

Batteries have changed a lot since I made this tricopter, I believe 3S is not used very much nowadays. But 2200mAh is a standard unit for capacity, it means you could pull 2.2A for one hour, 4.4A for half an hour and so on. At the time, I chose this because it was the only battery I had, but you could make it a little more "engineered" by using a weight function to choose the battery that would give you the best endurance.

- Receiver: Flysky IA6B

Receivers usually come together with transmitters (the controls) and 2.4GHz is the standar frequency. Mine is really one of the most inexpensive ones. With higher prices, you could get better range and maybe even telemetry.

- Controller board: KK2

This is the brain of the multirotor. It takes the Pitch, Roll and Yaw commands from the receiver and turns them into signals for the motors as well as do the 3axis controls. KK2 was a really good choice at the time because it had a display, so I didnt need to connect it to a computer everytime I wanted to tune parameters etc. I believe boards nowadays are way more advanced. I plan on experimenting with [Ardupilot](https://ardupilot.org/) soon, it is a really cool opensource project that runs on a lot of the modern machines.

## Gallery

This tricopter has not seen a lot of flying in the last 3 years, so I will put some pictures here as soon as I get it flying again, which is probably going to be pretty soon, given that I am writing this during the COVID19 quarantine and I am currently tinkering with all my old projects. Stay tuned!
