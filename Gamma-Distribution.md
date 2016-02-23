# Gamma Distribution
A [Gamma distribution](https://en.wikipedia.org/wiki/Gamma_distribution) can be used to approximate [[Reaction Times]].

## Equation
The gamma equation has three parameters, ```a```, ```epsilon```, and ```lambda```.

``` f(x| a,epsilon,lambda) = lambda^a * (x-epsilon)^(a-1) * exp(-lambda*(x-epsilon)) / gamma(a) ```

where gamma() is the [gamma function](https://en.wikipedia.org/wiki/Gamma_function).

### a
The rate parameter **a** reflects the approximate number of exponentials contributing to the function (potentially representing the number of exponentially-distributed processes occurring). Does not track with visual search set size.

### epsilon
The shift parameter **epsilon** moves the function along the x-axis without affecting its shape.
Varies with visual search task and target-present vs. target-absent, but not search set size - would seem to be more closely tied to decision processes.

### lambda
Each exponential process may have a different scale, but the average scale of the processes is captured by the parameter **lambda**. 
Captures the duration of search processes.

### Changes in parameters
Increase in **a** = more exponentials contributing to function (more skew)
	(potentially more exponentially-distributed processing steps)
 Increase in **E** = higher mean reaction time (change only in the mean)
 Increase in **L** = steeper/higher peak (more consistency / less variance) 
	(higher efficiency across processes)