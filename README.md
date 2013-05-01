# unplug2shutdown

A python tool to shutdown your computer by removing an USB device.

Originally intended to be run on RaspberryPi to prevent brutal shutdown.

## Dependencies

 - GObject python bindings;
 - GUdev python bindings;

**Debian and derivatives**

	sudo apt-get install python-gobject python-gudev

## Installation and usage

This tool is at a **very early stage**, there's no installer yet so here's the deal:

1. run **as root**:

		/path/to/unplug2shutdown.py --configure
2. 	follow the instructions. Basically you'll need to plug the device that you want to use as a shutdown handler;
3. 	run the tool as root at startup:

		/path/to/unplug2shutdown.py &
4. unplug the device and look at the magic;	

Any **feedback** or **pull requests** are welcome.


## Uninstall

No installer yet, no uninstaller yet. Remove downloaded files and the configuration file:

	/root/.unplug2shutdownrc

## License

Apache License  
Version 2.0, January 2004

See LICENSE

## Author(s)

Claudio "Dawson" d'Angelis <claudiodangelis@gmail.com>  
http://claudiodangelis.com
