## System Specifications (SS)

### SS1 (Power Supply)
Must regulate own power from 9-12V supply.

- [X] 5 V Supply voltage
- [X] 3.3 V Supply voltage
- [X] LED ( [D6](./README.md) ) indicator

### SS2 (UART)
- [X] TX soldered
- [X] RX soldered
- [X] Configuration correct (8 data, 1 even parity bit, 1 stop bit & 57600 baud)
- [ ] [Formatted](./README.md#main) correctly
- [ ] Correct startup behaviour
- [ ] Handles & responds to commands

### SS3 (Ultrasonic sensor)
- [ ] Measures distance
- [ ] Measures up to 30 cm
- [ ] Detect whether object is < 10cm
- [ ] Flash LED ([D2](./README.md))


### SS4 (Accelerometer)
Unsafe driving: >0.5 g
Impact: >1.5 g
- [ ] Records measured acceleration
- [ ] Impact & unsafe driving detection
- [ ] LED ([D3](./README.md)) indicates unsafe driving(flashing) and impact(on)

### SS5 (Photodiode)
- [ ] Records light conditions
- [ ] Performs low light detection (< 300 lux)
- [ ] LED ([D4](./README.md)) flashes with low light warning
- [ ] Correct $R_f$ (feedback resistor) value for photo-current-to-voltage converter circuit

### SS6 (Temperature sensor)
- [ ] Records temperature
- [ ] Determines whether temperature > 30 C
- [ ] LED ([D5](./README.md)) flashes when high temp detected


### SS7 (Status LED's)
- [ ] Flash timing for status LED's is 500 ms ON and 500 ms OFF
- [X] Correct $R$-value used for series resistors (current must not exceed STM32's max)

### SS8 (Keypad)
- [X] Soldered keypad
- [ ] Implemented keypad
- [ ] Debouncing
- [ ] Pulldown resistors

### SS9 (LCD Display)
Waveshare 1602 LCD using Hitachi HD44780U controller?
Use pins PB1, PB11-PB15(Using BSRR register)

- [ ] LCD low level driver
- [ ] LCD high level driver
- [ ] Contrast resistors $R8$ and $R9$ give good contrast
- [ ] Menu navigation with [Keypad](###-SS8-(Keypad))
- [ ] [Ultrasonic sensor](###-SS3-(Ultrasonic-sensor)) warning message
- [ ] [Accelerometer](##-#SS4-(Accelerometer)) warning message
- [ ] [Photodiode](###-SS5-(Photodiode)) warning message
- [ ] [Temperature sensor](###-SS6-(Temperature-sensor)) warning message

### SS10 (SD card)
- [ ] SD card driver
- [ ] CSV
- [ ] Saves date & time
- [ ] Saves light intensity (lux)
- [ ] Saves temperature (Celcius)
- [ ] Saves distance (cm)
- [ ] Saves X, Y, Z acceleration, in g
- [ ] Saves warning condition states
- [ ] (Optional) Saves GPS coordinates

### SS11 (RTC)
- [ ] Keeps accurate time using RTC
- [ ] [Ultrasonic sensor](###-SS3-(Ultrasonic-sensor)) warning cooldown
- [ ] [Accelerometer](##-#SS4-(Accelerometer)) warning cooldown
- [ ] [Photodiode](###-SS5-(Photodiode)) warning cooldown
- [ ] [Temperature sensor](###-SS6-(Temperature-sensor)) warning cooldown

### SS12 (TIC)
- [ ] [Implements Test Interface connection](./README.md)
- [ ] Push buttons implemented

### SS13 (GPS)



 
