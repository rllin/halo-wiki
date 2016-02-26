# The Function

The RQA function is found in the analytics.py program in the halo python library.  It is titled rqa and requires 4 inputs: trace; embedding dimension (ed); time-delay (td); and the neighborhood (radius). details on what these 4 inputs mean can be found below

## Trace

The trace is simply the filtered signal, so the signal should have been rectified, band-passed, and notch filtered as described on the [[EMG]] page.

## Embedding Dimension (ed)

The embedding dimension is the dimension that the original signal exists in.  the emg records the signal in 2 dimensions, namely time and voltage.  However, the signal could be coming from any number of places, not just the muscle, and with each new source that adds variability and possible dimensions to the true source signal.  There are a number of ways to determine the correct embedding dimension, with one of the most popular being the [false nearest neighbors method](http://www.csee.wvu.edu/~xinl/library/papers/physics/embedding_dimension.pdf).  With EMG signals the embedding dimension should be between 10 and 20 dimensions to ensure proper encapsulation.

## Time-Delay (td)

The time delay is the amount of time you want your windows of the RQA analysis to overlap.  the window is the slice of the overall signal that you are comparing. generally 4-6 points is used as the time delay.

## The Neighborhood (radius)

The neighborhood or radius is how similar 2 points need to be to be considered a recurrence. A large radius will lead to lots of recurrences, including one's that may or may not be useful, a small radius will lead to fewer recurrences leading to little information to gleen insight from.  The problem of choosing the proper radius for an EMG signal is compounded by the fact that people will vary in the relative volatility of their muscles.  Becuase of this it is important to have the radius be a percentage of the overall range of possible values in the signal. For most emg signals 15% of the distance between the max and the min is deemed a suitable value.  When computing RQA you will need to have this change subject to subject and if the same subject comes back for multiple sessions even session to session the radius will need to be recalculated as placing the emg in a slightly different spot will change the geometry and the strength of the signal.