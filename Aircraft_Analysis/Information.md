# Aircraft dataset


## The Dataset

In this directory, you'll find:
 A `flight_XXXXX.csv` file for each flight in the dataset.
 Each file contains the following signals from 5 seconds prior to launch, to 15 seconds after launch, logged at approximately 50Hz:

Name | Units | Description
--- |:---:| -----:
`seconds_since_launch` | seconds | time since launch
`position_ned_m[0]` | meters | position of the zip relative to a fixed reference point in the north direction
`position_ned_m[1]` | meters | position of the zip relative to a fixed reference point in the east direction
`position_ned_m[2]` | meters | position of the zip relative to a fixed reference point in the down direction
`velocity_ned_mps[0]` | meters/second | velocity of the zip, in the north direction
`velocity_ned_mps[1]` | meters/second | velocity of the zip, in the east direction
`velocity_ned_mps[2]` | meters/second | velocity of the zip, in the down direction
`accel_body_mps2[0]` | meters/second^2 | acceleration of the zip, in the body-forward direction
`accel_body_mps2[1]` | meters/second^2 | acceleration of the zip, in the body-right direction
`accel_body_mps2[2]` | meters/second^2 | acceleration of the zip, in the body-down direction
`orientation_rad[0]` | radians | Euler (Tait-Bryan) roll of the zip
`orientation_rad[1]` | radians | Euler (Tait-Bryan) pitch of the zip
`orientation_rad[2]` | radians | Euler (Tait-Bryan) yaw of the zip
`angular_rate_body_radps[0]` | radians/second | Angular velocity of the zip, about the body-forward direction
`angular_rate_body_radps[1]` | radians/second | Angular velocity of the zip, about the body-right direction
`angular_rate_body_radps[2]` | radians/second | Angular velocity of the zip, about the body-down direction
`position_sigma_ned_m[0]` | meters | estimated standard error of position_ned_m[0], i.e. positional uncertainty in the north direction
`position_sigma_ned_m[1]` | meters | estimated standard error of position_ned_m[1], i.e. positional uncertainty in the east direction
`position_sigma_ned_m[2]` | meters | estimated standard error of position_ned_m[2], i.e. positional uncertainty in the down direction

- A `summary_data.csv` file containing the following data for each flight in the dataset:

Name | Units | Description
--- |:---:| -----:
`flight_id` | n/a | unique identifier for the flight
`battery_serial_number` | n/a | serial number of the battery
`body_serial_number` | n/a | serial number of the body
`wing_serial_number` | n/a | serial number of the wing
`commit` | n/a | git commit SHA representing the version of software
`launch_airspeed` | meters/second | airspeed of the plane during launch
`launch_groundspeed` | meters/second | groundspeed of the plane during launch
`launch_timestamp` | n/a | time string `YYYT-MM-DD HH:MM:SS CAT` where CAT, i.e. Central Africa Time, is the timezone
`preflight_voltage` | volts | dc voltage of the battery immediately prior to launch
`air_temperature` | celsius | air temperature during launch
`rel_humidity` | percentage | relative humidity during launch
`static_pressure` | pascals | static air pressure during launch
`wind_direction` | degrees | direction of the wind during launch, with 0 blowing to the north, 90 blowing to the east
`wind_magnitude` | meters/second | magnitude of the wind during launch

