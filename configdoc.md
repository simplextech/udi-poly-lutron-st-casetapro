# Configuring this node server

Enter the IP Address for your Caseta Pro bridge.  If
you have multiple systems connecting to your bridge you may (probably) will encounter
problems.

Devices can be added by clicking the 'Add Lutron Devices' button.  
Each device has 3 parameters to configure.
- Display Name in Admin Console
- Lutron Integration ID Number
    - Retrieved from Integration Report
- Device Type  

See below for the device type mapping information

If device type is not setup correctly the device will be created wrong or not at all.

### Device Types:

#### Pico Remotes
- 2 Button              = 4
- 2 Button Raise Lower  = 5
- 3 Button              = 6
- 3 Button Raise Lower  = 7
- 4 Button Pico         = 8

#### Switch / Dimmer
- Switch                = 10
- Dimmer                = 11
- Fan Controller        = 12

#### Shades
- Depends on requests