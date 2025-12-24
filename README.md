# omega-structure-vs-noise

## Omega as an Empirical Measure of Temporal Structure in Financial Time Series

### Overview
This repository presents an empirical study of a simple information-theoretic quantity, Omega, defined as the mutual information between consecutive observations in a time series.

The goal is to test whether Omega can distinguish structured financial data from genuinely random sequences.

### Definition
Given a time series X_t, we define:

Omega = I(X_t ; X_(t-1))

where I(· ; ·) denotes mutual information.  
Omega measures temporal dependence or structural coherence that is not captured by marginal entropy alone.

### Null Hypothesis
For an IID random sequence, Omega should be approximately zero (up to finite-sample estimation error).

### Experiments
We compare:
- BTC return time series (financial market data)
- California Daily 3 lottery numbers (a certified random process)

using identical estimation procedures for Omega.

### Key Observation
Omega is statistically non-zero for BTC returns and collapses toward zero for the lottery sequence, indicating the presence of temporal structure in market data that is absent in true randomness.

### Scope and Limitations
- This repository does not claim universality.
- No physical or thermodynamic laws are asserted.
- No cross-domain generalization is made.
- Omega is studied here purely as an empirical diagnostic.

### Status
This repository documents an initial, reproducible finding.  
Extensions and theoretical generalizations are intentionally deferred.

