While putting together our project, we initially started by taking the Raspberry PI out of the kit and setting it up. After attaching the needed heat syncs, and accesories to make
it capable of being controlled including a keyboard, monitor, mouse, and ethernet. Then we began the main setup of the Raspberry PI. We installed the PI OS into a micro usb we
bought off amazon using a micro usb to usb adapter. Setup in this regard was fairly easy. We had to change the default password after reading the notification that hackers
actively watched the BU network looking for new Raspberry Pi's and other unsecured systems and quickly reformatted the password to something sufficiently complex. We then began
the process of installing python and the necessary libraries in the PI.

In the process of setting up the Pi, we ran into difficulties regarding libraries that were needed however we were able to figure out which were missing and install them. To
generate the data we ran the code wifi_scan.py. wifi_scan.py scans for wifi signals a set number of times and saves the data in json format to a file. We were unaware that
plotting our data, which was retrieved in the lab by the highway, was not possible on the Pi, and had to first be transferred to a laptop. We noticed this after the date format
kept returning date errors and after we could not figure out why we checked Github. We realized this was due to the fact the code was not linux friendly. Once this was done
however we downloaded the necessary python libraries to our personal laptop and ran wifi_plot.py from there. At this point the code ran correctly due to being on a windows system
and getting the graph was fairly easy. A photo is attached below.





![image](https://user-images.githubusercontent.com/86809648/133538111-bb279fff-789a-4ec7-9d41-022bf3a9b264.png)

A good use for this system is to detect the wifi signals from passing cars over time. For example if the raspberry pi was run for longer periods of time we could collect and report traffic data upt year long scales. This info could then be used to figure out peak traffic times and help city planners figure out good times for road repairs so it isn't during a busy time period, without needing someone to count the traffic going by.  
