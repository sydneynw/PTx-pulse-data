# PTx-pulse-data
This repository currently contains universally optimized RF pulse shapes and gradient waveforms of pTx pulses used in the paper __doi__  

In total, four pulses were generated, all of which are non-selective:

'UPcom_exc.mat' contains the waveforms for the 5°  excitation pulse for the commercially available 8Tx/32Rx coil (Nova Medical, Wilmington, USA)
'UPcom_inv.mat' contains the waveforms for the 180° inversion pulse for the commercially available 8Tx/32Rx coil (Nova Medical, Wilmington, USA)

'UPsb_exc.mat' contains the waveforms for the 5°  excitation pulse for the self-built 8Tx/32Rx coil (presented in:  https://doi.org/10.3389/fphy.2021.701330)
'UPsb_inv.mat' contains the waveforms for the 180° inversion pulse for the self-built 8Tx/32Rx coil (presented in:  https://doi.org/10.3389/fphy.2021.701330)

each '.mat' file consists of two arrays:

'RF' is a complex double matrix describing the RF/voltage waveforms for all transmit channels in volts ([V]).
	the first dimension describes the temporal evolution with a sampling time of 10 µs
	the second dimension counts the transmit channels, see the other image 'Tx_element_numbering.png' 

'G' is a double matrix describing the gradient waveforms for all three gradient coils in gauss per centimeter ([G/cm])
	the first dimension describes the temporal evolution with a sampling time of 10 µs
	the second dimension counts the gradient coils, which generate gradients in (1) left-right or x (2) anterior-posterior or y (3) head-feet or z direction 
	
