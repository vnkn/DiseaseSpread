# DiseaseSpread

This whitepaper and the accompanying code demonstrates our model for understanding the flow of the spread of a disease. We use a slightly modified SIR Model to
generate simulated disease spreads, and then we try to learn this information using
two different methods. First, we use Google Deepmind’s recently released Graph Nets
library, which has the capacity to store (and dynamically update) disease capabilities
such as its infectivity rate, transition power between edges, and the number of sick
(and healthy) people in different nodes of the graph. We then compare the results
of this simulation to a regular Feed-Forward Neural Network, and show that using
GraphNets to store more data results in significantly better train and test accuracy -
with the mean squared error being 3 times using Graphnet than with a regular neural
network.
