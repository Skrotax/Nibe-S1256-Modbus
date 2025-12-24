Just how i set up my Nibe S1256 heatpump.
Did not like the +700 unused entities that the integrated Nibe produces.
I copied mkaiser´s modbus_sungrow.yaml and replaced the solar sensors with Nibe sensors from the paramater list.
(https://github.com/mkaiser/Sungrow-SHx-Inverter-Modbus-Home-Assistant)

I made 4x input numbers from UI, but if you wat to copy-paste them:

input_number:
  # Värmekurva 0-15
  input_number.varmekurva
    name: Värmekurva
    min: 0
    max: 15
    step: 1
    mode: box 
    icon: mdi:chart-line

  # Värmeförskjutning -10 till +10
  input_number.varmeforskjutning
    name: Värmeförskjutning
    min: -10
    max: 10
    step: 1
    mode: box
    icon: mdi:plus-minus
    unit_of_measurement: "°C"

  # Min framledning 5-35°C
  input_number.min_framledning
    name: Min Framledning
    min: 5
    max: 35
    step: 0.5
    mode: box
    icon: mdi:thermometer-low
    unit_of_measurement: "°C"

  # Max framledning 20-70°C
  input_number.max_framledning
    name: Max Framledning
    min: 20
    max: 70
    step: 0.5
    mode: box
    icon: mdi:thermometer-high
    unit_of_measurement: "°C"

Corresponting automations is attached as .txt files and can be directly copied into the UI yaml editor.
