> [!IMPORTANT]
>
> This project is deprecated and is read-only for historical context only.

# Gilded Rose Refactoring Kata

This Kata was forked from [Emily Bache's version](https://github.com/emilybache/GildedRose-Refactoring-Kata) and modified to fit the needs of the Guild Education engineering team.

Select a language to do your code challenege in. Each language has a README explaining how to run your tests. You'll have two hours to interpret the requirements below, write tests, and refactor the implementation in your chosen language.

## Code Challenge

To start, you'll want to look at the requirements outlined below, which explain what the code is for. We strongly advise you that you'll also need some tests if you want to make sure you don't break the code while you refactor.

You should write some unit tests yourself, using the requirements below to identify suitable test cases. We've provided a failing unit test in a popular test framework as a starting point for you.

Whichever testing approach you choose, the idea of the exercise is to demonstrate your skills at designing test cases and refactoring.

## Requirements

*Estos requisitos también están disponibles [en Español](./GildedRoseRequirements_es.md).*

Hi and welcome to team Gilded Rose. As you know, we are a small inn with a prime location in a
prominent city ran by a friendly innkeeper named Allison. We also buy and sell only the finest goods.
Unfortunately, our goods are constantly degrading in quality as they approach their sell by date. We
have a system in place that updates our inventory for us. It was developed by a no-nonsense type named
Leeroy, who has moved on to new adventures. Your task is to add the new feature to our system so that
we can begin selling a new category of items. First an introduction to our system:

- All items have a SellIn value which denotes the number of days we have to sell the item
- All items have a Quality value which denotes how valuable the item is
- At the end of each day our system lowers both values for every item

Pretty simple, right? Well this is where it gets interesting:

- Once the sell by date has passed, Quality degrades twice as fast
- The Quality of an item is never negative
- "Aged Brie" actually increases in Quality the older it gets
- The Quality of an item is never more than 50
- "Sulfuras", being a legendary item, never has to be sold or decreases in Quality
- "Backstage passes", like aged brie, increases in Quality as its SellIn value approaches; Quality increases by 2 when there are 10 days or less and by 3 when there are 5 days or less but Quality drops to 0 after the concert

We have recently signed a supplier of conjured items. This requires an update to our system:

- "Conjured" items degrade in Quality twice as fast as normal items

Feel free to make any changes to the UpdateQuality method and add any new code as long as everything
still works correctly. However, do not alter the Item class or Items property as those belong to the
goblin in the corner who will insta-rage and one-shot you as he doesn't believe in shared code
ownership (you can make the UpdateQuality method and Items property static if you like, we'll cover
for you).

Just for clarification, an item can never have its Quality increase above 50, however "Sulfuras" is a
legendary item and as such its Quality is 80 and it never alters.

