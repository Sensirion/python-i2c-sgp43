# Python I2C Driver for Sensirion SGP43

This repository contains the Python driver to communicate with a Sensirion SGP43 sensor over I2C. 

<img src="https://raw.githubusercontent.com/Sensirion/python-i2c-sgp43/master/images/sensor_sgp41.jpg"
    width="300px" alt="SGP43 picture">


Click [here](https://sensirion.com/products/catalog/SGP41/) to learn more about the Sensirion SGP43 sensor.


Air Quality Sensor for VOC and NOx Measurements.



The default I²C address of [SGP43](https://sensirion.com/products/catalog/SGP41/) is **0x59**.



## Connect the sensor

You can connect your sensor over a [SEK-SensorBridge](https://developer.sensirion.com/sensirion-products/sek-sensorbridge/).
For special setups you find the sensor pinout in the section below.

<details><summary>Sensor pinout</summary>
<p>
<img src="https://raw.githubusercontent.com/Sensirion/python-i2c-sgp43/master/images/sgp41_pinout.jpg"
     width="300px" alt="sensor wiring picture">

| *Pin* | *Cable Color* | *Name* | *Description*  | *Comments* |
|-------|---------------|:------:|----------------|------------|
| 1 | red | VDD | Supply Voltage | 1.7V to 3.6V
| 2 | black | GND | Ground | 
| 3 | green | SDA | I2C: Serial data input / output | 
| 4 | blue | NC | Do not connect | 
| 5 |  | VDDH |  | Supply voltage hotplate; see data sheet on how to connect.
| 6 | yellow | SCL | I2C: Serial clock input | 


</p>
</details>


## Documentation & Quickstart

See the [documentation page](https://sensirion.github.io/python-i2c-sgp43) for an API description and a 
[quickstart](https://sensirion.github.io/python-i2c-sgp43/execute-measurements.html) example.


## Contributing

We develop and test this driver using our company internal tools (version
control, continuous integration, code review etc.) and automatically
synchronize the `master` branch with GitHub. But this doesn't mean that we
don't respond to issues or don't accept pull requests on GitHub. In fact,
you're very welcome to open issues or create pull requests :-)

### Check coding style

The coding style can be checked with [`flake8`](http://flake8.pycqa.org/):

```bash
pip install -e .[test]  # Install requirements
flake8                  # Run style check
```

In addition, we check the formatting of files with
[`editorconfig-checker`](https://editorconfig-checker.github.io/):

```bash
pip install editorconfig-checker==2.0.3   # Install requirements
editorconfig-checker                      # Run check
```

## License

See [LICENSE](LICENSE).
