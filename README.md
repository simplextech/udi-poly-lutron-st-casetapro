# udi-poly-lutron-casetapro

Lutron Caseta Pro NodeServer for Polyglot

- Polyglot V2 (On-premise installation).
- Testing Platform
    - ISY FW 5.3
    - Polisy Polyglot 2.2.9
    - Lutron Caseta Pro bridge

To get started with an on-premise installation: 
- NodeServer is availble in the Polyglot Store

[Caseta Pro Information](https://www.casetawireless.com/proproducts)


### Currently Supported Components
- Dimmer
- Switch
- Pico Remotes
    - 2 Button
    - 2 Button Raise/Lower
    - 3 Button
    - 3 Button Raise/Lower
    - 4 Button

### Scenes / Phantom Buttons
- Caseta Pro provides access to Scenes via the Phantom Button methodology of RadioRa 2.  The phantom
button control is directly available from the main repeater/bridge node.  Scenes must be referenced by the
phantom button number and can be retrieved from the Integration Report.
- If there is demand Scenes may be converted into node elements within the Admin Console.

### In-Development Components
- Shades
    - Pending testing/information

## Notes

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