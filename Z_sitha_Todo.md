### Todo

fast_waypoint at do_nav_wp

#### Pump and centrifugal setup
Servo9 = 22
servo10 = 23

#### liquid sensor Pin setup
servo11/13 = -1 //change from output servo to input pin
btn_enable = 1 // reboot the fc
btn_pin1 = pin# // Goi aux3=60 fmuv3=54
btn_option1 = 1 // pull the logic pin high
wpnav_sensor_pin = gpio pin

#### Loiter z control
`update_z_controller()`
    `update_surface_offset`
         const float curr_surface_alt_above_origin_cm = copter.inertial_nav.get_position_z_up_cm() - dir * rf_state.alt_cm;
         

    `set_pos_target_z_from_climb_rate_cm`

                   