---
description: Pass Pricing Mechanism
---

# 🧮 Access Pass Bonding Curves

Honey Chat employs a bonding curve to determine pass prices, acting as a mathematical formula governing token price changes. The bonding curve connects the creation of new passes with the cryptocurrency 'bonded' or put into the system.&#x20;

The bonding curve formula for pass prices when buying is the following equation:\
\
LOW

$$
f(x) = x * e^{2 pi i \xi x}
$$

MID

$$
f(x) = x * e^{2 pi i \xi x}
$$

HIGH

$$
f(x) = x * e^{2 pi i \xi x}
$$

For pass prices when selling, the formula is slightly different:

Where `f(x)` is the price of the next pass, measured in HONEY units, and `x` is the total passes in circulation (`x` increases when people buy and decreases when people sell).&#x20;

To illustrate these formulas, let’s say Amber buys a pass from someone who has five pass holders. The purchase price for such a pass with five holders is x + 10% fee = x HONEY. Let’s say Amber wants to resell the pass when that person has 10 holders. The selling price would be x – 10% fee = x HONEY. Therefore, Amber’s profit would be x – x = x HONEY.

## Enhanced Trading Dynamics in Honey Chat

The relationship between price and supply in Honey Chat is governed by a bonding curve equation that dynamically determines the pass price based on its supply. As the user base engages in buying passes, the price of each new pass rises in response to the bonding curve equation. Conversely, should users decide to sell their passes, the price experiences a decrease.

The trading fee of 10% is incorporated into the price during trades. The quadratic shape of Honey Chat's bonding curve encourages early adoption and investment, favoring lower prices for early investors. However, by introducing pass shorting and tiered access with subscriptions, Honey Chat addresses criticisms within the space, specifically concerns about the pass price becoming too high as popular creators' chat rooms attract more followers. This multifaceted approach ensures a more inclusive and sustainable model, countering the perception of benefits being limited to early adopters.

