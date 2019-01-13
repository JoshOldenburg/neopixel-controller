- Weapon battery is 12S, voltage range is 30-51V
- Drive battery is 5S, voltage range 12.5-21V

H11L1
=====
- Forward current min: 2mA
- Forward current max: 60mA
- Forward voltage: 1.15-1.5V
- Max power: 120mW

Drive battery drop resistors
----------------------------
Resistor must drop 11-19.85V

### 1.5k
- Dropping 11V -> 7.3mA, 11mW in opto, 80mW in resistor
- Dropping 19.85V -> 13.2mA, 20mW in opto, 262mW in resistor

Weapon battery drop resistors
-----------------------------
Resistor must drop 28.5-49.85V

### 3.9k
- Dropping 28.5V -> 7.3mA, 11mW in opto, 208mW in resistor
- Dropping 49.85V -> 12.8mA, 19mW in opto, 638mW in resistor

Price
=====
Quantity 3: $7 for boards, $17 for components = $24/$8 each

Design Review Issues
====================
- Resistors will drop too much power. Use power resistors or multiple in series. FIXED - using through hole power resistors
- Can't use a BEC to power it as then you can have weapon motor power without indication when the drive motors are off. FIXED - will power off of 2xAAA again

ATTiny85
========
- .9V/1.8V digital on/off voltage at 3V supply
