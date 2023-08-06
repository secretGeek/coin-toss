# Coin-Toss-Simulator

This is a Web-based simulation of a 'Coin Toss Game'.

See it online here: **[Coin-Toss Simulation](https://secretgeek.github.io/coin-toss/)**


## Description of this Coin Toss Simulation

1. Start with a population of people, all of whom have the same amount of money. (There are two constants to be set here: `populationSize` (e.g. `100`) and `moneyPerPlayer` (e.g. `$100`))
2. Everyone gets to play a coin toss game which is tilted in their favor! If they win, their wealth grows by `WinPercent` -- and if they lose, their wealth shrinks by `LossPercent`. The great news is that `WinPercent` is greater than `LostPercent` -- so your expected return on each bet is positive!
3. Repeat step 2 indefinitely.

Since the expected return is positive, "on average" people will win money! So everyone gets rich! Yay! Except... that's not what happens. Take a look at how it plays out. It sucks. It really sucks.

Keep an eye on what happens to the distribution of wealth amongst the population.

To begin with the distribution of wealth is perfectly "level" - everyone has the same amount of money. After one round of betting each player has either gained 60% or lost 40%. Half the people are happy, and half are not. But the happy half are more in front than the unhappy half.

As the rounds accumulate, you may expect people's wealth to bounce up and down around the $100 mark -- since the mean dollars per player is fixed (no money is being created or destroyed, no new players are joining, none are leaving.)

But what the Yard Sale Model instead shows is that, although an individual's wealth may bounce up and down from one bet to the next, people with less money are likely to continue to average toward less and less money, their money tending to accumulate in a group of "haves". And as time progresses forward, the group of "haves" tends to get smaller, until even 1 player captures close to $100 of all wealth.

The Yard Sale Model is used to demonstrate that wealth accumulation can arise naturally, even in a seemingly "fair" system, and without any variation in "skill" between players.

There are variants of the Yard Sale Model where extra factors are applied. For example, the application of a "tax" after each round, which moves each player some distance closer to the mean (i.e. "robbing the rich and giving to the poor") -- and its been shown that such models can, with the right factors, achieve a steady state with very similar wealth distribution to those observed in modern societies.

Critics of the Yard Sale Model indicate that "true" trades are not the same as these "zero-sum" gambles. For example, if I buy milk from a dairy farmer, I buy it because its value *to me* (thirsty for milk) is greater than the value it has for the farmer (who is not thirsty for milk) -- hence "value" is created in real trades.

I've built this simulation with the -- as yet unrealised -- intention of looking at ways to model "non-zero sum" trades. It's quite difficult in practice to find a simple model that realistically depicts the "non-zero" nature of trades. Which trades are really non-zero? If i'm the final consumer of a product (e.g. milk, or cigarettes) then I'm not really gaining more than I've paid or growing my wealth. I feel that to do the concept justice I may need to add labor, and labor-productivity factors.

## References

- [Why the super rich are inevitable](https://pudding.cool/2022/12/yard-sale/)
- [Is Inequality Inevitable? - Scientific American](https://www.scientificamerican.com/article/is-inequality-inevitable/)
  - [(PDF) Describing Realistic Wealth Distributions with the Extended Yard-Sale Model of Asset Exchange](https://www.researchgate.net/publication/301876072_Describing_Realistic_Wealth_Distributions_with_the_Extended_Yard-Sale_Model_of_Asset_Exchange)
- [Yard Sale Model - University of Maryland](http://www.physics.umd.edu/hep/drew/math_general/yard_sale.html)
- [Yard Sale Wealth Model - Hash.ai](https://hash.ai/@eadan/yard-sale-wealth-model)
- [Gini coefficient - Wikipedia](https://en.wikipedia.org/wiki/Gini_coefficient)
