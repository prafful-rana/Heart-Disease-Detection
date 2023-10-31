This ECG signal is a Time-series. Hence, we perform Time-series classification with the
help of deep learning neural network. We aim to achieve this in three ways, One being
a 2D Convolutional Neural Network (2D-CNN), second being a 1D Convolutional Neural
Network (1D-CNN) and the third being a hybrid dual input network (2D-CNN & 1D-CNN
inputs). We perform the Feature Extraction using two methods, One is the Empirical Mode
Decomposition (EMD) and the second is the Fourier Decomposition Method (FDM). We
then compare the results obtained using both the methods.

<h1> Time Frequency Representation </h1>

A Time-Frequency representation (TFR) is a view of the signal, represented over both
time and frequency. TFRs are complex valued fields over time and frequency, with the
modulus representing the amplitude or energy density and the argument represents phase.
TFR representaion in this project is obtained by decomposing the signal into intrinsic band
functions and then we apply hilbert’s transform to obtain the corresponding TFR.
![dataset_sample0_nopad](https://github.com/prafful-rana/Heart-Disease-Detection/assets/56781776/7390d23e-0cdb-433a-ab9e-ede11fcac9d8)
![sample0_fdm_hht](https://github.com/prafful-rana/Heart-Disease-Detection/assets/56781776/dacc198a-bb70-471d-b2c4-ce48d942f141)

<h1>Empirical Mode Decomposition</h1>
It is an adaptive and efficient decomposition method capable of decomposing any complex signal into finite intrinsic mode functions. The Data itself dictates the decomposition. It is suitable for processing non-linear, non-stationary signal analysis. The decomposition
is accomplished using empirical bases termed Intrinsic Mode Functions (IMF’s) that satisfy
the following properties:
i) For the whole dataset, the number of extrema and number of zero crossings must either
equal or differ by atmost one.
ii) At any point, the mean value of the envelope defined by the local maxima and envelope
defined by local minima is zero.
Contrary to almost all previous signal analysis methods, this new method is intuitive, direct
and adaptive.
All the IMFs must satisfy two basic conditions:
(i) in the complete duration of time series, the number of extrema (i.e. maxima and minima)
and the number of zero crossings are equal or differ at most by one.
(ii) At any point of time in the complete duration of time series, the average of the upper
and lower envelopes, obtained by the interpolation of local maxima and the local minima,
is zero.
![no_padded_imf](https://github.com/prafful-rana/Heart-Disease-Detection/assets/56781776/fc9e2bb8-6936-4ffa-9fe8-afe8d5360def)
