mongoDB.prefpane
================

Don't you love mongoDB. Don't you hate it literally drains your memory?

Well, mongoDB prefpane is a simple shortcut to start/stop the mongoDB daemon.

Installation
------------

* Clone the source and compile the source, then run the .prefpane generated.
* Download the compressed binary version from the downloads page

Updating
--------

It currently doesn't track updates with Sparkle, so you will need to come back later and download new versions.

Configuration
-------------

As of this version it will try to get the mongod binary from popular places (/usr/local/bin/mongod, /usr/bin/mongod, /bin/mongod/, /opt/bin/mongod). If for any weird reason you have it in a differnt location, you will need to set it in DaemonController.h.
i.e. @#define MONGOD_LOCATION @"/fruity/loops/mongod"@

If you need to set extra parameters to run mongod, then edit the Arguments textbox from the pane.

In development...
-----------------

* Redifined UI
  * Managing arguments is going to be nicer (not a simple text field)
  * Locating of the binary using a NSOpenPanel
  * Enable/disable start mongod on login

Known Issues
------------

It crashes System Preferences when re/installing the .prefpane.

Credits
-------

DaemonController and MBSliderButton based in the ones made by [Max Howell](http://github.com/mxcl)
