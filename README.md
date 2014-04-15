ninja-presence-ping
===================

FORK: this fork uses the state device to track the number of devices detected by ping and uses the standard log object

This is a ping presence driver for your own Ninja Block (http://ninjablocks.com)

To install the easy way you'll need the ninja toolbelt. (https://github.com/ninjablocks/ninja-toolbelt for instructions)

install commando: `ninja install https://github.com/svrooij/ninja-presence-ping`

or install clonning this repo into your ninjablocks drivers folder, then run `npm install`

This driver will create two devices, one with the raw data as devices respond to a ping. And one generic state device that will update to the number of devices detected (0,1,2,...)
So you should be able to use those in your threshold rules!!

For everyone who likes this driver, you can also use this widget (https://gist.github.com/svrooij/6974775)

*************
To-do
=====

- [x] Create a [gist](https://gist.github.com/svrooij/6974775) for display
- [x] Add state device for using the presence in the rules engine
- [x] Enable configuration of host trough the settings, instead of the 'edit the index.js file' way
- [x] Rewrite the sub driver
- [x] Moved main state logic to ninja-presence-base
- [ ] Add a device per host, for even better control of the rules
