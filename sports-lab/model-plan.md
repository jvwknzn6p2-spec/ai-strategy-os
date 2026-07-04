# AI Sports Lab — Model Plan

## Objective

Predict MLB game outcomes and estimate win probabilities that can be
compared against betting market odds to find expected value.

## Pipeline

1. **Data Collection**
   - Team and player statistics
   - Starting pitcher data
   - Historical game results
   - Market odds

2. **Baseline Model**
   - Simple rating-based win probability (e.g., Elo-style)
   - Establish a benchmark before adding complexity

3. **Monte Carlo Simulation**
   - Simulate games thousands of times using team/player distributions
   - Produce win probability estimates with uncertainty

4. **Odds Analysis & Expected Value**
   - Convert market odds to implied probabilities
   - Compare model probability vs. implied probability
   - Flag positive expected value opportunities

5. **Backtesting**
   - Replay past seasons through the pipeline
   - Measure accuracy, calibration, and simulated return

6. **AI Multi-Agent Review**
   - Independent AI agents critique model assumptions and outputs
   - Disagreements are logged and investigated

## Success Criteria

- Model calibration measurably better than a naive baseline
- Fully reproducible backtest results
- Documented assumptions for every model component
