# Simulated-Annealling-for-TSP-Python
Python with check point and decay rate on all the possible parameter.

sa = SA.Simulated_Anealing(data=data, T0=5e10, T_end=1e-8, alpha=0.99, epoch=50, MaxInt=1e6,
                                   re_heat_prop=0.1, re_heat_percent=0.10, portion_factor=0)
path_best, cost_best, time=sa.solve(verbose=False, check_point=False, filename=file)


data: import data matrix, if None raise error
T0: initial temperature to start the algorithms
T_end: the temperature to stop the algorithms
alpha: temperature decay rate
epoch: repeatably create number of epoch of new path under current states and keep the best
MaxInt: the number of iteration allowed.
re_heat_prop: the probability to get the current temperature up after annealing.
portion_factor: for new path generator, the bigger the more path generated during each generation.

