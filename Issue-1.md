## Issue-1

In the simulation of [2-node-network.groovy](Source_Code/2-node-network.groovy) in unet-3.1.0, shell browser for node 1 and 2 looks as follows,

<p align="center">
  <img src="Images/Node-1.png" width="450" /> 
  <img src="Images/Node-2.png" width="450" /> 
</p>

notice the difference, in node 1 shell window (down) "Dashboards" is missing

## Reason

This happens when you are using unet-3.1.0 along with unet-3.0.0 previously available in your system. The port number is occupied by the web server (Jetty) instance running with unet-3.0.0. 

## Solution

Change the port number of node-1 (or the node, which is not running properly), to change the port number, open the simulation script, locate the statements written for node deployment. In the line for deployment of node-1, change the port number given as value for the 'web' property of the node. (in this case change from 8081  to 8083 or something)
