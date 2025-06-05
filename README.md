# Trading Challenge Probability Simulator  

[Try it live](https://victornpb.github.io/trade/)

This tool is effective at modeling a statisc system. It answers the question: "If a trader with a fixed set of performance stats trades with a fixed set of rules, what are the likely odds?"
It is excellent for analyzing the mathematical relationship between your inputs and the constraints of a prop firm challenge probabilities.

It does not predict the future or account for market dynamics. It is a probability calculator to test the statistical viability of a trading strategy profile.

---

## Why it matters, a concrete example

Most traders think they grasp the impact of win-rate and risk-reward, but tiny tweaks can flip the odds.

For example:

Lets say you trade with RR 1.5 to 2, risking $500 per trade (assuming 60% WR) your odds of passing an evaluation is about 69%.  
And lets say, you drop your risk to $250 per trade (not changing anything else)  
Your chance of passing an eval in 1 month collapses from 69% to only 22%!

Another example:

If your WR is only 50%, you risk $500 per trade with RR: 2.5 to 3, you have a 74% success of passing.
If you decide to risk only $250 trading RR: of 1.3 to 2 you would need an insane 84% win rate to have the same (74%) odds of passing as the example above.

Examples above use a typical 20-day challenge with a \$3 000 profit target and a \$1 500 loss limit.

---

## Context and limits

This is a **static-stats probability simulator**. This will not help you trade better, it will only help you understand the relationship between rules and odds.
You can do anything right and still setup yourself for failure by choosing risks that will put the odds against you, this tool will help you with that.

Market volatility, slippage, commissions, psychology, skill drift, and changing conditions are outside its scope.

---

## How you can use it

1. **Collect real stats** Grab your last few dozen trades: actual win-rate, average Risk-to-Reward, how often you trade, and typical risk per trade.  
2. **Set the challenge rules** Enter the prop-firm target, drawdown, and days allowed.  
3. **Run a multi-simulation** Start with at least a thousand runs. The pass percentage you see is the honest baseline for your current style.  
4. **Probe a single lever** Use the Success Optimizer to vary one variable while freezing the rest.  
   * What if you risk \$100 more?  
   * What if your win-rate improves by five points?  
   * What if you hold winners for a larger RR range?  
   The sweep shows which change delivers the biggest jump in pass probability.  
5. **Adjust your plan** Armed with the numbers, decide whether to tweak risk, hunt for higher RR, work on win-rate, or accept that the challenge isn’t favorable with your present stats.
