# udi-poly-lutron-st-casetapro

Lutron NodeServer for Polyglot

- Polyglot V2 (On-premise installation).
- Testing Platform
    - ISY FW 5.3
    - Polisy Polyglot 2.2.9
    - Lutron RadioRA 2 Main Repeater 12.8.0
    - Caseta Pro bridge

To get started with an on-premise installation: 
- NodeServer is availble in the Polyglot Store

[Lutron Caseta Pro Information](https://www.casetawireless.com/proproducts)

### Currently Supported Components
- Dimmer
- Switch
- Pico Remotes
    - 2 Button
    - 2 Button Raise/Lower
    - 3 Button
    - 3 Button Raise/Lower
    - 4 Button

### In-Development Components
- Shades
    - Pending demand

## Notes
- Keypad raise/lower functionality is not presented to the Admin Console as there's no percentage of scene status available to manipulate.

# Configuring this node server
- Multiple Control systems connecting to a main repeater or bridge using the same username/password is not supported by Lutron and will cause the main repeater/bridge to lock down the connection requiring a time-out period of 15 minutes or power cycle!

## Caseta Pro
- Default username and password are lutron/integration and are the defaults for the NodeServer.
- Telnet Support must be enabled from the mobile app
  - Settings -> Advanced -> Integration -> Telnet Suport
- The Integration Report is accessible from the mobile app.
  - Settings -> Advanced -> Integration
- The Lutron Integration Protocol does not report status of Occupancy sensors for Caseta Pro.  Occupancy sensors added as devices will not report status.
- Pico remotes are the only keypad available for Caseta Pro.

## Adding Devices
- Devices are added by clicking the 'Add Lutron Devices' button.
- Three parameters to configure.
  - Display Name in Admin Console
  - Lutron Integration ID Number
  - Retrieved from Integration Report

# Device Type Mapping Information
- If device type is not setup correctly the device will be created wrong or not at all.

## Device Types:
| Device    | Value |
|-----------|-------|
| Pico 2 Button                     | 4 |
| Pico 2 Button Raise / Lower       | 5 |
| Pico 3 Button                     | 6 |
| Pico 3 Button Raise / Lower       | 7 |
| Pico 4 Button                     | 8 |
| Maestro / Caseta Switch           | 10 |
| Maestro / Caseta Dimmer           | 11 |
| Meastro / Caseta Fan Controller   | 12 |
| Sivoia QS Wireless Shades         | 30 |
