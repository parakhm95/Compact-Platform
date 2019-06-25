Configuring the PX4 stack
==========================

Change the following parameters in the PX4 stack:

Circuit breakers parameters - Bypass safety
--------------------------------------------
#. CBRK\_IO\_SAFETY : 22027 | Disable arming check for safety switch.
#. CBRK\_SUPPLY\_CHK : 894281 | Disable the arming check for voltage/power for battery in case the power module is not connected.
#. CBRK\_USB\_CHK : 197848 | Disable the arming check for USB cable being plugged-in.

*Note* : Do not disable USB check mentioned above without knowing what you are doing. This check was disabled for easy diagnosis of the errors on the platform.

PID and Noise-filter parameters
--------------------------------


Tuned the Low-pass filter using `filter tuning guide`_ and settled on 80Hz for IMU\_GYRO\_CUTOFF and 45 Hz for MC\_DTERM\_CUTOFF. Make sure PID-Gains are very low so that the noise doesn't originate from the control loop.

*Note* : Set the hover throttle parameter MPC\_THR\_HOVER to the throttle needed for hovering or the vehicle will not hold altitude. Issue referenced `here`_.


#. IMU\_GYRO\_CUTOFF : 80 | Noise filter cutoff.
#. MC\_DTERM\_CUTOFF : 45 | Noise filter cutoff.
#. IMU\_GYRO\_CUTOFF : 80 | Noise filter cutoff.
#. MC\_DTERM\_CUTOFF : 45 | Noise filter cutoff.
#. MC\_PITCHRATE\_D : 0.001
#. MC\_PITCHRATE\_I : 0.027
#. MC\_PITCHRATE\_P : 0.04
#. MC\_PITCH\_P : 5.5
#. MC\_ROLLRATE\_D : 0.001
#. MC\_ROLLRATE\_I : 0.027
#. MC\_ROLLRATE\_P : 0.04
#. MC\_ROLL\_P : 5.5
#. MC\_YAWRATE\_I : 0.06
#. MC\_YAWRATE\_P : 0.1
#. MC\_YAW\_P : 2.3

Rangefinder parameters : Garmin Lidar Lite v3 or Maxbotix MB1242 
----------------------------------------------------------------

#. SENS\_EN\_LL40LS : 2 | Enable the Garmin Lidar Lite v3 on $I^2C$.
#. EKF2\_HGT\_MODE : 2 | Selecting the rangefinder as the primary height sensor.
#. EKF2\_MIN\_RNG : 0.05 | Minimum sensing distance for Garmin Lidar Lite v3. 
#. EKF2\_RNG\_AID : 1 | Enabling range aid for takeoff and landing.
#. MPC\_THR\_HOVER : 0.3 - 0.4 | 30\% throttle for a 3:1 power-to-weight ratio of the robot. Verify in manual mode.
#. SENS_EN_MB12XX : 1 | Enable the Maxbotix MB1242 sonar.

Logging parameters
-------------------

#. SDLOG\_MODE : 1 | Log from boot to disarm - Used for error detection.
#. SDLOG\_PROFILE : 91
#. SDLOG\_UTC\_OFFSET : -240 | 4 hours or 240 mins behind UTC.

.. _filter tuning guide: https://docs.px4.io/en/config_mc/racer_setup.html#filter-tuning
.. _here: https://github.com/PX4/Firmware/issues/12180