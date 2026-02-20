# Markov Credit Lab

Trying to build intuition for stochastic processes, credit risk, and portfolio loss models.

This project aims to learns concepts by **simulating them**, visualizing them, and gradually turning toy models into finance models.

*Why credit risk models behave the way they do*

---

## Learning Philosophy

Each notebook answers one question.

Not:

> "implement a Markov chain"

But:

> "what does a Markov chain actually mean for a firm’s credit quality?"

Every step adds only one idea:
simulation → intuition → math → financial interpretation

---

## Where this project is going

We will slowly build a full credit-risk engine starting from almost nothing.

random movement → ratings → defaults → portfolio losses → clustering → regimes → continuous time models

---

## Roadmap

### 00 - Markov Basics (Understanding movement between states)

Goal: Learn what a Markov chain *feels like*

* simulate a simple chain
* understand transition probabilities
* long-run distribution (stationarity)
* absorbing states
* expected time to absorption

Financial meaning:

> a company changing credit quality over time

---

### 01 - Credit Ratings

Goal: Turn states into credit ratings

* AAA → AA → A → BBB → BB → B → CCC → D
* default as absorbing state
* probability of eventual default
* expected time to default from each rating

Financial meaning:

> why lower ratings have shorter survival horizons

---

### 02 - Many Firms (Portfolio Behavior)

Goal: Understand portfolio loss distributions

* simulate thousands of firms
* distribution of defaults
* diversification vs concentration
* why losses are skewed

Financial meaning:

> where credit VaR comes from

---

### 03 - Regimes (Default Clustering)

Goal: Break independence assumption

* normal economy vs recession economy
* switching transition matrices
* clustered defaults

Financial meaning:

> systemic risk and crisis periods

---

### 04 - Continuous Time Credit Models

Goal: Connect to real quant finance models

* generator matrix
* hazard rates
* reduced-form default intensity models

Financial meaning:

> CDS pricing / survival probabilities

---

## Project Rules

1. Every notebook ends with a short insight section
   What did I learn? What surprised me?

2. Always simulate before reading theory

3. Every concept must be visualized

4. If I cannot explain it in simple words, I don’t understand it yet

---

## Current Status

Starting from scratch - rebuilding intuition for Markov chains and stochastic systems.

---

## Long-term goal

Be able to naturally understand and build models used in:

* CreditMetrics / rating migrations
* default clustering
* portfolio credit VaR
* intensity based models

without memorizing formulas - only understanding dynamics
