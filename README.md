# Openshutter
Open source laser shutter


Laser shutters are expensive (~1000 pounds) for the kind of devices they are. So we are implementing an open source version of it.

Here are the parts one needs to buy from Thorlabs to get a working shutter:

https://www.thorlabs.com/thorproduct.cfm?partnumber=SC10
https://www.thorlabs.com/thorproduct.cfm?partnumber=SH05/M
https://www.thorlabs.com/thorproduct.cfm?partnumber=TC200CAB10

The project can be broken down into 3 parts:

Electronic control:
 - receive 5V pulses to open shutter (figure out max on/off frequency)
 - get feedback from optosensor on shutter to know if shutter is open or closed
 - have a hard key to enable/disable shutter
 - control more then one shutter 
   - (maybe with delay control in between shutters to increase on/off frequency? if shutters are closing in oppposite directions?)
 
Mechanical shutter:

- based on solenoid
- if no power is present, shutter closes and laser bean is interrupted
- capable of opening/closing at least 10mm window (circle or square, not important)

