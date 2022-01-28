---
layout: post
title: Ugrainium 2.35
date: 2018-03-25 19:09 -0800
category: [Lifehack, Nutrition]
tags: [timehack, nutrition, habits]
description: Staying fueled without the hassle
image:
  src: /assets/img/flax-seeds.jpg
  width: 1000
  height: 200
  alt: Ugrainium Mix
---
## Problem Description

Out of a typical day, I've measured that about 2-3 hours goes toward dealing with food in some way. Time spent preparing, foraging, eating, shopping, cleaning-up afterward, or recovering from the post-lunch sleepeez. That's close to 20%, more than a day a week, of my waking life tied-up with eating. What if that time could be taken back and used for something else less mundane, like art, spending time with friends, or just relaxing to get more creative energy?

Another issue is getting the proper amount of nutrients in a day without going overboard with specific nutrition regimes. After measuring the sum of nutrition profiles for foods eaten during the day, it's obvious that getting the proper amounts of nutrients like potassium, omega-3, and insoluble fiber won't happen by accident just by choosing a variety of "healthy" foods

There are a few existing products to solve this problem, for example: Soylet and Huel. I've tried them, but found them either not very tasty, or the ingredients made too many negative nutritional compromises for the sake of marketability

## Solution Idea

Prepare a balanced, easy to use, portable food which is nutritionally complete and can be quickly consumed every two hours throughout the day. By having nutrition every two hours, the post eating sleepiness can be avoided and energy levels can stay at full power all day.

A set of base ingredients are selected and combined in the proper ratios to match individual nutrition needs.

## Steps

### Ingredient Selection
A set of base ingredients were selected by going through the USDA foods database and the NIH articles on nutrition for specific foods. The ingredients were also taste tested by varying the recipe every once in a while. Some of the base ingredients include flaxseed, barley, oats, lecithin (for choline), pea and whey protein.

### Recipe Calculation
The SciPy library includes a set of optimizers which are used to find the optimal combination of ingredients to meet nutritional needs. The set of ingredients along with their nutrients plus a personal nutrition profile are kept in a Google Sheet and read-in by the optimizer

### Equipment Needed
![Mixing Container with Fin](/assets/img/bucket-with-fin.jpg){: width="200" height="150" .shadow .right }
![Mixing Container](/assets/img/mixing-bucket.jpg){: width="200" height="150" .shadow .right }

There are a few items which will be needed for the preparation of Ugrainium:
 - A food-safe _mixing container_ with a tight fitting lid. A 25 liter mixing container has enough volume for about two weeks of food.
 - Attaching an internal mixing fin is needed to thoroughly mix the ingredients
 - All ingredient calculations and measurements are by mass. A _5kg scale_ with a 1g precision is need for measuring the bulk ingredients. _A 50g scale_ with a 1mg precision is needed for measuring vitamin and mineral ingredients
 - A _coffee grinder_ for grinding tablets and minerals into a fine powder
 - Optionally use a _stand mixer_. A stand mixer does a thorough job of mixing the non-bulk ingredients before being added to the bulk ingredients


## Aha!

A side effect of having prepared meals is that hunger driven eating and food selection (junk food) are taken out of the equation. That has meant that over-eating and mindless snacking doesn't happen. As a result, it's easy to stay at an ideal weight and body composition, just eat on schedule.

Another boon has been for long bike rides. It's much easier to stay fueled-up by bringing Ugrainium on the ride and mixing in with water along the way. Mid-ride bonking has been eliminated. Plus Ugrainium is light-weight and not bulky which is great on a all day ride.

## What's Next

 - Use singular value decomposition to measure ingredient spread and use the information to select more ideal ingredients
