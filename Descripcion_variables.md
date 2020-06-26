### Descripción de las variables de los sensores 

A continuación está la descripción las variables de los sensores:

- ts: tiempo de la transferencia tiempo de almacenamiento
- t: tiempo de toma de dato del sensor
- p00: puvliómetros 
- tm00: temperatura 
- hr00: húmedad relativa
- h00: altura de la sección 1
- h01: altura de la sección 2
- bs00: radiación solar
- dv00: dirección del viento 
- vv00: velocidad del viento
- gs00: húmedad del suelo en la sección 0
- gs01: húmedad del suelo en la sección 1 
- b: bateria 
- f: frecuencia

Las variables que se utilizaron en este proyecto son las alturas, con ellas se calcula el caudal y el volumen XXX
y  la 

### Calculos para la medición de caudal, volumen y húmedad del suelo

Para la medición de caudal se utiliza la siguiente ecuación:

Q = k * h_real ^ n

Donde k = 0.08693607, n = 1.9322. La altura real es calculada a partir de la resta de las alturas h00 y h01. 

Respecto a la húmedad del suelo se utiliza la siguiente ecuación dependiento de la húmedad del suelo registrada por el sensor.

-Si la húmedad del suelo es mayor o igual a 480 entonces 

 hm_suelo = 0.235 ( hr - 480)

-Si la húmedad del suelo es menor a 480  entonces

hm_suelo = 0.115 (hr - 245)


