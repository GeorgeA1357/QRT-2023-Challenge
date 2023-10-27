# QRT-2023-Challenge
Can you explain the price of electricity? ChallengeData by MathA


# Predicting 24h changes in Electricity futures for Germany and France
QRT's 2023 data challenge: https://challengedata.ens.fr/participants/challenges/97/

# Challenge context

Every day, a multitude of factors impact on the price of electricity. Local weather variations will affect both electricity generation and demand for instance. Long term phenomena, such as global warming, will also have a significant influence. Geopolitical events, such as the war in Ukraine, may affect in parallel the price of commodities, which are key inputs in electricity generation, knowing that each country relies on a particular energy mix (nuclear, solar, hydro, gas, coal, etc). Moreover, each country may import/export electricity with its neighbors through dynamical markets, like in Europe. These various elements make quite complex the modelisation of electricy price in a given country.

# Challenge goals

The aim is to model the electricity price from weather, energy (commodities) and commercial data for two European countries - France and Germany. Let us stress that the problem here is to explain the electricity price with simultaneous variables and thus this is not a prediction problem.

More precisely, the goal of this challenge is to learn a model that outputs from these explanatory variables a good estimation for the daily price variation of electricity futures) contracts, in France and Germany. These contracts allow you to receive (or to deliver) a given amount of electricity at a specified price by the contract delivered at a specified time in the future (at the contract's maturity). Thus, futures contracts are financial instruments that give you some expected value on the future price of electricity under actual market conditions - here, we focus on short-term maturity contracts (24h). Let us stress that electricity future exchange is a dynamic market in Europe.

Regarding the explanatory variables, the participants are provided with daily data for each country which involve weather quantitative measurements (temperature, rain, wind), energetic production (commodity price changes), and electricity use (consumption, exchanges between the two countries, import-export with the rest of Europe).

The score function (metric) used is the Spearman's correlation between the participant's output and the actual daily price changes over the testing data set sample.
