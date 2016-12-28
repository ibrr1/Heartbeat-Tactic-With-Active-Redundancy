# Heartbeat-Tactic-With-Active-Redundancy

Contents of This File
----------------------

 * Description
 * Quality Attributes and More
 * Requirements and Installation
 * Setting Pacemaker Application 
 * Maintenance
 
Description
-----------
This is an example of applying one of the availability tactics for fault detection which is heartbeat tactic. In this example we have applied the heartbeat tactic with active redundancy in a pacemaker device.


Quality Attributes and More
---------------------------

Name: Pacemaker

Domain: Health Care 

RQ1: The Pulse Generator shall be available 99% of the time.

RQ2: The Pulse Generator shall sense the lack of heartbeat and generate a counter pulse 99% of the time back to the heart (DAQ).

Environment: while the pacemaker listens to regular patient heartbeat.

Response: Detect and generate messages to determine if the heart stopped for a minimum of time (0.5 milliseconds), generate an artificial pulse (stimulus) to the heart (DAQ).  

Response measure: Failure detected within a time interval of 0.5 milliseconds and the pacemaker generates artificial pulse and continues to listen to regular “heart” pulses.


Requirements and Installation
-----------------------------

- Python 3.4.3 
To download and install python go to:
https://www.python.org/downloads/

- PYRO4
To download and install PYRO4 go to:
https://pythonhosted.org/Pyro4/install.html


Setting Pacemaker Application
-----------------------------

1. Copy the application folder named HeartbeatProjectWithActiveRedundancy in your Desktop.

2. Open the command prompt.

3. Enter the HeartbeatProjectWithActiveRedundancy/

4. Type the following commands in any order in different consoles:
    pyro4-ns
    python3 pacemaker_active_node.py
    python3 pacemaker_redundant_node.py
    python3 heart_simulator/DAQ.py


Maintenance
-----------

If there is any problem in running the application, 
Please don't hesitate to contact us: 
- Ibrahim Aldosari: ima9428@rit.edu
- Cesar Armando Perez Fernandez: cap7879@rit.edu

