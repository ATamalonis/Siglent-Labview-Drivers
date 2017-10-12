# Siglent-Labview-Drivers
Drivers for Siglent Function Generators and Oscilloscopes
These files were written using National Instruments LabVIEW 2017

Building off the following Siglent Labview Driver Packages:
Siglent SDG 1000 5000 800 Series
Siglent SDS 1000 2000 Series

These Siglent Driver Packages were missing some basic function calls and some of the included calls needed modification. In this repository please find my additions and changes to these driver packages. These changes have been submitted to Siglent and National Instruments for review and inclusion in the certified driver packages.

Configure Clock Source.vi - Modified to return a boolean indicating if the clock setting was successful
Configure Standard Waveform Amp Only.vi - Modified to only update the Amplitude of the selected channel
Configure Standard Waveform Freq Only.vi - Modified to only update the Frequency of the selected channel
Enable Buzzer.vi - Turns on or off the audible buzzer
Enable Output Two Channel.vi - Wraps the "Enable Output.vi" in a for loop allowing a boolean array to be sent
Select Phase-Lock Mode.vi - Sets the phase-lock mode between the two channels - this feature was not documented in the VISA command documentation for the function generator at the time of writing this
