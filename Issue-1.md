## Issue-1

In the simulation of [2-node-network.groovy](Source_Code/2-node-network.groovy) in unet-3.1.0, shell browser for node 1 and 2 looks as follows,

<p align="center">
  <img src="Images/Node-1.png" width="450" /> 
  <img src="Images/Node-2.png" width="450" /> 
</p>

notice the difference, in node 1 shell window (down) "Dashboards" is missing

## Reason

The port number is occupied by the web server (Jetty) running with unet-3.0.0

## Solution
