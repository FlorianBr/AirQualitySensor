# AirQualitySensor

ESP32 based Air Quality Sensor with sensors for temperature, humidity, pressure and air quality.
The data should be displayed on the LCD and also transmitted to Home Assistant for automations.

## Hardware

### ESP32

- IO0 - x
- IO1 - LCD Backlight
- IO2 - Speaker LRCLK (?)
- IO3 - Touch Int
- IO4 - Touch CSL (?)
- IO5 - 
- IO6 - 
- IO7 - 
- IO8 - Touch SDA (?)
- IO9 - 
- IO10 - CS (?)
- IO11 - Touch MISO
- IO12 - Touch CLK
- IO13 - Touch MOSI
- IO14 - 
- IO15 - 
- IO16 - 
- IO17 - U1 TXD
- IO18 - U1 RXD
- IO19 - USB+
- IO20 - USB-
- IO21 - LCD QSPI D0
- IO38 - Touch CS
- IO39 - LCD QSPI D3
- IO40 - LCD QSPI D2
- IO41 - Speaker DIn
- IO42 - Speaker BCLK
- IO43 - U0 TXD 
- IO44 - U0 RXD
- IO45 - LCD CS
- IO46 - 
- IO47 - LCD QSPI CLK
- IO48 - LCD QSPI D1


### Display

- 480x272 pixel, 16 bit color
- Driver: [NV3041A](https://admin.osptek.com/uploads/NV_3041_A_Datasheet_V1_2_20221011_686486a221.pdf)
- Touch Panel: XPT2046

### Components

- ESP32+Display: [Guition GJC4827W543](https://github.com/lsdlsd88/JC4827W543)
- Temperature, Pressure, Humidity: GY-BME280-3.3
- CO2-Sensor: SCD41
- VOC-Sensor: GY-SPG40
- Particles: SDS011

## Software

Not sure yet if I'll use the esp-idf with MQTT connectivity or the easier but muuuch more limited ESPHome.
I guess I'll try both and start with ESPHome while waiting for the ordered sensor boards.

## TODO (ESPHome)

- [x] Basic yaml
- [x] Display
- [x] BME280
- [ ] SPG40
- [ ] SCD41
- [ ] SDS011

## TODO (esp-idf)

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
