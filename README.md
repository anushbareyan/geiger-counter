# Building the MIT LANPh Geiger-Muller Counter

This project was undertaken after completing the lectures of the Nuclear Detection workshop.For building the counter I followed the DIY Geiger Counter Instructions by Areg Danagoulian. 


The Geiger counter is a type of particle detector. It can detect hits from gammas – essentially ~MeV photons that come from nuclear decay in various radioactive materials that surround us.


## Step 1: Assembling the HV Module
To power the Geiger tube, I needed a high-voltage (HV) module. I built this module using a 555 timer and associated components to boost the 4.5V input to approximately 200V-300V. After assembling it, HV output needs to be tested using a voltmeter to ensure it falls within the expected range. 

Here is the completed HV module:

![photo1706619493](https://github.com/anushbareyan/geiger-counter/assets/122983285/23937921-f0c4-4716-8f23-99e675aa6a90)

## Step 2: Connecting Geiger Tube
For this, I soldered two bare wires to the clips that connect to the both terminals of the tube, then connecting it to the breadboard. 

![geig](https://github.com/anushbareyan/geiger-counter/assets/122983285/5dfa7f4f-defb-471e-8d07-dfe832fcb7ea)

## Step 3: Instrumenting the Geiger Counter with Arduino DAQ

Adding an Arduino microcontroller to digitize and process the analog signal from the Geiger tube.


## Step 5: Loading the Arduino sketch into the microcontroller

Transfering the given code to the Arduino device. This will connect the screen and it will turn on when connecting the battery.

![photo1706622214](https://github.com/anushbareyan/geiger-counter/assets/122983285/45f7b889-0735-48b6-9881-ca1dd0507540)

# Experiment: Attenuation of Gamma Rays

I conducted an experiment to investigate the attenuation of gamma rays as they interact with different materials. The goal of my experiment was to measure the transmission of gamma rays through lead and plastic materials and compare the results with theoretical predictions.

## Procedure

### Step 1: Background Measurement
- I ran the counter for 5 minutes to measure the background counts.
- I calculated the background rate in counts per minute (CPM) and its error.

### Step 2: Open Beam
- I placed the 60Co source about 10 cm away from the detector and measured for 5 minutes.
- I calculated the rate in CPM and its error.

https://github.com/anushbareyan/geiger-counter/assets/122983285/a9daacac-094a-4a7b-b611-dc238640b60f

### Step 3: Attenuation for Lead
- I repeated Step 2 with the lead absorber in place.
- I calculated the rate in CPM and its error.

### Step 4: Calculate Transmission
- I calculated the transmission using the values obtained in Steps 1-3.
- I determined the error using error propagation.

### Step 5: Compare to Theory
- I used XCOM tables to determine the theoretical transmission for 60Co gammas and lead.
- I compared the experimental results with the theoretical values with Z-score.

## Attenuation for Plastic and 137Cs
- I repeated the steps for plastic material and a 137Cs source.
- I determined the rate for open beam with 137Cs.
- I calculated the attenuated rate for plastic.
- I calculated the transmission and compared it with theoretical values with Z-score.

![Screenshot_20240130_175646](https://github.com/anushbareyan/geiger-counter/assets/122983285/82449a32-c670-498d-8ff5-010d8612abdc)
