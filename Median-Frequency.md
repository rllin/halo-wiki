## Purpose

Median frequency is an easy and reliable way to get a quick overview of what the frequency power spectrum looks like.  After transforming the signal with a fourier's transformation, you can produce a power spectrum that looks like the one below

![](https://www.eda.kent.ac.uk/images/general/medical_demg6.jpg)

Now this power spectrum includes both a rested and a fatigued spectrum which is perfect for our purposes.  On the power spectrum above the x-axis are all the frequencies that make up the signal while the y-axis can be thought of as the amount that those frequencies contribute to the overall signal.  As the muscle fatigues the power spectrum shifts to the left, meaning that the lower frequencies contribute more to the overall signal.  This is represented by a decrease in the median frequency, which is weighted to take into account the strength of each individual frequency.

## Advantages of Mean Frequency

While both mean and median frequencies do a good job of providing a quick estimate of the power spectrum....

## Analysis

Computing the median frequency involves 4 distinct steps, filtering, slicing, transforming, and averaging the signal.

### Filtering

Filtering involves rectifying, bandpass filtering and notch filtering details of which can be found back at the [[EMG]] page.

### Slicing

Some studies may skip this step depending on the study design and how much data is actually encapsulated in the data file.  For most studies there will be parts of the signal data file that are not important (waiting for the trial to start, in between tests when we are still recording for convenience), it is important to cut the file into sections that include the peaks of EMG activity that we care about.

### Transforming

Transforming involves passing the filtered signal through a Fast Fourier Transformation (FFT).  The FFT will separate the signal into all the different frequencies that make up the signal and how much they each contribute to the signal.  This produces the power spectrum shown above.  In the halo python library, the file analytics.py contains a FFT included in the med_frequency function.  The med_frequency function takes 4 inputs, the signal, the sampling rate (fs), the precision (defaulted = 2) and the average (default = hist_median).  Since most of the time we are taking the median frequency, the type of average is defaulted to be the median, however, you can change this to suit your needs.

### Averaging

In this case, we are taking the median, the function med_frequency, after performing the FFT will call a function called hist_median, also found in analytics.py, which is simply a faster way to compute the median of the power spectrum.  At the end, the median will be returned and you will have a good measure of fatigue in your EMG signal.