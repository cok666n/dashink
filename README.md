# DashInk
E-Ink Dashboard for HomeAssistant using ESPHome

## Description
This uses a ESP-Home device like the WaveShare ESP Board to drive a e-paper (e-ink) screen based dashboard for HomeAssistant

As this is not touch enabled, this focuses mainly in displaying useful information for the family. 
So far 2 sections are displayed, one is displaying current outdoors temperature, and the other displays thermostat informations for the whole house.

This is a work in progres and highly linked to my own setup, use it as inspiration only.

![image](https://github.com/user-attachments/assets/8438b4bb-9630-44f4-a2e8-f8cd92e163bd)

## Files
### dashink.yaml
Main esphome script, the display lamda is where most of the work happens

### secrets.yaml
You will need to provide your own secrets.yaml
```yaml
wifi_ssid: "Your SSID"
wifi_password: "Your Password"
api_key: "Your HA API key"
ota_password: "Your ota (HA)"
```

### sensors.yaml
This is a sample of how I setup my sensors in the HomeAssistant configuration.yaml file. You will need this in order to extract weather forecast data. 
