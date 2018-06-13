# homebridge-gpio-polling

Fork note: Uses polling (100msec default, override with config.poll_interval) rather than edge detection, since edge detection wasn't working well for your beloved author here.

This Homebridge plugin exposes itself as a motion sensor, and passes through if the monitored pin is high or low.

We use BCM pin numbering here rather than RPi or otherwise.

Sample configuration looks like:

```
{
    "accessory": "MotionSensor",
    "name": "Motion",
    "pin": 26,
    "poll_interval": 100
}
```
