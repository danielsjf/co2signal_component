# CO2Signal platform for Home assistant
[Home Assistant](https://www.home-assistant.io/) platform for the [CO2Signal](https://www.co2signal.com/) website.

This platform extends the sensor component. To enable this platform, create a new file with the contents of `CO2Signal.py` in `<config>/custom_components/sensor/co2signal.py`.

Next, add the following lines to your `configuration.yaml`:

```yaml
sensor:
  - platform: co2signal
    token: SECRET
    country_code: BE
    refresh_rate: 15 # minutes between polling
```

The token can be found via the [CO2Signal website](https://www.co2signal.com/).

The custom component uses the [CO2Signal package](https://pypi.org/project/CO2Signal/) that can be found on pypi.
