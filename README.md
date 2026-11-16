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
    0        1        2        3        4        5        6        7
  8        9        10       11       12       13       14       15 
0 +1.97250 +2.01843 +2.06435 +2.10000 +2.12083 +2.13139 +2.13500 +2.12806 +2.11417 +2.10750 +2.11704 +2.13380 +2.14500 +2.14454 +2.13852 +2.13250

1 +1.95769 +1.99440 +2.03112 +2.06157 +2.08372 +2.09961 +2.10907 +2.10857 +2.10165 +2.09880 +2.10591 +2.11708 +2.12509 +2.12646 +2.12467 +2.12287

2 +1.94287 +1.97038 +1.99789 +2.02315 +2.04662 +2.06783 +2.08315 +2.08909 +2.08914 +2.09009 +2.09478 +2.10037 +2.105 19 +2.10839 +2.11082 +2.11324

3 +1.93250 +1.95315 +1.97380 +1.99500 +2.01889 +2.04333 +2.06250 +2.07324 +2.07870 +2.08250 +2.08500 +2.08583 +2.08750 +2.09111 +2.09556 +2.10000

4 +1.92796 +1.94576 +1.96355 +1.98269 +2.00553 +2.02971 +2.04944 +2.06245 +2.07101 +2.07620 +2.07685 +2.07412 +2.07269 +2.07451 +2.07763 +2.08074

5 +1.92787 +1.94516 +1.96244 +1.98065 +2.00155 +2.02337 +2.04167 +2.05529 +2.06539 +2.07102 +2.07004 +2.06458 +2.06009 +2.05871 +2.05829 +2.05787

6 +1.93250 +1.94898 +1.96546 +1.98250 +2.00139 +2.02083 +2.03750 +2.05111 +2.06194 +2.06750 +2.06509 +2.05741 +2.05000 +2.04481 +2.03991 +2.03500

7 +1.94130 +1.95645 +1.97161 +1.98732 +2.00472 +2.02268 +2.03824 +2.05159 +2.06255 +2.06769 +2.06423 +2.05493 +2.04463 +2.03459 +2.02355 +2.01250

8 +1.95481 +1.96835 +1.98189 +1.99602 +2.01187 +2.02832 +2.04259 +2.05505 +2.06534 +2.06954 +2.06522 +2.05482 +2.04176 +2.02628 +2.00814 +1.99000

9 +1.97500 +1.98463 +1.99426 +2.00500 +2.01824 +2.03259 +2.04500 +2.05583 +2.06472 +2.06750 +2.06194 +2.05028 +2.03500 +2.01574 +1.99287 +1.97000

10 +2.00843 +2.00891 +2.00939 +2.01269 +2.02121 +2.03255 +2.04232 +2.05051 +2.05713 +2.05778 +2.04996 +2.03616 +2.01944 +1.99987 +1.97739 +1.95491

11 +2.04852 +2.03757 +2.02661 +2.02065 +2.02339 +2.03112 +2.03769 +2.04250 +2.04615 +2.04417 +2.03370 +2.01760 +2.00000 +1.98177 +1.96204 +1.94231

12 +2.07750 +2.05972 +2.04194 +2.03000 +2.02806 +2.03194 +2.03500 +2.03639 +2.03694 +2.03250 +2.02037 +2.00324 +1.98500 +1.96657 +1.94704 +1.92750

13 +2.08574 +2.06958 +2.05342 +2.04157 +2.03711 +2.03696 +2.03620 +2.03432 +2.03184 +2.02537 +2.01335 +1.99736 +1.97870 +1.95695 +1.93255 +1.90815

14 +2.08287 +2.07294 +2.06301 +2.05454 +2.04865 +2.04422 +2.03935 +2.03415 +2.02851 +2.02018 +2.00927 +1.99567 +1.97685 +1.95024 +1.91841 +1.88657

15 +2.08000 +2.07630 +2.07259 +2.06750 +2.06019 +2.05148 +2.04250 +2.03398 +2.02519 +2.01500 +2.00519 +1.99398 +1.97500 +1.94352 +1.90426 +1.86500

echo:Bed Leveling ON
echo:Fade Height 10.00

. Salida G29 (con cama caliente):

. Slicer: Orca slicer, configuraciones:
 
