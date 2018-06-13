# homebridge-gpio-polling

Watches a GPIO pin. Reports state to Homebridge as a Motion Sensor. Simple.

This is special because:

- It uses polling rather than edge detection, since edge detection wasn't working well for your beloved author here
- We use BCM pin numbering

Sample configuration looks like:

```
{
    "accessory": "GPIOSensor",
    "name": "Motion",
    "pin": 26,
    "poll_interval": 100
}
```
