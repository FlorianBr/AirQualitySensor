# AirQualitySensor

ESP32 based Air Quality Sensor with sensors for temperature, humidity, pressure and air quality.
The data should be displayed on the LCD and also transmitted to Home Assistant for automations.

## Hardware

### Components

- ESP32+Display: [Guition GJC4827W543](https://github.com/lsdlsd88/JC4827W543)
- Temperature, Pressure, Humidity: GY-BME280-3.3
- CO2-Sensor: SCD41
- VOC-Sensor: GY-SPG40
- Particles: SDS011

## Software

A big todo. Not sure yet if esp-idf with MQTT connectivity or ESPHome.

## TODO

- [ ] Base Software
- [ ] SW Driver: BME280
- [ ] SW Driver: SCD41
- [ ] SW Driver: SPG40
- [ ] SW Driver: SDS011
- [ ] SW Driver: Display
- [ ] SW: Data acquisition
- [ ] SW: Data filtering and compensation
- [ ] SW: Display UI design
- [ ] SW: Display current data
- [ ] SW: Display historic data (graphs)
- [ ] SW: MQTT / HA connectivity
- [ ] HW: PCB / Wiring
- [ ] HW: 3D-printed case
- [ ] Documentation
