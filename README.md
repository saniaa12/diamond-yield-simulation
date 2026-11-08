# Diamond Yield Simulation

A small Python project exploring how randomness affects diamond
yields during mining trips.

I built this project to practise NumPy, probability modelling,
simulation and data visualisation.

## Research question

How do variations in the number of ores mined and the drops
from each ore affect total diamond yield?

## Model

The simulation generates 1,000 mining trips using these assumptions:

- Ore counts follow a Poisson distribution with a mean of 30.
- Each ore drops 1, 2, 3 or 4 diamonds, with probabilities
  of 40%, 20%, 20% and 20%.
- Drops are independent of each other and of the ore count.

These are illustrative assumptions rather than a validated
model of actual Minecraft gameplay.

## Analysis

The notebook:

- Simulates diamond yields using NumPy.
- Calculates the mean, standard deviation and fifth-percentile yield.
- Compares the simulated mean with the theoretical mean of
  66 diamonds per trip.
- Plots a histogram of simulated outcomes.

The fifth-percentile yield describes the lower end of the
simulated outcomes. It is not the minimum possible yield
or a guarantee about a future trip.

## How to run

1. Download the notebook from this repository.
2. Install NumPy and Matplotlib in your Python environment:

   ```bash
   pip install numpy matplotlib
   ```

3. Open the notebook in VS Code with Jupyter support,
   or another Jupyter notebook environment.
4. Select your Python environment and run the cells in order.

## Limitations

- The model does not include travel time, danger or inventory limits.
- The assumptions have not been checked against gameplay data.
- Simulation estimates may change with the random seed
  and number of simulated trips.

## Possible next steps

- Compare different average ore counts.
- Investigate how the number of simulations affects the results.
- Estimate the probability of collecting fewer than a chosen
  number of diamonds.
