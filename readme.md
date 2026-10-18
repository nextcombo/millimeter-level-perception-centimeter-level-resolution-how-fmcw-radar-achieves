# Millimeter-level perception, centimeter-level resolution: How FMCW radar achieves precise target detection [with MATLAB code]

Millimeter-level perception, centimeter-level resolution: How does FMCW radar achieve precise target detection? In the fields of intelligent driving, traffic monitoring, industrial security, and smart home, there is a sensor that is becoming the "core perceptual pivot."
It is not afraid of the night, fearless of rain and fog, and does not interfere with dust. It can measure the distance, speed and direction of the target in real time, achieving all-weather, high precision, non-contact detection.
It is ——FMCW Frequency Modulated Continuous Wave Radar.
Today's article, we will not discuss code or formulas; instead, we will use plain language to guide you through the complete logic of FMCW radar from signal emission to target positioning.
1. What is FMCW radar? FMCW, abbreviated as Frequency-Modulated Continuous-Wave, stands for Frequency-Modulated Continuous-Wave radar.
Simply put, its working method is very intuitive:
Continuous electromagnetic wave with linearly varying frequency
Receive the echo signal reflected back by the target.
Compare the frequency difference between transmitted and echo signals.
Directly solve for: distance, speed, angle from the frequency difference.
It belongs to short-range real-time measurement radar, which is particularly suitable for traffic monitoring, vehicle assistance, security detection and other scenarios.
II. Four Key Indicators Determining Radar Performance
1  
The distance resolution can distinguish the two closest targets. The distance resolution is determined by the signal bandwidth, and the wider the bandwidth, the finer the detail.
2  
The maximum detection distance system can stably detect the farthest distance.
3  
Speed resolution and maximum speed distinguish the precision of slow-moving targets, as well as the highest speed that can be measured.
4  
The ability to discern the orientation of targets under the angle resolution of a multi-antenna array.
In typical traffic monitoring scenarios, the following indicators are commonly used:
Distance resolution: 0.3 meters
Maximum detection distance: 300 meters
Maximum speed: 200 km/h
Speed resolution: 1.56 km/h
Antenna channel: 16
III. From Signal to Target: A Complete FMCW Processing Flow
FMCW radars do not "see" targets directly; instead, they convert electromagnetic waves into recognizable information through a standard process.
1. System Parameter Design: Start by calculating the key working parameters of the entire system based on requirements: signal bandwidth, sweep duration, sweep slope, maximum differential frequency, sampling rate, and number of sample points. This step determines the accuracy and range of the radar.
2. Building a Three-Dimensional Signal Cube: The radar echo forms a three-dimensional signal body:
First dimension: Range (fast time)
Second dimension: Speed (slow time)
Third dimension: Angle (multiple antenna channels) – each data point contains the complete information about the target.
3. Three-Dimensional FFT Spectral Analysis: This is the core step of FMCW. Through three-dimensional fast Fourier transform, the time-domain signal is converted into the frequency domain:
One-dimensional FFT → Extract distance
Two-dimensional FFT → Extract distance + speed
Three-dimensional FFT → Extract distance + speed + angle
A single transformation simultaneously obtains three key parameters.
4. Peak Detection: Locate the peak in the true target spectrum, which corresponds to the real target. The system automatically searches for peaks, eliminates noise, and precisely locates each target.
5. Multi-dimensional Visualization: Finally, draw the data into an intuitive map:
Distance-Speed Heatmap
Distance-Angle Heatmap
One-dimensional Distance/Speed/Angle Spectrum Line
Polar coordinate space orientation plot
Turning invisible signals into clearly visible monitoring results.
IV. Why Logarithmic Amplitude? You might notice that most radar spectra perform logarithmic (amplitude) processing.
The reason is simple:
Signal strength differences between targets are enormous
Direct drawing would lose details of weak targets
By taking logarithms, weak signals are "amplify", making details clearer
This is the standard operation for visualizing radar signals.
V. How to Identify Multiple Targets with One Probe? FMCW radar supports simultaneous detection of multiple targets.
The system can superimpose multiple target echo signals, forming multiple independent peaks in the spectrum, each corresponding to a target, without interference.
In typical demonstration scenarios:
Target 1: Distance 100 meters, speed -50 km/h, angle -60°
Target 2: Distance 200 meters, speed +75 km/h, angle +45°
Both radars can clearly distinguish and precisely output them.
VI. FMCW Radar: The "Perceptual Eye" that is everywhere because of its high accuracy, low cost, and strong environmental adaptability. FMCW has permeated all industries:
Intelligent driving: Vehicle range measurement, speed measurement, collision warning
Traffic monitoring: Speed, traffic volume, vehicle type recognition
Intelligent security: Area invasion, human presence perception
Industrial control: Level, material level, displacement measurement
Smart home: Human sensor, breathing monitoring
It is one of the most cost-effective solutions for near-field perception at present.
VII. Core advantages of FMCW radar✅ All-weather operation: Unaffected by rain, fog, dust, darkness✅ Three parameters synchronous measurement: Distance, speed, angle obtained at once✅ High precision: Centimeter-level distance, Kilometer-level speed accuracy✅ Low cost and easy mass production: Simple structure, suitable for large-scale implementation✅ Real-time strength: Fast processing, suitable for dynamic monitoring
Conclusion: From electromagnetic wave emission to three-dimensional FFT analysis, and then to peak detection and visualization presentation - FMCW radar uses a rigorous and efficient signal processing process to turn invisible signals into perceivable, applicable, and grounded target data.
It is not just a sensor but also a pair of precise eyes that perceive the world for machines.
In the future, with the continuous development of autonomous driving, Internet of Things, and intelligent transportation, FMCW radar will enter more scenarios, silently guarding safety and efficiency.
Radar principle explanation
Algorithm and engineering application
Latest industry trends and cases
💬 Leave a message: Which type of radar technology do you want to know more about?

## Images

![Millimeter-level perception, centimeter-level resolution: How FMCW radar achieves precise target detection [with MATLAB code]](01.jpg)
![Millimeter-level perception, centimeter-level resolution: How FMCW radar achieves precise target detection [with MATLAB code]](02.jpg)
![Millimeter-level perception, centimeter-level resolution: How FMCW radar achieves precise target detection [with MATLAB code]](03.jpg)
![Millimeter-level perception, centimeter-level resolution: How FMCW radar achieves precise target detection [with MATLAB code]](04.jpg)
![Millimeter-level perception, centimeter-level resolution: How FMCW radar achieves precise target detection [with MATLAB code]](05.jpg)
![Millimeter-level perception, centimeter-level resolution: How FMCW radar achieves precise target detection [with MATLAB code]](06.jpg)

<!-- PAYMENT_BLOCK -->

## Get this dataset

- Payment link (Stripe): [Buy now](https://buy.stripe.com/3cs8yP7sY87d0vu9AB)
- Payment QR code: ![Payment QR code](pay.png)

<!-- /PAYMENT_BLOCK -->
