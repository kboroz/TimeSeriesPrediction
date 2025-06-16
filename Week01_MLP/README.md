ALL RECOMMENDED - Watch at Least ONE of the Video-Playlists:

https://www.youtube.com/playlist?list=PL0rM26FV6611AJD1bOdfbwxAZuZiuHR8i

https://www.youtube.com/playlist?list=PL_iP0SGUzx9SvI_loo4I6orC-6o5-7hKp

https://www.youtube.com/playlist?list=PLqYFiz7NM_SMC4ZgXplbreXlRY4Jf4zBP

# INFO on Cross-Validation:

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

