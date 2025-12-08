# Binomial-option-pricing-crr
Implementation of the Cox–Ross–Rubinstein (CRR) binomial model for option pricing, including risk-neutral valuation, replicating portfolio (Δ and B), and discrete Greeks (Δ, Γ, Θ). 
Binomial Option Pricing (CRR Model)

This project implements the Cox–Ross–Rubinstein (CRR) binomial model for pricing European options.
It includes risk-neutral valuation, the replicating portfolio, and discrete Greeks, following the theoretical foundations of:

Hull – Options, Futures and Other Derivatives

Paul Wilmott Introduces Quantitative Finance

Hilpisch – Python for Finance

 Features
1. CRR Binomial Tree

Up and down factors derived from volatility:

𝑢
=
𝑒
𝜎
Δ
𝑡
,
 
𝑑
=
1
/
𝑢
u=e
σ
Δt
	​

, d=1/u

Risk-neutral probability:

𝑝
=
𝑒
𝑟
Δ
𝑡
−
𝑑
𝑢
−
𝑑
p=
u−d
e
rΔt
−d
	​


2. Option Pricing

European call payoff

Backward induction

Risk-neutral expectation + discounting

3. Replicating Portfolio

At each node:

Delta:

Δ
=
𝐶
𝑢
𝑝
−
𝐶
𝑑
𝑜
𝑤
𝑛
𝑆
𝑢
𝑝
−
𝑆
𝑑
𝑜
𝑤
𝑛
Δ=
S
up
	​

−S
down
	​

C
up
	​

−C
down
	​

	​


Bond position:

𝐵
=
𝑒
−
𝑟
Δ
𝑡
(
𝐶
𝑑
𝑜
𝑤
𝑛
−
Δ
𝑆
𝑑
𝑜
𝑤
𝑛
)
B=e
−rΔt
(C
down
	​

−ΔS
down
	​

)

Shows explicitly that an option is equivalent to a dynamic position in the underlying asset + bond.

4. Greeks from the Tree

Delta

Gamma

Theta

5. Visualization

Pretty plot of the underlying price tree

 Purpose

Build intuition behind derivatives pricing

Bridge toward the Black–Scholes model

Understand replication and risk-neutral pricing

Perfect for interviews in S&T, Derivatives, or Quant roles
