
# INFO on Cross-Validation:

https://medium.com/@ahmedfahad04/understanding-walk-forward-validation-in-time-series-analysis-a-practical-guide-ea3814015abf

https://pub.towardsai.net/the-combinatorial-purged-cross-validation-method-363eb378a9c5

https://pub.towardsai.net/combinatorial-purgedkfold-cross-validation-for-deep-reinforcement-learning-f8df689ca874

Standard K-Fold CV

    Randomly splits data into K folds.
    Simple and fast.
    Assumes i.i.d., causes leakage in time series.
    Not suitable for financial time series data.

Walk-Forward CV

    Trains on past, tests on future in time order.
    Realistic for trading/backtesting.
    Tests only one path, can miss regime shifts.
    Common in finance.

Purged K-Fold CV

    Removes training samples that overlap with test label windows.
    Prevents label leakage.
    Needs label window info, reduces training size.
    Effective for financial ML.

Embargoed CV

    Adds time buffer after test fold to prevent correlation leakage.
    Handles serial dependency.
    Shrinks training set further.
    Useful when features are autocorrelated.

Combinatorial Purged CV (CPCV)

    Tests many train/test splits with purging and embargoing.
    Robust to regime changes, gives distributional insight.
    Very compute-heavy.
    Best for strategy validation in finance


