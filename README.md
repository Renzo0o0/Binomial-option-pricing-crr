# Binomial-option-pricing-crr
Implementation of the Cox–Ross–Rubinstein (CRR) binomial model for option pricing, including risk-neutral valuation, replicating portfolio (Δ and B), and discrete Greeks (Δ, Γ, Θ). 
Binomial Option Pricing (CRR Model)


Hull – Options, Futures and Other Derivatives

Paul Wilmott Introduces Quantitative Finance

Hilpisch – Python for Finance

Features

CRR Binomial Tree

Up and down factors based on volatility:
u = exp(sigma * sqrt(dt))
d = 1 / u

Risk-neutral probability:
p = (exp(r * dt) - d) / (u - d)

Option Pricing

European call payoff at maturity

Backward induction

Risk-neutral expected value discounted at the risk-free rate

Replicating Portfolio
At each node:

Delta = (C_up - C_down) / (S_up - S_down)

Bond = exp(-r * dt) * (C_down - Delta * S_down)

This shows explicitly that an option can be replicated by holding Delta units of the underlying and a position in a risk-free bond.

Greeks (from the binomial tree)

Delta

Gamma

Theta

Visualization

Plot of the underlying's CRR price tree

Purpose

Build intuition behind derivatives pricing

Understand risk-neutral valuation

Show the mechanics of replication

Prepare for the Black–Scholes model

Useful for S&T, derivatives, quant, and risk interviews

How to Use

Run the single-cell Python file or notebook

Adjust parameters such as volatility, time steps, strike or interest rate

Observe how the option value, Greeks and the replicating portfolio change

Dependencies

numpy

pandas

matplotlib
