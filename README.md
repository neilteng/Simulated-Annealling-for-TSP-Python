# Simulated-Annealling-for-TSP-Python
Python with check point and decay rate on all the possible parameter.


    def __init__(self, data=None, T0=5000.0, T_end=1e-8, alpha=0.98, epoch=10, MaxInt=1e7, re_heat_prop=0.10, re_heat_percent=0.05, decay_factor=500):
        """
        data: import data matrix, if None raise error
        T0: initial temperature to start the algorithms
        T_end: the temperature to stop the algorithms
        alpha: temperature decay rate
        epoch: repeatably create number of epoch of new path under current states and keep the best
        MaxInt: the number of iteration allowed.
        re_heat_prop: the probability to get the current temperature up after annealing.
        decay_factor: for new path generator, the bigger the less path generated during each generation.
