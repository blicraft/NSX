# NSX
Upgrading from ESXi 6.0 to 6.5 with NSX in the environment.
According to VMware’s documentation you need to do a 1 by 1 upgrade of all hosts in a cluster. That means you are not able to run VUM and remediate a cluster.  That’s lame and there has to be a better way. So, this is how I got around that problem. I built a custom ESXi 6.5 image and had the VXLAN VIB injected into it. 
Step one: Start the Auto Deploy and Image Builder services in your vCenter. You do this by going to Home  Administration  Deployment, System Configuration  Services  
