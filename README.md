# Voltage
This is C code that simulates a battery meter display. The program takes two arguments from the command line: the battery voltage value (in units of 0.001 volts) and a display mode flag ('V' for voltage or 'P' for percent).

The program sets the BATT_VOLTAGE_PORT and BATT_STATUS_PORT values based on the command line arguments, then uses the set_batt_from_ports function to set the values of a batt_t struct representing the battery status. The set_display_from_batt function then takes this struct as input and sets the BATT_DISPLAY_PORT value based on the desired display mode.

The program then calls the batt_update function, which updates the battery meter display by setting individual LED segments based on the BATT_DISPLAY_PORT value.

The output of the program includes the values of the BATT_VOLTAGE_PORT, BATT_STATUS_PORT, and BATT_DISPLAY_PORT registers, as well as the values of the batt_t struct and the display mode. The final output is a graphical representation of the battery meter display.
