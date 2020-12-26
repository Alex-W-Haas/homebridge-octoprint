# homebridge-octoprint

Plugin to support [OctoPrint](https://octopi.octoprint.org) 3D printer control via the [HomeBridge Platform](https://github.com/nfarina/homebridge).

# Installation

1. Install homebridge using: npm install -g homebridge
2. Install homebridge-octoprint using: npm install -g homebridge-octoprint
3. Update your configuration file. See sample-config.json in this repository for a sample or below.

```
"accessories": [
    {
      "accessory": "OctoPrint",
      "name": "OctoPrint",
      "api_key": "XXXXX"
    }
]
```

# What does this plugin do?

This plugin adds the current print status of OctoPrint to HomeKit. The print status is shown as a lightbulb, with the brightness value equaling the current print progress (0-100%). If you deactivate the lightbulb, octoprint is instructed to abort the current print. Note, that print jobs cannot be started with this plugin (so activating the lightbulb does not do anything).

# Notes for implementation
Personal version for doing some testing on, as the master version does not work properly, and logs are currently insufficent.
