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
                        32.4mm
               |----------|
               |       |__+__| __
   Z=0    |____+____|          |  4.3mm 
 _____________\/_______________|___________cama
X=0          Nozle
Y=0

>>> G28
SENDING:G28
>>> M420 S0
SENDING:M420 S0
echo:Bed Leveling OFF
echo:Fade Height 10.00
>>> G30 x110 y110
SENDING:G30 X110 Y110
Bed X: 110.00 Y: 110.00 Z: 0.59

2-
>>> G29 V4
SENDING:G29 V4
G29 Auto Bed Leveling
Probing mesh point 1/36.
//action:notification Probing Point 1/36
Bed X: 180.00 Y: 20.00 Z: 0.62
Probing mesh point 2/36.
//action:notification Probing Point 2/36
Bed X: 148.20 Y: 20.00 Z: 0.59
Probing mesh point 3/36.
//action:notification Probing Point 3/36
Bed X: 116.40 Y: 20.00 Z: 0.56
Probing mesh point 4/36.
//action:notification Probing Point 4/36
Bed X: 84.60 Y: 20.00 Z: 0.54
Probing mesh point 5/36.
//action:notification Probing Point 5/36
Bed X: 52.80 Y: 20.00 Z: 0.46
Probing mesh point 6/36.
//action:notification Probing Point 6/36
Bed X: 21.00 Y: 20.00 Z: 0.37
Probing mesh point 7/36.
//action:notification Probing Point 7/36
Bed X: 21.00 Y: 56.00 Z: 0.30
Probing mesh point 8/36.
//action:notification Probing Point 8/36
Bed X: 52.80 Y: 56.00 Z: 0.38
Probing mesh point 9/36.
//action:notification Probing Point 9/36
Bed X: 84.60 Y: 56.00 Z: 0.48
Probing mesh point 10/36.
//action:notification Probing Point 10/36
Bed X: 116.40 Y: 56.00 Z: 0.53
Probing mesh point 11/36.
//action:notification Probing Point 11/36
Bed X: 148.20 Y: 56.00 Z: 0.54
Probing mesh point 12/36.
//action:notification Probing Point 12/36
Bed X: 180.00 Y: 56.00 Z: 0.59
Probing mesh point 13/36.
//action:notification Probing Point 13/36
Bed X: 180.00 Y: 92.00 Z: 0.56
Probing mesh point 14/36.
//action:notification Probing Point 14/36
Bed X: 148.20 Y: 92.00 Z: 0.55
Probing mesh point 15/36.
//action:notification Probing Point 15/36
Bed X: 116.40 Y: 92.00 Z: 0.56
Probing mesh point 16/36.
//action:notification Probing Point 16/36
Bed X: 84.60 Y: 92.00 Z: 0.53
Probing mesh point 17/36.
//action:notification Probing Point 17/36
Bed X: 52.80 Y: 92.00 Z: 0.46
Probing mesh point 18/36.
//action:notification Probing Point 18/36
Bed X: 21.00 Y: 92.00 Z: 0.38
Probing mesh point 19/36.
//action:notification Probing Point 19/36
Bed X: 21.00 Y: 128.00 Z: 0.46
Probing mesh point 20/36.
//action:notification Probing Point 20/36
Bed X: 52.80 Y: 128.00 Z: 0.50
Probing mesh point 21/36.
//action:notification Probing Point 21/36
Bed X: 84.60 Y: 128.00 Z: 0.54
Probing mesh point 22/36.
//action:notification Probing Point 22/36
Bed X: 116.40 Y: 128.00 Z: 0.57
Probing mesh point 23/36.
//action:notification Probing Point 23/36
Bed X: 148.20 Y: 128.00 Z: 0.55
Probing mesh point 24/36.
//action:notification Probing Point 24/36
Bed X: 180.00 Y: 128.00 Z: 0.49
Probing mesh point 25/36.
//action:notification Probing Point 25/36
Bed X: 180.00 Y: 164.00 Z: 0.46
Probing mesh point 26/36.
//action:notification Probing Point 26/36
Bed X: 148.20 Y: 164.00 Z: 0.52
Probing mesh point 27/36.
//action:notification Probing Point 27/36
Bed X: 116.40 Y: 164.00 Z: 0.57
Probing mesh point 28/36.
//action:notification Probing Point 28/36
Bed X: 84.60 Y: 164.00 Z: 0.57
Probing mesh point 29/36.
//action:notification Probing Point 29/36
Bed X: 52.80 Y: 164.00 Z: 0.55
Probing mesh point 30/36.
//action:notification Probing Point 30/36
Bed X: 21.00 Y: 164.00 Z: 0.58
Probing mesh point 31/36.
//action:notification Probing Point 31/36
Bed X: 21.00 Y: 200.00 Z: 0.61
Probing mesh point 32/36.
//action:notification Probing Point 32/36
Bed X: 52.80 Y: 200.00 Z: 0.60
Probing mesh point 33/36.
//action:notification Probing Point 33/36
Bed X: 84.60 Y: 200.00 Z: 0.61
Probing mesh point 34/36.
//action:notification Probing Point 34/36
Bed X: 116.40 Y: 200.00 Z: 0.56
Probing mesh point 35/36.
//action:notification Probing Point 35/36
Bed X: 148.20 Y: 200.00 Z: 0.53
Probing mesh point 36/36.
//action:notification Probing Point 36/36
Bed X: 180.00 Y: 200.00 Z: 0.45
//action:notification 3D Printer Ready.
Bilinear Leveling Grid:
      0      1      2      3      4      5
 0 +0.375 +0.460 +0.537 +0.560 +0.592 +0.620
 1 +0.302 +0.380 +0.477 +0.527 +0.542 +0.592
 2 +0.380 +0.462 +0.530 +0.565 +0.552 +0.557
 3 +0.462 +0.500 +0.545 +0.575 +0.547 +0.495
 4 +0.582 +0.552 +0.570 +0.570 +0.517 +0.465
 5 +0.615 +0.605 +0.612 +0.565 +0.532 +0.455
Subdivided with CATMULL ROM Leveling Grid:
        0        1        2        3        4        5        6        7        8        9       10       11       12       13       14       15
 0 +0.37500 +0.40361 +0.43222 +0.46000 +0.48843 +0.51602 +0.53750 +0.54870 +0.55380 +0.56000 +0.57028 +0.58167 +0.59250 +0.60204 +0.61102 +0.62000
 1 +0.34528 +0.37248 +0.39967 +0.42731 +0.45765 +0.48842 +0.51333 +0.52855 +0.53791 +0.54657 +0.55566 +0.56405 +0.57361 +0.58534 +0.59822 +0.61111
 2 +0.31556 +0.34134 +0.36713 +0.39463 +0.42687 +0.46083 +0.48917 +0.50840 +0.52202 +0.53315 +0.54104 +0.54644 +0.55472 +0.56864 +0.58543 +0.60222
 3 +0.30250 +0.32759 +0.35269 +0.38000 +0.41278 +0.44778 +0.47750 +0.49898 +0.51519 +0.52750 +0.53380 +0.53620 +0.54250 +0.55657 +0.57454 +0.59250
 4 +0.31704 +0.34333 +0.36963 +0.39713 +0.42823 +0.46054 +0.48806 +0.50872 +0.52459 +0.53583 +0.53968 +0.53891 +0.54194 +0.55289 +0.56765 +0.58241
 5 +0.34824 +0.37646 +0.40468 +0.43231 +0.46038 +0.48785 +0.51111 +0.52919 +0.54305 +0.55194 +0.55295 +0.54898 +0.54806 +0.55384 +0.56266 +0.57148
 6 +0.38000 +0.40806 +0.43611 +0.46250 +0.48731 +0.51046 +0.53000 +0.54583 +0.55806 +0.56500 +0.56370 +0.55713 +0.55250 +0.55287 +0.55519 +0.55750
 7 +0.40574 +0.43021 +0.45468 +0.47778 +0.49954 +0.51992 +0.53741 +0.55242 +0.56454 +0.57093 +0.56863 +0.56060 +0.55287 +0.54755 +0.54252 +0.53750
 8 +0.43204 +0.45084 +0.46964 +0.48806 +0.50656 +0.52468 +0.54065 +0.55519 +0.56757 +0.57380 +0.57104 +0.56214 +0.55157 +0.54030 +0.52737 +0.51444
 9 +0.46250 +0.47472 +0.48694 +0.50000 +0.51500 +0.53083 +0.54500 +0.55824 +0.56981 +0.57500 +0.57102 +0.56065 +0.54750 +0.53185 +0.51343 +0.49500
10 +0.50296 +0.50662 +0.51027 +0.51639 +0.52709 +0.54024 +0.55194 +0.56261 +0.57182 +0.57444 +0.56729 +0.55355 +0.53769 +0.52049 +0.50117 +0.48185
11 +0.54759 +0.54178 +0.53596 +0.53444 +0.54059 +0.55104 +0.56000 +0.56726 +0.57304 +0.57222 +0.56112 +0.54342 +0.52509 +0.50792 +0.49012 +0.47231
12 +0.58250 +0.57074 +0.55898 +0.55250 +0.55546 +0.56370 +0.57000 +0.57324 +0.57454 +0.57000 +0.55639 +0.53694 +0.51750 +0.50000 +0.48250 +0.46500
13 +0.59981 +0.58830 +0.57678 +0.57000 +0.57214 +0.57903 +0.58287 +0.58134 +0.57676 +0.56833 +0.55487 +0.53757 +0.51917 +0.50023 +0.48021 +0.46019
14 +0.60741 +0.59966 +0.59191 +0.58750 +0.59019 +0.59623 +0.59769 +0.59076 +0.57926 +0.56667 +0.55480 +0.54184 +0.52583 +0.50512 +0.48135 +0.45759
15 +0.61500 +0.61102 +0.60704 +0.60500 +0.60824 +0.61343 +0.61250 +0.60019 +0.58176 +0.56500 +0.55472 +0.54611 +0.53250 +0.51000 +0.48250 +0.45500
echo:Unknown command: "M10M105"
echo:Unknown command: "nU5U5M105"
>>> M420 V1
SENDING:M420 V1
Bilinear Leveling Grid:
      0      1      2      3      4      5
 0 +0.375 +0.460 +0.537 +0.560 +0.592 +0.620
 1 +0.302 +0.380 +0.477 +0.527 +0.542 +0.592
 2 +0.380 +0.462 +0.530 +0.565 +0.552 +0.557
 3 +0.462 +0.500 +0.545 +0.575 +0.547 +0.495
 4 +0.582 +0.552 +0.570 +0.570 +0.517 +0.465
 5 +0.615 +0.605 +0.612 +0.565 +0.532 +0.455
Subdivided with CATMULL ROM Leveling Grid:
        0        1        2        3        4        5        6        7        8        9       10       11       12       13       14       15
 0 +0.37500 +0.40361 +0.43222 +0.46000 +0.48843 +0.51602 +0.53750 +0.54870 +0.55380 +0.56000 +0.57028 +0.58167 +0.59250 +0.60204 +0.61102 +0.62000
 1 +0.34528 +0.37248 +0.39967 +0.42731 +0.45765 +0.48842 +0.51333 +0.52855 +0.53791 +0.54657 +0.55566 +0.56405 +0.57361 +0.58534 +0.59822 +0.61111
 2 +0.31556 +0.34134 +0.36713 +0.39463 +0.42687 +0.46083 +0.48917 +0.50840 +0.52202 +0.53315 +0.54104 +0.54644 +0.55472 +0.56864 +0.58543 +0.60222
 3 +0.30250 +0.32759 +0.35269 +0.38000 +0.41278 +0.44778 +0.47750 +0.49898 +0.51519 +0.52750 +0.53380 +0.53620 +0.54250 +0.55657 +0.57454 +0.59250
 4 +0.31704 +0.34333 +0.36963 +0.39713 +0.42823 +0.46054 +0.48806 +0.50872 +0.52459 +0.53583 +0.53968 +0.53891 +0.54194 +0.55289 +0.56765 +0.58241
 5 +0.34824 +0.37646 +0.40468 +0.43231 +0.46038 +0.48785 +0.51111 +0.52919 +0.54305 +0.55194 +0.55295 +0.54898 +0.54806 +0.55384 +0.56266 +0.57148
 6 +0.38000 +0.40806 +0.43611 +0.46250 +0.48731 +0.51046 +0.53000 +0.54583 +0.55806 +0.56500 +0.56370 +0.55713 +0.55250 +0.55287 +0.55519 +0.55750
 7 +0.40574 +0.43021 +0.45468 +0.47778 +0.49954 +0.51992 +0.53741 +0.55242 +0.56454 +0.57093 +0.56863 +0.56060 +0.55287 +0.54755 +0.54252 +0.53750
 8 +0.43204 +0.45084 +0.46964 +0.48806 +0.50656 +0.52468 +0.54065 +0.55519 +0.56757 +0.57380 +0.57104 +0.56214 +0.55157 +0.54030 +0.52737 +0.51444
 9 +0.46250 +0.47472 +0.48694 +0.50000 +0.51500 +0.53083 +0.54500 +0.55824 +0.56981 +0.57500 +0.57102 +0.56065 +0.54750 +0.53185 +0.51343 +0.49500
10 +0.50296 +0.50662 +0.51027 +0.51639 +0.52709 +0.54024 +0.55194 +0.56261 +0.57182 +0.57444 +0.56729 +0.55355 +0.53769 +0.52049 +0.50117 +0.48185
11 +0.54759 +0.54178 +0.53596 +0.53444 +0.54059 +0.55104 +0.56000 +0.56726 +0.57304 +0.57222 +0.56112 +0.54342 +0.52509 +0.50792 +0.49012 +0.47231
12 +0.58250 +0.57074 +0.55898 +0.55250 +0.55546 +0.56370 +0.57000 +0.57324 +0.57454 +0.57000 +0.55639 +0.53694 +0.51750 +0.50000 +0.48250 +0.46500
13 +0.59981 +0.58830 +0.57678 +0.57000 +0.57214 +0.57903 +0.58287 +0.58134 +0.57676 +0.56833 +0.55487 +0.53757 +0.51917 +0.50023 +0.48021 +0.46019
14 +0.60741 +0.59966 +0.59191 +0.58750 +0.59019 +0.59623 +0.59769 +0.59076 +0.57926 +0.56667 +0.55480 +0.54184 +0.52583 +0.50512 +0.48135 +0.45759
15 +0.61500 +0.61102 +0.60704 +0.60500 +0.60824 +0.61343 +0.61250 +0.60019 +0.58176 +0.56500 +0.55472 +0.54611 +0.53250 +0.51000 +0.48250 +0.45500
echo:Bed Leveling ON
echo:Fade Height 10.00

3-
>>> G29
SENDING:G29
//action:notification Probing Point 1/36
//action:notification Probing Point 2/36
//action:notification Probing Point 3/36
//action:notification Probing Point 4/36
//action:notification Probing Point 5/36
//action:notification Probing Point 6/36
//action:notification Probing Point 7/36
//action:notification Probing Point 8/36
//action:notification Probing Point 9/36
//action:notification Probing Point 10/36
//action:notification Probing Point 11/36
//action:notification Probing Point 12/36
//action:notification Probing Point 13/36
//action:notification Probing Point 14/36
//action:notification Probing Point 15/36
//action:notification Probing Point 16/36
//action:notification Probing Point 17/36
//action:notification Probing Point 18/36
//action:notification Probing Point 19/36
//action:notification Probing Point 20/36
//action:notification Probing Point 21/36
//action:notification Probing Point 22/36
//action:notification Probing Point 23/36
//action:notification Probing Point 24/36
//action:notification Probing Point 25/36
//action:notification Probing Point 26/36
//action:notification Probing Point 27/36
//action:notification Probing Point 28/36
//action:notification Probing Point 29/36
//action:notification Probing Point 30/36
//action:notification Probing Point 31/36
//action:notification Probing Point 32/36
//action:notification Probing Point 33/36
//action:notification Probing Point 34/36
//action:notification Probing Point 35/36
//action:notification Probing Point 36/36
//action:notification 3D Printer Ready.
Bilinear Leveling Grid:
      0      1      2      3      4      5
 0 +0.387 +0.477 +0.570 +0.592 +0.627 +0.662
 1 +0.340 +0.420 +0.527 +0.565 +0.592 +0.622
 2 +0.362 +0.457 +0.540 +0.582 +0.565 +0.570
 3 +0.482 +0.520 +0.580 +0.610 +0.582 +0.512
 4 +0.580 +0.550 +0.572 +0.567 +0.540 +0.477
 5 +0.662 +0.640 +0.642 +0.605 +0.560 +0.472
Subdivided with CATMULL ROM Leveling Grid:
        0        1        2        3        4        5        6        7        8        9       10       11       12       13       14       15
 0 +0.38750 +0.41741 +0.44731 +0.47750 +0.51074 +0.54426 +0.57000 +0.58222 +0.58667 +0.59250 +0.60324 +0.61537 +0.62750 +0.63917 +0.65083 +0.66250
 1 +0.36907 +0.39716 +0.42525 +0.45481 +0.48946 +0.52558 +0.55380 +0.56813 +0.57456 +0.58167 +0.59251 +0.60402 +0.61556 +0.62690 +0.63826 +0.64963
 2 +0.35065 +0.37692 +0.40319 +0.43213 +0.46818 +0.50690 +0.53759 +0.55404 +0.56246 +0.57083 +0.58178 +0.59267 +0.60361 +0.61463 +0.62570 +0.63676
 3 +0.34000 +0.36565 +0.39130 +0.42000 +0.45639 +0.49583 +0.52750 +0.54556 +0.55583 +0.56500 +0.57481 +0.58352 +0.59250 +0.60231 +0.61241 +0.62250
 4 +0.33870 +0.36671 +0.39473 +0.42454 +0.45963 +0.49652 +0.52657 +0.54563 +0.55786 +0.56713 +0.57335 +0.57662 +0.58111 +0.58863 +0.59737 +0.60611
 5 +0.34519 +0.37675 +0.40832 +0.43963 +0.47235 +0.50481 +0.53176 +0.55131 +0.56535 +0.57426 +0.57565 +0.57191 +0.57056 +0.57489 +0.58161 +0.58833
 6 +0.36250 +0.39463 +0.42676 +0.45750 +0.48741 +0.51593 +0.54000 +0.55935 +0.57426 +0.58250 +0.58028 +0.57139 +0.56500 +0.56500 +0.56750 +0.57000
 7 +0.39611 +0.42353 +0.45095 +0.47769 +0.50456 +0.53075 +0.55306 +0.57151 +0.58608 +0.59352 +0.59018 +0.57971 +0.56972 +0.56294 +0.55666 +0.55037
 8 +0.44056 +0.46027 +0.47999 +0.50065 +0.52405 +0.54839 +0.56917 +0.58602 +0.59932 +0.60565 +0.60241 +0.59221 +0.57944 +0.56473 +0.54746 +0.53019
 9 +0.48250 +0.49417 +0.50583 +0.52000 +0.53944 +0.56139 +0.58000 +0.59435 +0.60537 +0.61000 +0.60667 +0.59694 +0.58250 +0.56231 +0.53741 +0.51250
10 +0.51722 +0.52025 +0.52327 +0.53019 +0.54462 +0.56294 +0.57815 +0.58862 +0.59598 +0.59806 +0.59404 +0.58474 +0.57046 +0.54965 +0.52385 +0.49806
11 +0.54944 +0.54348 +0.53751 +0.53676 +0.54570 +0.55986 +0.57102 +0.57671 +0.57940 +0.57833 +0.57343 +0.56477 +0.55176 +0.53277 +0.50944 +0.48611
12 +0.58000 +0.56806 +0.55611 +0.55000 +0.55463 +0.56509 +0.57250 +0.57370 +0.57185 +0.56750 +0.56130 +0.55259 +0.54000 +0.52176 +0.49963 +0.47750
13 +0.60861 +0.59583 +0.58305 +0.57556 +0.57801 +0.58575 +0.59009 +0.58761 +0.58173 +0.57407 +0.56593 +0.55600 +0.54204 +0.52192 +0.49777 +0.47361
14 +0.63556 +0.62495 +0.61435 +0.60778 +0.60924 +0.61473 +0.61630 +0.61043 +0.60063 +0.58954 +0.57903 +0.56722 +0.55102 +0.52795 +0.50050 +0.47306
15 +0.66250 +0.65407 +0.64565 +0.64000 +0.64046 +0.64370 +0.64250 +0.63324 +0.61954 +0.60500 +0.59213 +0.57843 +0.56000 +0.53398 +0.50324 +0.47250
>>> M420 V1
SENDING:M420 V1
Bilinear Leveling Grid:
      0      1      2      3      4      5
 0 +0.387 +0.477 +0.570 +0.592 +0.627 +0.662
 1 +0.340 +0.420 +0.527 +0.565 +0.592 +0.622
 2 +0.362 +0.457 +0.540 +0.582 +0.565 +0.570
 3 +0.482 +0.520 +0.580 +0.610 +0.582 +0.512
 4 +0.580 +0.550 +0.572 +0.567 +0.540 +0.477
 5 +0.662 +0.640 +0.642 +0.605 +0.560 +0.472
Subdivided with CATMULL ROM Leveling Grid:
        0        1        2        3        4        5        6        7        8        9       10       11       12       13       14       15
 0 +0.38750 +0.41741 +0.44731 +0.47750 +0.51074 +0.54426 +0.57000 +0.58222 +0.58667 +0.59250 +0.60324 +0.61537 +0.62750 +0.63917 +0.65083 +0.66250
 1 +0.36907 +0.39716 +0.42525 +0.45481 +0.48946 +0.52558 +0.55380 +0.56813 +0.57456 +0.58167 +0.59251 +0.60402 +0.61556 +0.62690 +0.63826 +0.64963
 2 +0.35065 +0.37692 +0.40319 +0.43213 +0.46818 +0.50690 +0.53759 +0.55404 +0.56246 +0.57083 +0.58178 +0.59267 +0.60361 +0.61463 +0.62570 +0.63676
 3 +0.34000 +0.36565 +0.39130 +0.42000 +0.45639 +0.49583 +0.52750 +0.54556 +0.55583 +0.56500 +0.57481 +0.58352 +0.59250 +0.60231 +0.61241 +0.62250
 4 +0.33870 +0.36671 +0.39473 +0.42454 +0.45963 +0.49652 +0.52657 +0.54563 +0.55786 +0.56713 +0.57335 +0.57662 +0.58111 +0.58863 +0.59737 +0.60611
 5 +0.34519 +0.37675 +0.40832 +0.43963 +0.47235 +0.50481 +0.53176 +0.55131 +0.56535 +0.57426 +0.57565 +0.57191 +0.57056 +0.57489 +0.58161 +0.58833
 6 +0.36250 +0.39463 +0.42676 +0.45750 +0.48741 +0.51593 +0.54000 +0.55935 +0.57426 +0.58250 +0.58028 +0.57139 +0.56500 +0.56500 +0.56750 +0.57000
 7 +0.39611 +0.42353 +0.45095 +0.47769 +0.50456 +0.53075 +0.55306 +0.57151 +0.58608 +0.59352 +0.59018 +0.57971 +0.56972 +0.56294 +0.55666 +0.55037
 8 +0.44056 +0.46027 +0.47999 +0.50065 +0.52405 +0.54839 +0.56917 +0.58602 +0.59932 +0.60565 +0.60241 +0.59221 +0.57944 +0.56473 +0.54746 +0.53019
 9 +0.48250 +0.49417 +0.50583 +0.52000 +0.53944 +0.56139 +0.58000 +0.59435 +0.60537 +0.61000 +0.60667 +0.59694 +0.58250 +0.56231 +0.53741 +0.51250
10 +0.51722 +0.52025 +0.52327 +0.53019 +0.54462 +0.56294 +0.57815 +0.58862 +0.59598 +0.59806 +0.59404 +0.58474 +0.57046 +0.54965 +0.52385 +0.49806
11 +0.54944 +0.54348 +0.53751 +0.53676 +0.54570 +0.55986 +0.57102 +0.57671 +0.57940 +0.57833 +0.57343 +0.56477 +0.55176 +0.53277 +0.50944 +0.48611
12 +0.58000 +0.56806 +0.55611 +0.55000 +0.55463 +0.56509 +0.57250 +0.57370 +0.57185 +0.56750 +0.56130 +0.55259 +0.54000 +0.52176 +0.49963 +0.47750
13 +0.60861 +0.59583 +0.58305 +0.57556 +0.57801 +0.58575 +0.59009 +0.58761 +0.58173 +0.57407 +0.56593 +0.55600 +0.54204 +0.52192 +0.49777 +0.47361
14 +0.63556 +0.62495 +0.61435 +0.60778 +0.60924 +0.61473 +0.61630 +0.61043 +0.60063 +0.58954 +0.57903 +0.56722 +0.55102 +0.52795 +0.50050 +0.47306
15 +0.66250 +0.65407 +0.64565 +0.64000 +0.64046 +0.64370 +0.64250 +0.63324 +0.61954 +0.60500 +0.59213 +0.57843 +0.56000 +0.53398 +0.50324 +0.47250
echo:Bed Leveling ON
echo:Fade Height 10.00

4-
>>> G30 X100 Y110
SENDING:G30 X100 Y110
Bed X: 100.00 Y: 110.00 Z: 0.57

5-
>>> g28
SENDING:G28
>>> M420 S0
SENDING:M420 S0
echo:Bed Leveling OFF
echo:Fade Height 10.00
>>> G30 X100 Y110
SENDING:G30 X100 Y110
Bed X: 100.00 Y: 110.00 Z: 0.56


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

 
