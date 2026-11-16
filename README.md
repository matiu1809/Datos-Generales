# Datos-Generales
##Descripcion del Hardware##
. Placa: Bigtreetech octopus v1.1
. Drivers DRV-8825 (4drivers idénticos)
. modo step/dir
. fuente switching 24v 15A
. cinemática cartesiana tipo Bedslinger o arquitectura de puente fijo y mesa móvil (Fixed Gantry / Moving Table)
. volumen de impresión: 230mm eje x, 230mm eje y, 76mm eje y
. Nema 17 con núcleo de 18mm de alto en eje x, y; nema 17 con núcleo de 30mm de alto en eje z
. Transición por husillo rosca acme de 8mm, 4 hilos, diametric de 8mm; en todos los ejes
. Motor unico en Eje z
. Hot end tipo E3D V6 con barrel bimetálico titanio cobre, boquilla 0.4mm latón con recubrimiento de teflón, funda protectora de silicona de block calefactor, resistencia 24v 50w, termistor 100k
. Cama Caliente Mk2b 200x200mm Impresora 3d 12/24v, termistor Neptune 4 Max / 4 Pro, 100.000Ω, 0 °C - 320 °C, NTC (Negative Temperature Coefficient) thermistor encapsulado en vidrio y cobre, 3.950 K, diametro de cabeza 1,3 mm; Cama Base Magnética Flexible Ender 235x235mm - Xprinted, Superficie PEI texturada, Chapa flexible, Base magnética adhesiva.
. Sensor De Proximidad Inductivo SN04-P (NPN) Normal Abierto
   Especificaciones:
   - Voltaje de Operación: 10V a 30V DC
   - Consumo: 5mA Nominal / 12mA Max
   - Tipo: NPN / Normal Abierto
   - Rango de medición: 4mm
   - Salida: DC de tres cables (NPN)
   - Material: ABS
   - Detección de objetos Ferrosos y Metálicos en general
   - Calidad Premium
   - Dimensiones: 18x18x31mm
   - Frecuencia de detección de 500 Hz
   - Corriente de salida de hasta 300 mA
   - Peso de solo 152 g
   - Pin final de carrera DIAG7, PG15 GND 3.3v, sin divisor de voltaje
. El sensor comienza a sensar a 5.4mm de la cama (es decir, con la boquilla a 1.6mm de la cama)
. el home se toma en el 0 de todos los ejes (x hacia la izquierda, y hacia atras, z hacia abajo); Recorridos reales: eje x 229mm, eje y 220mm, eje z 76mm
. altura del sensor respecto a la boquilla 3.8mm hacia arriba
. Salida M503:
>>M503
echo :; Linear Units:
echo: G21 ; (mm)
echo :; Temperature Units:
echo: M149 C ; Units in Celsius
echo :; Filament settings (Disabled):
echo: M200 SO D1.75
echo :; Steps per unit:
echo: M92 X400.00 Y400.00 Z400.00 E226.00
echo :; Max feedrates (units/s):
echo: M203 X150.00 Y150.00 Z150.00 E45.00
echo :; Max Acceleration (units/s2):
echo:
M201 X400.00 Y400.00 Z400.00 E2000.00
echo :; Acceleration (units/s2) (P<print
-accel> R<retract-accel> T<travel-accel>):
echo: M204 P200.00 R1500.00 T200.00
echo :; Advanced (B<min_segment_time_us>S<min_feedrate> T<min_travel_feedrate>J<junc_dev>):
echo: M205 B20000.00 S0.00 T0.00 J0.01
echo :; Home offset:
echo: M206 X0.00 Y0.00 Z0.00
echo :; Auto Bed Leveling:
echo: M420 S1 Z10.00 ; Leveling ON
echo: G29 W IO JO ZO.92750
echo: G29 W I1 JO ZO.72750
echo: G29 W I2 JO ZO.70000
echo: G29 W I3 JO ZO.74750
echo: G29 W I4 JO ZO.85250
echo: G29 W I5 JO Z1.16250
echo: G29 W IO J1 ZO.56500
echo: G29 W I1 J1 Z0.54500
echo: G29 W I2 J1 ZO.57750
echo: G29 W I3 J1 ZO.64250
echo: G29 W I4 J1 ZO.67250
echo: G29 W I5 J1 ZO.70500
echo: G29 W IO J2 ZO.54000
echo: G29 W I1 J2 Z0.53500
echo: G29 W I2 J2 Z0.55500
echo: G29 W I3 J2 Z0.59750
echo: G29 W I4 J2 Z0.63500
echo: G29 W I5 J2 Z0.63250
echo: G29 W IO J3 Z0.55250
echo: G29 W I1 J3 Z0.54250
echo: G29 W I2 J3 Z0.56500
echo: G29 W I3 J3 Z0.58250
echo: G29 W I4 J3 Z0.60500
echo: G29 W I5 J3 Z0.59250
echo: G29 W IO J4 ZO.61250
echo: G29 W I1 J4 ZO.48250
echo: G29 W I2 J4 ZO.48750
echo: G29 W I3 J4 Z0.51500
echo: G29 W I4 J4 ZO.51000
echo: G29 W IS J4 ZO.49250
echo: G29 W IO J5 Z1.12250
echo: G29 W I1 J5 ZO.77750
echo: G29 W I2 J5 ZO.67000
echo: G29 W I3 J5 ZO.66000
echo: G29 W I4 J5 Z0.69750
echo: G29 W I5 J5 ZO.82250
echo:; Material heatup parameters:
echo: M145 SO H180.00 B70.00 F0
echo: M145 S1 H240.00 B110.00 F0
echo:; Hotend PID:
echo: M301 P22.20 I1.08 D114.00
echo :; Bed PID:
echo: M304 P67.33 I6.33 D477.59
echo :; Z-Probe Offset:
echo: M851 X35.00 Y0.00 Z-0.30 ; (mm)
ok
. Salida M115:
>>M115
FIRMWARE_NAME:Marlin bugfix-2.0.x (Sep
29 2026 19:33:11) SOURCE_CODE_URL:githu
b.com/MarlinFirmware/Marlin PROTOCOL_VE
RSION:1.0 MACHINE_TYPE:3D Printer EXTRU
DER_COUNT: 1 UUID: cede2a2f-41a2-4748-9b1
2-c55c62f367ff
Cap: SERIAL_XON_XOFF:0
Cap:BINARY_FILE_TRANSFER:0
Cap: EEPROM: 1
Cap:VOLUMETRIC: 1
Cap:AUTOREPORT_POS:0
Cap: AUTOREPORT_TEMP: 1
Cap: PROGRESS:0
Cap: PRINT_JOB: 1
Cap: AUTOLEVEL: 1
Cap: RUNOUT: 0
Cap: Z_PROBE: 1
Cap: LEVELING_DATA: 1
Cap:BUILD_PERCENT:0
Cap: SOFTWARE_POWER:0
Cap: TOGGLE_LIGHTS:0
Cap:CASE_LIGHT_BRIGHTNESS:0
Cap: EMERGENCY_PARSER : 1
Cap: HOST_ACTION_COMMANDS: 1
Cap: PROMPT_SUPPORT: 1
Cap: SDCARD: 1
Cap:MULTI_VOLUME:0
Cap: REPEAT: 0
Cap: SD_WRITE: 1
Cap: AUTOREPORT_SD_STATUS:0
Cap:LONG_FILENAME:0
Cap:LFN_WRITE:0
Cap: CUSTOM FIRMWARE UPLOAD:0
Cap: EXTENDED_M20:0
Cap: THERMAL_PROTECTION: 1
Cap:MOTION_MODES:0
Cap:ARCS: 1
Cap: BABYSTEPPING: 1
Cap: CHAMBER_TEMPERATURE:0
Cap:COOLER_TEMPERATURE:0
Cap:MEATPACK:0
Cap:CONFIG_EXPORT:0
ok
. Salida M48 (con cama fria): 
echo:busy: processing
echo:busy: processing
Finished!
Mean: 1.764250 Min: 1.763 Max: 1.767 Ra
nge: 0.005
Standard Deviation: 0.001601
//action: notification Deviation: 0.0016
01
X:80.00 Y:120.00 Z:6.90 E:0.00 Count X:
32000 Y:48000 Z:2830
########
Repeatability Test
Mean: 1.76425
Min: 1.76300
Max: 1.76700
Range: 0.00500
Standard Deviation: 0.00160

. Salida G29 (con cama fria):
>>M420 V1
Bilinear Leveling Grid:
    0      1      2      3      4      5
0 +1.973 +2.100 +2.135 +2.108 +2.145 +2.132
1 +1.932 +1.995 +2.063 +2.082 +2.088 +2.100
2 +1.932 +1.983 +2.037 +2.067 +2.050 +2.035
3 +1.975 +2.005 +2.045 +2.067 +2.035 +1.970
4 +2.078 +2.030 +2.035 +2.033 +1.985 +1.928
5 +2.080 +2.067 +2.043 +2.015 +1.975 +1.865

Subdivided with CATMULL ROM Leveling Gr id:
     0        1        2        3        4        5        6        7        8        9        10       11       12       13       14       15 
0  +1.97250 +2.01843 +2.06435 +2.10000 +2.12083 +2.13139 +2.13500 +2.12806 +2.11417 +2.10750 +2.11704 +2.13380 +2.14500 +2.14454 +2.13852 +2.13250
1  +1.95769 +1.99440 +2.03112 +2.06157 +2.08372 +2.09961 +2.10907 +2.10857 +2.10165 +2.09880 +2.10591 +2.11708 +2.12509 +2.12646 +2.12467 +2.12287
2  +1.94287 +1.97038 +1.99789 +2.02315 +2.04662 +2.06783 +2.08315 +2.08909 +2.08914 +2.09009 +2.09478 +2.10037 +2.10519 +2.10839 +2.11082 +2.11324
3  +1.93250 +1.95315 +1.97380 +1.99500 +2.01889 +2.04333 +2.06250 +2.07324 +2.07870 +2.08250 +2.08500 +2.08583 +2.08750 +2.09111 +2.09556 +2.10000
4  +1.92796 +1.94576 +1.96355 +1.98269 +2.00553 +2.02971 +2.04944 +2.06245 +2.07101 +2.07620 +2.07685 +2.07412 +2.07269 +2.07451 +2.07763 +2.08074
5  +1.92787 +1.94516 +1.96244 +1.98065 +2.00155 +2.02337 +2.04167 +2.05529 +2.06539 +2.07102 +2.07004 +2.06458 +2.06009 +2.05871 +2.05829 +2.05787
6  +1.93250 +1.94898 +1.96546 +1.98250 +2.00139 +2.02083 +2.03750 +2.05111 +2.06194 +2.06750 +2.06509 +2.05741 +2.05000 +2.04481 +2.03991 +2.03500
7  +1.94130 +1.95645 +1.97161 +1.98732 +2.00472 +2.02268 +2.03824 +2.05159 +2.06255 +2.06769 +2.06423 +2.05493 +2.04463 +2.03459 +2.02355 +2.01250
8  +1.95481 +1.96835 +1.98189 +1.99602 +2.01187 +2.02832 +2.04259 +2.05505 +2.06534 +2.06954 +2.06522 +2.05482 +2.04176 +2.02628 +2.00814 +1.99000
9  +1.97500 +1.98463 +1.99426 +2.00500 +2.01824 +2.03259 +2.04500 +2.05583 +2.06472 +2.06750 +2.06194 +2.05028 +2.03500 +2.01574 +1.99287 +1.97000
10 +2.00843 +2.00891 +2.00939 +2.01269 +2.02121 +2.03255 +2.04232 +2.05051 +2.05713 +2.05778 +2.04996 +2.03616 +2.01944 +1.99987 +1.97739 +1.95491
11 +2.04852 +2.03757 +2.02661 +2.02065 +2.02339 +2.03112 +2.03769 +2.04250 +2.04615 +2.04417 +2.03370 +2.01760 +2.00000 +1.98177 +1.96204 +1.94231
12 +2.07750 +2.05972 +2.04194 +2.03000 +2.02806 +2.03194 +2.03500 +2.03639 +2.03694 +2.03250 +2.02037 +2.00324 +1.98500 +1.96657 +1.94704 +1.92750
13 +2.08574 +2.06958 +2.05342 +2.04157 +2.03711 +2.03696 +2.03620 +2.03432 +2.03184 +2.02537 +2.01335 +1.99736 +1.97870 +1.95695 +1.93255 +1.90815
14 +2.08287 +2.07294 +2.06301 +2.05454 +2.04865 +2.04422 +2.03935 +2.03415 +2.02851 +2.02018 +2.00927 +1.99567 +1.97685 +1.95024 +1.91841 +1.88657
15 +2.08000 +2.07630 +2.07259 +2.06750 +2.06019 +2.05148 +2.04250 +2.03398 +2.02519 +2.01500 +2.00519 +1.99398 +1.97500 +1.94352 +1.90426 +1.86500

echo:Bed Leveling ON
echo:Fade Height 10.00

. Salida G29 (con cama caliente):



>>M420 V1
Bilinear Leveling Grid:
    0      1      2      3      4      5
0 +2.015 +2.125 +2.158 +2.142 +2.180 +2.178
1 +2.005 +2.053 +2.110 +2.128 +2.128 +2.135
2 +2.005 +2.037 +2.082 +2.120 +2.085 +2.060
3 +2.025 +2.043 +2.070 +2.102 +2.055 +1.993
4 +2.098 +2.055 +2.043 +2.027 +1.987 +1.932
5 +2.098 +2.075 +2.053 +2.005 +1.963 +1.865

Subdivided with CATMULL ROM Leveling Grid:
     0        1        2        3        4        5        6        7        8        9        10       11       12       13       14       15
0  +2.01500 +2.05454 +2.09407 +2.12500 +2.14333 +2.15306 +2.15750 +2.15407 +2.14537 +2.14250 +2.15259 +2.16852 +2.18000 +2.18213 +2.17981 +2.17750
1  +2.01130 +2.04211 +2.07291 +2.09870 +2.11783 +2.13193 +2.14093 +2.14203 +2.13804 +2.13722 +2.14424 +2.15443 +2.16213 +2.16460 +2.16457 +2.16454
2  +2.00759 +2.02967 +2.05176 +2.07241 +2.09232 +2.11080 +2.12435 +2.12999 +2.13071 +2.13194 +2.13589 +2.14035 +2.14426 +2.14707 +2.14932 +2.15157
3  +2.00500 +2.02046 +2.03593 +2.05250 +2.07241 +2.09343 +2.11000 +2.11944 +2.12444 +2.12750 +2.12852 +2.12759 +2.12750 +2.12944 +2.13222 +2.13500
4  +2.00352 +2.01587 +2.02822 +2.04250 +2.06110 +2.08163 +2.09880 +2.11115 +2.12013 +2.12481 +2.12298 +2.11685 +2.11213 +2.11119 +2.11166 +2.11213
5  +2.00315 +2.01450 +2.02585 +2.03889 +2.05540 +2.07359 +2.08981 +2.10434 +2.11689 +2.12296 +2.11844 +2.10744 +2.09787 +2.09284 +2.08925 +2.08565
6  +2.00500 +2.01537 +2.02574 +2.03750 +2.05185 +2.06759 +2.08250 +2.09824 +2.11315 +2.12000 +2.11333 +2.09861 +2.08500 +2.07593 +2.06796 +2.06000
7  +2.00824 +2.01755 +2.02686 +2.03741 +2.05008 +2.06399 +2.07778 +2.09394 +2.10998 +2.11704 +2.10906 +2.09211 +2.07546 +2.06233 +2.04950 +2.03667
8  +2.01370 +2.02197 +2.03023 +2.03954 +2.05046 +2.06242 +2.07472 +2.09035 +2.10632 +2.11296 +2.10424 +2.08619 +2.06731 +2.05015 +2.03216 +2.01417
9  +2.02500 +2.03046 +2.03593 +2.04250 +2.05074 +2.06009 +2.07000 +2.08343 +2.09741 +2.10250 +2.09315 +2.07491 +2.05500 +2.03528 +2.01389 +1.99250
10 +2.04796 +2.04663 +2.04530 +2.04583 +2.04932 +2.05469 +2.06056 +2.06906 +2.07807 +2.07981 +2.06986 +2.05263 +2.03370 +2.01435 +1.99329 +1.97222
11 +2.07676 +2.06687 +2.05698 +2.05000 +2.04781 +2.04852 +2.04944 +2.05136 +2.05348 +2.05074 +2.04030 +2.02499 +2.00824 +1.99071 +1.97175 +1.95278
12 +2.09750 +2.08222 +2.06694 +2.05500 +2.04870 +2.04574 +2.04250 +2.03861 +2.03444 +2.02750 +2.01657 +2.00287 +1.98750 +1.97028 +1.95139 +1.93250
13 +2.10287 +2.08807 +2.07328 +2.06111 +2.05367 +2.04885 +2.04306 +2.03522 +2.02640 +2.01611 +2.00466 +1.99175 +1.97602 +1.95608 +1.93332 +1.91056
14 +2.10019 +2.08904 +2.07789 +2.06806 +2.06105 +2.05535 +2.04778 +2.03678 +2.02389 +2.01056 +1.99858 +1.98615 +1.96926 +1.94508 +1.91643 +1.88778
15 +2.09750 +2.09000 +2.08250 +2.07500 +2.06843 +2.06185 +2.05250 +2.03833 +2.02139 +2.00500 +1.99250 +1.98056 +1.96250 +1.93407 +1.89954 +1.86500
echo:Bed Leveling ON
echo:Fade Height 10.00

. Slicer: Orca slicer, configuraciones:
 - PETG Pintalot:
{
	"default_filament_colour": [
		"#000000"
	],
	"enable_overhang_bridge_fan": [
		"0"
	],
	"fan_max_speed": [
		"0"
	],
	"fan_min_speed": [
		"0"
	],
	"filament_cost": [
		"22505.5"
	],
	"filament_density": [
		"1.27"
	],
	"filament_extruder_variant": [
		"Direct Drive Standard"
	],
	"filament_flow_ratio": [
		"0.95"
	],
	"filament_max_volumetric_speed": [
		"10"
	],
	"filament_settings_id": [
		"PETG Printalot"
	],
	"filament_type": [
		"PETG"
	],
	"filament_vendor": [
		"Pintalot"
	],
	"from": "User",
	"hot_plate_temp": [
		"70"
	],
	"hot_plate_temp_initial_layer": [
		"80"
	],
	"inherits": "Generic PLA @System",
	"name": "PETG Printalot",
	"nozzle_temperature_initial_layer": [
		"235"
	],
	"nozzle_temperature_range_low": [
		"215"
	],
	"reduce_fan_stop_start_freq": [
		"0"
	],
	"slow_down_for_layer_cooling": [
		"0"
	],
	"version": "2.4.0.3"
}

 - Impresora Octopus:
{
	"adaptive_bed_mesh_margin": "0",
	"auxiliary_fan": "0",
	"bbl_use_printhost": "0",
	"bed_custom_model": "",
	"bed_custom_texture": "",
	"bed_exclude_area": [
		"0x0"
	],
	"bed_exclude_volume_mode": "shared",
	"bed_exclude_volumes": "",
	"bed_mesh_max": "99999,99999",
	"bed_mesh_min": "-99999,-99999",
	"bed_mesh_probe_distance": "50,50",
	"bed_temperature_formula": "by_highest_temp",
	"before_layer_change_gcode": ";BEFORE_LAYER_CHANGE\n;[layer_z]\nG92 E0\n",
	"belt_frame_tilt_angle": "45",
	"belt_frame_tilt_decouple": "0",
	"belt_printer": "0",
	"belt_printer_infinite_y": "1",
	"belt_slice_rotation": "x",
	"belt_slice_rotation_angle": "45",
	"belt_support_floor_offset": "0",
	"best_object_pos": "0.5,0.5",
	"build_plate_tilt_x": "0",
	"build_plate_tilt_y": "0",
	"change_extrusion_role_gcode": "",
	"change_filament_gcode": "",
	"cooling_filter_enabled": "0",
	"cooling_tube_length": "5",
	"cooling_tube_retraction": "91.5",
	"default_bed_type": "",
	"default_filament_profile": [],
	"default_nozzle_volume_type": [
		"Standard"
	],
	"default_print_profile": "",
	"deretract_speed_extruder_change": [
		"0"
	],
	"deretraction_speed": [
		"30",
		"30",
		"30"
	],
	"disable_m73": "0",
	"emit_machine_limits_to_gcode": "0",
	"enable_belt_purge_tower": "0",
	"enable_filament_ramming": "1",
	"enable_long_retraction_when_cut": "0",
	"enable_power_loss_recovery": "printer_configuration",
	"enable_pre_heating": "0",
	"extra_loading_move": "-2",
	"extruder_bed_exclude_volumes": [
		""
	],
	"extruder_clearance_dist_to_rod": "40",
	"extruder_clearance_height_to_lid": "140",
	"extruder_clearance_height_to_rod": "36",
	"extruder_clearance_radius": "65",
	"extruder_colour": [
		"#FCE94F"
	],
	"extruder_max_nozzle_count": [
		"1"
	],
	"extruder_offset": [
		"0x0"
	],
	"extruder_printable_area": [],
	"extruder_printable_height": [
		"0"
	],
	"extruder_type": [
		"Direct Drive"
	],
	"extruder_variant_list": [
		"Direct Drive Standard,Direct Drive High Flow,Direct Drive Extra High Flow"
	],
	"fan_direction": "undefine",
	"fan_kickstart": "0",
	"fan_speedup_overhangs": "0",
	"fan_speedup_time": "0",
	"farthest_point_timelapse": "0",
	"file_start_gcode": "",
	"flashforge_serial_number": "",
	"from": "User",
	"gcode_flavor": "marlin",
	"gcode_remap_x": "pos_x",
	"gcode_remap_y": "pos_y",
	"gcode_remap_z": "pos_z",
	"gcode_skip_config_block": "0",
	"grab_length": [
		"0"
	],
	"group_algo_with_time": "0",
	"head_wrap_detect_zone": [],
	"high_current_on_filament_swap": "0",
	"host_type": "octoprint",
	"hotend_cooling_rate": [
		"2",
		"2",
		"2"
	],
	"hotend_heating_rate": [
		"2",
		"2",
		"2"
	],
	"imex_carriage_margin": "0",
	"imex_firmware_managed_zones": "0",
	"imex_gantry_count": "1",
	"imex_mode_active_tools": [],
	"imex_mode_gcodes": [],
	"imex_mode_names": [],
	"imex_nozzle_clearance_x": "30",
	"imex_nozzle_clearance_y": "30",
	"imex_tool_layout": "front-left",
	"imex_tools_per_gantry": "2",
	"imex_viz_theme": "standard",
	"inherits": "MyMarlin 0.4 nozzle",
	"input_shaping_damp_x": "0.1",
	"input_shaping_damp_y": "0.1",
	"input_shaping_emit": "0",
	"input_shaping_freq_x": "0",
	"input_shaping_freq_y": "0",
	"input_shaping_type": "Default",
	"is_imex": "0",
	"layer_change_gcode": ";AFTER_LAYER_CHANGE\n;[layer_z]",
	"long_retractions_when_cut": [
		"0",
		"0",
		"0"
	],
	"machine_bed_mass_Y": "0",
	"machine_end_gcode": "G1 E-1.0 F2100 ; retract\nG92 E0.0\nG1{if max_layer_z < max_print_height} Z{z_offset+min(max_layer_z+30, max_print_height)}{endif} E-34.0 F720 ; move print head up & retract filament\nG4 ; wait\nM104 S0 ; turn off temperature\nM140 S0 ; turn off heatbed\nM107 ; turn off fan\nG1 X0 Y105 F3000 ; park print head\nM84 ; disable motors",
	"machine_hotend_change_time": "0",
	"machine_load_filament_time": "0",
	"machine_max_acceleration_e": [
		"5000",
		"5000",
		"5000",
		"5000",
		"5000",
		"5000"
	],
	"machine_max_acceleration_extruding": [
		"10000",
		"10000",
		"10000",
		"10000",
		"10000",
		"10000"
	],
	"machine_max_acceleration_retracting": [
		"1000",
		"1000",
		"1000",
		"1000",
		"1000",
		"1000"
	],
	"machine_max_acceleration_travel": [
		"0",
		"0",
		"0",
		"0",
		"0",
		"0"
	],
	"machine_max_acceleration_x": [
		"10000",
		"10000",
		"10000",
		"10000",
		"10000",
		"10000"
	],
	"machine_max_acceleration_y": [
		"10000",
		"10000",
		"10000",
		"10000",
		"10000",
		"10000"
	],
	"machine_max_acceleration_z": [
		"500",
		"500",
		"500",
		"500",
		"500",
		"500"
	],
	"machine_max_force_Y": "0",
	"machine_max_jerk_e": [
		"5",
		"5",
		"5",
		"5",
		"5",
		"5"
	],
	"machine_max_jerk_x": [
		"8",
		"8",
		"8",
		"8",
		"8",
		"8"
	],
	"machine_max_jerk_y": [
		"8",
		"8",
		"8",
		"8",
		"8",
		"8"
	],
	"machine_max_jerk_z": [
		"0.4",
		"0.4",
		"0.4",
		"0.4",
		"0.4",
		"0.4"
	],
	"machine_max_junction_deviation": [
		"0.01",
		"0.01",
		"0.01",
		"0.01",
		"0.01",
		"0.01"
	],
	"machine_max_printed_mass": "0",
	"machine_max_speed_e": [
		"60",
		"60",
		"60",
		"60",
		"60",
		"60"
	],
	"machine_max_speed_x": [
		"500",
		"500",
		"500",
		"500",
		"500",
		"500"
	],
	"machine_max_speed_y": [
		"500",
		"500",
		"500",
		"500",
		"500",
		"500"
	],
	"machine_max_speed_z": [
		"10",
		"10",
		"10",
		"10",
		"10",
		"10"
	],
	"machine_min_extruding_rate": [
		"0"
	],
	"machine_min_travel_rate": [
		"0"
	],
	"machine_pause_gcode": "M601",
	"machine_prepare_compensation_time": "260",
	"machine_start_gcode": "G90 ; use absolute coordinates\nM83 ; extruder relative mode\nM204 S[machine_max_acceleration_extruding] T[machine_max_acceleration_retracting]\nM104 S[first_layer_temperature] ; set extruder temp\nM140 S[first_layer_bed_temperature] ; set bed temp\n\n; --- INICIO Y MAPA ---\nG28 ; Home de todos los ejes\nM420 S1 ; Activar malla de nivelacion\n\nM412 S0 ; Apagar el sensor de filamento (Comando corregido)\n\n; --- MANIOBRA EVASIVA Y CALENTAMIENTO SEGURO ---\nG0 Z15 F600 ; Levanta la boquilla a 15mm (Pasa por encima del tornillo)\nG0 X10 Y15 F3000 ; Se mueve a zona segura dentro del vidrio (X15 Y15)\nM190 S[first_layer_bed_temperature] ; Espera que la cama llegue a temp final\nM109 S[first_layer_temperature] ; Espera que la boquilla llegue a temp final\n\n; --- LINEA DE PURGA SEGURA ---\nG0 Z0.2 F600 ; Ahora si, baja a la altura de impresion\nG92 E0.0 ; Resetea el extrusor\nG1 X10 Y150.0 Z0.5 F1500.0 E15 ; Dibuja la primera linea hacia el fondo\nG1 X10.4 Y150.0 Z0.5 F5000.0 ; Se mueve un milimetro al lado\nG1 X10.4 Y20.0 Z0.5 F1500.0 E30 ; Dibuja la segunda linea volviendo\nG92 E0.0 ; Resetea la memoria del extrusor\nG1 Z2.0 F3000 ; Levanta la boquilla a 2mm para viajar al centro sin rayar",
	"machine_tool_change_time": "0",
	"machine_unload_filament_time": "0",
	"manual_filament_change": "0",
	"master_extruder_id": "1",
	"max_layer_height": [
		"0.32"
	],
	"max_resonance_avoidance_speed": "120",
	"min_layer_height": [
		"0.08"
	],
	"min_resonance_avoidance_speed": "70",
	"name": "Impresora Octopus",
	"nozzle_diameter": [
		"0.4"
	],
	"nozzle_flush_dataset": [
		"0",
		"0",
		"0"
	],
	"nozzle_height": "2.5",
	"nozzle_hrc": "0",
	"nozzle_type": [
		"brass",
		"brass",
		"brass"
	],
	"nozzle_volume": [
		"0",
		"0",
		"0"
	],
	"parallel_printheads_bed_exclude_areas": [],
	"parallel_printheads_count": "1",
	"parking_pos_retraction": "92",
	"part_cooling_fan_min_pwm": "0",
	"pellet_modded_printer": "0",
	"physical_extruder_map": [
		"0"
	],
	"preferred_orientation": "0",
	"printable_area": [
		"0x0",
		"200x0",
		"200x220",
		"0x220"
	],
	"printable_height": "70",
	"printer_agent": "",
	"printer_extruder_id": [
		"1",
		"1",
		"1"
	],
	"printer_extruder_variant": [
		"Direct Drive Standard",
		"Direct Drive High Flow",
		"Direct Drive Extra High Flow"
	],
	"printer_model": "Generic Marlin Printer",
	"printer_notes": "27-8 primera configuracion\n",
	"printer_plugin_config_overrides": "",
	"printer_settings_id": "Impresora Octopus",
	"printer_structure": "undefine",
	"printer_technology": "FFF",
	"printer_variant": "0.4",
	"printhost_authorization_type": "key",
	"printhost_ssl_ignore_revoke": "0",
	"printing_by_object_gcode": "",
	"purge_in_prime_tower": "1",
	"resonance_avoidance": "0",
	"retract_after_wipe": [
		"0%",
		"0%",
		"0%"
	],
	"retract_before_wipe": [
		"70%",
		"70%",
		"70%"
	],
	"retract_length_toolchange": [
		"1",
		"1",
		"1"
	],
	"retract_lift_above": [
		"0",
		"0",
		"0"
	],
	"retract_lift_below": [
		"0",
		"0",
		"0"
	],
	"retract_lift_enforce": [
		"All Surfaces",
		"All Surfaces",
		"All Surfaces"
	],
	"retract_restart_extra": [
		"0",
		"0",
		"0"
	],
	"retract_restart_extra_toolchange": [
		"0",
		"0",
		"0"
	],
	"retract_when_changing_layer": [
		"1",
		"1",
		"1"
	],
	"retraction_distances_when_cut": [
		"18",
		"18",
		"18"
	],
	"retraction_length": [
		"0.4",
		"0.4",
		"0.4"
	],
	"retraction_minimum_travel": [
		"0.4",
		"0.4",
		"0.4"
	],
	"retraction_speed": [
		"30",
		"30",
		"30"
	],
	"scan_first_layer": "0",
	"single_extruder_multi_material": "1",
	"support_air_filtration": "1",
	"support_chamber_temp_control": "0",
	"support_cooling_filter": "0",
	"support_fast_purge_mode": "0",
	"support_multi_bed_types": "0",
	"support_object_skip_flush": "0",
	"support_parallel_printheads": "0",
	"template_custom_gcode": "",
	"thumbnails": "48x48/PNG,300x300/PNG",
	"thumbnails_format": "PNG",
	"time_cost": "0",
	"time_lapse_gcode": "",
	"tool_change_on_wipe_tower": "0",
	"travel_slope": [
		"3",
		"3",
		"3"
	],
	"upward_compatible_machine": [],
	"use_3mf": "0",
	"use_firmware_retraction": "0",
	"use_relative_e_distances": "1",
	"version": "2.4.0.1",
	"wait_for_temp_on_wipe_tower": "0",
	"wipe": [
		"1",
		"1",
		"1"
	],
	"wipe_distance": [
		"1",
		"1",
		"1"
	],
	"wipe_tower_type": "type2",
	"wrapping_detection_gcode": "",
	"wrapping_detection_layers": "20",
	"wrapping_exclude_area": [],
	"z_hop": [
		"0",
		"0",
		"0"
	],
	"z_hop_types": [
		"Slope Lift",
		"Slope Lift",
		"Slope Lift"
	],
	"z_offset": "0"
}

 - 0.2mm PETG Printalot
 {
	"alternate_extra_wall": "1",
	"bottom_shell_layers": "3",
	"bottom_shell_thickness": "0.4",
	"bottom_solid_infill_flow_ratio": "0.95",
	"bridge_acceleration": "200",
	"brim_flow_ratio": "0.9",
	"brim_object_gap": "0.3",
	"brim_type": "outer_only",
	"brim_width": "4",
	"default_acceleration": "200",
	"elefant_foot_compensation": "0.1",
	"enable_support": "1",
	"ensure_vertical_shell_thickness": "ensure_moderate",
	"from": "User",
	"fuzzy_skin_first_layer": "1",
	"fuzzy_skin_mode": "combined",
	"fuzzy_skin_point_distance": "0.5",
	"fuzzy_skin_thickness": "0.15",
	"infill_combination": "1",
	"infill_combination_max_layer_height": "80%",
	"inherits": "0.08mm Extra Fine @MyMarlin",
	"initial_layer_acceleration": "200",
	"initial_layer_infill_speed": "65",
	"initial_layer_print_height": "0.1",
	"initial_layer_speed": "65",
	"initial_layer_travel_speed": "80",
	"inner_wall_acceleration": "200",
	"internal_bridge_flow": "0.95",
	"internal_bridge_speed": "50",
	"internal_solid_infill_acceleration": "200",
	"ironing_speed": "60",
	"is_infill_first": "1",
	"layer_height": "0.15",
	"max_travel_detour_distance": "1000",
	"name": "0.2mm PETG Printalot",
	"outer_wall_acceleration": "200",
	"outer_wall_speed": "80",
	"overhang_2_4_speed": "40",
	"print_extruder_id": [
		"1"
	],
	"print_extruder_variant": [
		"Direct Drive Standard"
	],
	"print_settings_id": "0.2mm PETG Printalot",
	"reduce_crossing_wall": "1",
	"reduce_infill_retraction": "0",
	"resolution": "0.01",
	"slice_closing_radius": "0.01",
	"sparse_infill_acceleration": "200",
	"sparse_infill_pattern": "gyroid",
	"support_bottom_interface_spacing": "0.2",
	"support_interface_pattern": "rectilinear_interlaced",
	"support_interface_spacing": "0.35",
	"support_interface_speed": "65",
	"support_interface_top_layers": "5",
	"support_ironing_flow": "5%",
	"support_object_first_layer_gap": "0.5",
	"support_object_xy_distance": "0.5",
	"support_speed": "80",
	"support_top_z_distance": "0.16",
	"support_type": "tree(auto)",
	"top_shell_layers": "3",
	"top_shell_thickness": "0.35",
	"top_solid_infill_flow_ratio": "0.95",
	"top_surface_acceleration": "200",
	"top_surface_pattern": "monotonic",
	"top_surface_speed": "80",
	"travel_acceleration": "350",
	"travel_speed": "80",
	"tree_support_branch_diameter_organic": "4",
	"tree_support_tip_diameter": "4",
	"tree_support_top_rate": "15%",
	"tree_support_wall_count": "1",
	"version": "2.4.0.1",
	"wall_transition_angle": "50",
	"xy_contour_compensation": "-0.1",
	"xy_hole_compensation": "0.25"
}

 
