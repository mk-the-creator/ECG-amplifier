This project focuses on the design and implementation of a low-cost ECG (Electrocardiogram) amplifier system used to measure the electrical activity of the human heart.

Electrode sensors are placed on the body to capture extremely weak heart signals (typically 0.1–5 mV). These signals are first conditioned using an AD8232 ECG sensor module, which performs initial amplification and signal stabilization.
To improve signal quality, the circuit includes a 50/60 Hz notch filter to remove power-line interference and a low-pass filter to eliminate high-frequency noise. Both filtering stages are implemented using LM741 operational amplifiers.

The cleaned ECG signal is then fed into an Arduino Nano, where the analog signal is digitized using the built-in ADC and displayed as a waveform. The output clearly shows P, QRS, and T waves, confirming proper heart signal acquisition.

The circuit was first simulated in LTspice to verify amplification and filtering behavior, followed by hardware implementation and testing. The system successfully produces stable and readable ECG waveforms.

Applications & Use Cases:
1)Basic heart-rate and rhythm monitoring
2)Educational demonstrations of biomedical signal processing
3)Low-cost and portable healthcare devices
4)Wearable and rural healthcare monitoring systems
