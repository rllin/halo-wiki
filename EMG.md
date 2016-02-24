There are 2 major steps to analyzing emg data.  The first is filtering the signal into something useful, and the second is extracting the data point that we can compare

# Filtering the signal

To filter the EMG signal, you first must rectify the signal.  rectifying the signal essentially takes the absolute value of the raw emg values.  This is done so that the signal has distinct peaks rather than bursts of noise.

The second step is applying what is known as a notch filter.  this will remove any noise fluctuating at a specific frequency.  In this case, we take a notch at 60hz because that is the frequency of electrical noise from wall outlets in America.

Finally, we feed the signal through a bandpass filter, this will remove both low frequencies and high frequencies that are not related to the signal.  In most cases, the signal should be band-passed with a low pass of 0 hz and a high-pass of 100 hz, however, this may change depending on how noisy the signal is.  for particularly noisy data it may be necessary to bandpass as small as a low pass at 0 and a high pass at 3 hz, however this should only be done to find the peaks and should not be referred to as the true data.

# Extracting the data from the signal

A number of ways to extract useful information from the emg signal are detailed below.

## Median Frequency/Mean Frequency

Both the Median Frequency and the Mean Frequency can be used as measures of peripheral fatigue as they both describe the power spectrum.  The power spectrum is a chart of all the individual frequencies that make up a signal and the amplitude associated with each signal.  As the muscle fatigues, the power spectrum shifts towards the lower frequencies, which is reflected by a lower median and mean frequency.  Generally median frequency has been shown to be a better reflection of the fatigue than mean frequency, however both are valid.

Details on how to actually calculate the [[median frequency]] or [[mean frequency]] can be found on their respective pages.

## Recurrence Plot Analysis (RQA)

RQA is a nonlinear approach to signal analysis, it essentially looks for recurrence in a signal, or how often a series of events repeat themselves.  A very good explanation of RQA can be found here https://www.nsf.gov/sbe/bcs/pac/nmbs/chap2.pdf including an example of using RQA for EMG analysis.  Overall RQA analysis produces a number of different statistics, but the one's we care about are the %determinism and the %laminarity.  Determinism refers to the number of recurrent points that form diagonal lines in the recurrence plot.  It is related to fatigue in that an increase in the determinism indicates greater levels of fatigue.

Details on how to run a [[RQA analysis]] are here