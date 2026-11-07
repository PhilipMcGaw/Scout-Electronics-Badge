# Arduino sensor data logging

## Working title

How to make sensor readings useful after you collect them

## Audience and scope

An adult-facing introduction to logging low-voltage sensor readings with a microcontroller. Use the source project as inspiration, not as a verified wiring guide. Keep exact board, shield, sensor, circuit and code choices open until their documentation is checked.

## Draft

A sensor reading is more useful when you can compare it with earlier readings. A data logger takes measurements at chosen intervals and saves them so they can be inspected later. A simple project might record temperature and light, then save each set of readings to a file on a memory card.

### Decide what each row should tell you

A useful record needs more than two numbers. Include a timestamp or elapsed time, the sensor readings, and units where they apply. A CSV file can be opened by many spreadsheet programs, but the first line should label each column, for example `time_s,temperature_C,light_adc`. Document the sampling interval and sensor setup as well. Without this context, a file of values can be difficult to interpret later.

### Readings are not automatically measurements

An analogue input converts a voltage into a number within the range and resolution supported by the selected board. That number is not automatically a temperature or a light level. The conversion depends on the sensor circuit, analogue reference, board and calibration.

For example, an LM335-family sensor produces a voltage related to absolute temperature and needs the operating circuit described in its datasheet. A photoresistor’s resistance changes with light, but a divider and analogue input give a relative reading; that alone does not make a calibrated lux meter. Record raw readings first, and only convert them using a checked sensor model, circuit and calibration method.

### Choose how to save and time the data

An SD card can hold a larger log than a microcontroller’s small built-in memory. The card interface may use SPI pins that are also used by other shields, so check the exact board and shield pin assignments, logic levels and supply requirements. Do not assume every SD module is safe to connect directly to every board.

If calendar time matters, use a real-time clock and check its backup power and accuracy. If elapsed time is enough, a running timer may be simpler, but it can reset when power is lost and its accuracy depends on the board. Test how often the logger writes data and what happens if power is interrupted; buffering data and writing in batches can affect both reliability and storage use.

### Make the log trustworthy

Choose a sampling interval that suits the change being observed. Very frequent samples create larger files and may record noise rather than useful changes. Keep the sensor away from heat sources or direct handling if those would distort the reading. Compare sensor values with a suitable reference when accuracy matters, and note any correction applied.

Before relying on a logger, check that it writes a file with clear column names, consistent units and expected timestamps. Open the saved file and inspect several records, including what happens around start-up and a power interruption. Treat these as design checks to perform, not as results claimed for the source project.

## Editorial and source notes

- Duino4Projects, [“Datalogger With Temperature Sensor and Photoresistor”](https://duino4projects.com/datalogger-with-temperature-sensor-and-photoresistor/), dated 2019-10-24 in indexed text. The page could not be fetched directly in this review; search-index text describes an Arduino Uno, Ethernet shield, microSD card, LM335Z and photoresistor. Treat it as an idea source only. Do not reuse its images, wiring diagram or code without checking the original source and reuse rights.
- Texas Instruments, [LMx35/LM335 datasheet](https://www.ti.com/lit/gpn/lm335). Check the exact sensor variant, operating current, circuit, calibration and conversion before including a temperature example.
- Arduino, [UNO R3 documentation](https://docs.arduino.cc/hardware/uno-rev3) and [SD card datalogger example](https://docs.arduino.cc/tutorials/mkr-eth-shield/mkr-eth-shield-user-manual/). These show board-specific ADC and SD logging context; confirm the exact hardware before adapting any pin or code example.
- The post should remain a general outline until a specific board, SD interface, sensor circuit and timekeeping method are selected and verified.
