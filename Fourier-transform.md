[Fourier transform](https://en.wikipedia.org/wiki/Fourier_transform)

**Fast Fourier Transform**

[FT vs PSD](http://www.dsprelated.com/showthread/comp.dsp/109448-1.php)

**NUFFT (Nonunifrom Fast Fourier Transform)** FFT of unevenly spaced / irregularly spaced / nonequispaced sampling / data
[StackExchange Forum](http://scicomp.stackexchange.com/questions/593/how-do-i-take-the-fft-of-unevenly-spaced-data)
[Greengard and Lee (2004) Accelerating the Nonuniform
Fast Fourier Transform](http://math.nyu.edu/faculty/greengar/glee_nufft_sirev.pdf)
"When sampling is uniform, the fast Fourier transform (FFT) allows this calculation to be computed in O(N log N) operations rather than O(N^2) operations. Unfortunately, when the sampling is non-uniform, the FFT does not apply."

**Sampling**
* Increasing sampling rate raises the Nyquist Frequency (the highest frequency that can be resolved without aliasing) but does not improve resolution at lower frequencies
* Increasing the number of samples (at the same sampling rate) improves the frequency domain resolution of the fourier transform

> Adding additional samples will improve the frequency domain resolution of our estimate and sampling at a finer rate will change the Nyquist frequency, the highest frequency for which the spectrum can be estimated. [W.H. Press, S.A. Teukolsky, W.T Vetterling and B.P. Flannery (2007) Numerical Recipes: The Art of Scientific Computing. Cambridge: Cambridge University Press. 3rd Ed.]

## Related
[windowing function](https://en.wikipedia.org/wiki/Window_function)
inverse Fourier Transform / Fourier Synthesis
[uncertainty principle](https://en.wikipedia.org/wiki/Fourier_transform#Uncertainty_principle)
[hermitian function](https://en.wikipedia.org/wiki/Hermitian_function)
[[detrendng]]
[auto-spectrum](http://www.gaussianwaves.com/topic/whats-the-difference-between-autospectrum-and-power-spectrum-densitypsd/)
cross-spectrum
[[Thomson's Multitaper Method]](http://nipy.org/nitime/examples/multi_taper_spectral_estimation.html#nr2007)

## Evaluation
* [FWHM, Full Width at Half Maximum](https://en.wikipedia.org/wiki/Full_width_at_half_maximum)
 * FDHM - Full Duration at Half Maximum (when ind. variable is time)
 * HWHM - Half duration at half maximum

## Names, Abbreviation, Misnomers, Similar
* [Fast Fourier Transform, FFT](https://en.wikipedia.org/wiki/Fast_Fourier_transform)
* [Discrete Fourier Transform, DFT](https://en.wikipedia.org/wiki/Discrete_Fourier_transform)
* [[spectral density]]
* [Power Spectral Density, PSD](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-011-introduction-to-communication-control-and-signal-processing-spring-2010/readings/MIT6_011S10_chap10.pdf)