Syndicate CloudVPN Scripts
==========================

These are a collection of initscripts (and eventually maybe some other junk) for the Yasashii
Syndicate's CloudVPN deployment.

Files
----------

* cloudvpn-ys = bring up the client and the tap interface
* brige-ys = br0 setup (make sure shorewall is configured for br0 and not eth1 or shit breaks)

Installation
---------------

Under Ubuntu, copy the scripts to /etc/init.d and run these commands:

	sudo update-rc.d cloudvpn-ys defaults 80 20
	sudo update-rc.d bridge-ys defaults 90 10
