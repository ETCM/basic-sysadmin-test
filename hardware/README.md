Hardware Requisition, Provisioning and Trouble-Shooting
=======================================================

Answer the following questions.

Q1) What is the difference between a RAID adapter and an HBA?
-------------------------------------------------------------
Host bus adapter (HBA) is a device performs I/O between a server and storage devices. It physically connects the two as well.
A RAID adapter is essentially a RAID controller. It's primary purpose is to allow a computer to view multiple disk as single logical disks for purposes such as redudancy. 

Q2) Switch, Hub, Router. Compare and Contrast.
----------------------------------------------
A hub is a layer-1 device that acts as a single network segment and can only serve to repeat a signal. It can be used to connect multiple cable segments. Hubs have no addressing mechanism so all traffic on the segments can be seen by other devices connected to the same hub. 

A switch is a layer-2 device that passes traffic just like a hub but has the ability to route packets to their destination using the MAC address. This allows switches to more efficiently route traffic as opposed to a hub that does not know the destination of the packet it is sending. Switches also learn where packets should be sent after by cache addresses within their MAC address table. This makes allows the network route traffic more quickly.

A router is a layer-3 device that passes traffic similar to a hub and switch. Routers are able to route traffic between different networks. Routers can use IP addressing to route traffic. They have the ability to perform Network Address Translation as well. Routers have the most features out of all three of these devices because they operate at a higher protocol. 

Q3) What matters when deciding between hardware and virtualized machines?
-------------------------------------------------------------------------
When considering whether to use a hardware or virtulized platform the main factors to take in to account are the number of servers needed, the cost of hardware, the amount of physical storage needed, any compliance issues that require physical seperation of assets and factors such as high availability(SAN).

Virtualization can save money in power costs and hardware but may not always be the best solution if the environment needs dedicated processing power.

Q4) On a $6000 budget, spec out a stand-alone storage server.
-------------------------------------------------------------
I'd have to request more information in order to properly spec out the server. At this point I know that it is a storage server but do not know if it will be a high volume of times, what it will be storing and if it will be used for any purposes such as disaster recovery.

Q5) How would you provision the previous machine for production?
----------------------------------------------------------------
See Q4 response.

Q6) Scenario 1:
---------------
Write through-put on your storage server is falling. How would you diagnose the issues?
I would start by checking for any problems with the I/O controller and also make sure that no drives within any array have gone bad. Next I'd set up some sort of performance monitoring to look for any trends that may be present.

Q7) Scenario 2:
---------------
The storage volume is filling up. You have four calendar weeks and $3000. Requisition and provision new hardware. Downtime on the storage must be kept below 5 minutes. Don't let the storage volume hit the cap.

Once again I'd need additional information so that I could match the previous storage volumes. I'd try to set up some sort of data mirroring from the old volume to the new volume so that once the data is mirrored, the old volume can be shut down with minimal downtime for the end users.
