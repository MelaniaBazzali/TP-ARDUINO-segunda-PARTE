# TP7 – Periféricos Parte 2

## Introducción

En este proyecto se desarrolló un sistema de comunicación entre una placa **Arduino UNO** y el entorno de programación **Processing**, con el objetivo de controlar y visualizar el estado de las **entradas y salidas digitales** de la placa mediante una **interfaz gráfica**.

El trabajo se divide en dos partes:  
- Por un lado, **Arduino** gestiona las señales de **entrada** (dos pulsadores) y **salida** (dos LEDs), enviando y recibiendo información a través del puerto serie.  
- Por otro lado, **Processing** representa gráficamente estos estados, mostrando las entradas con distintos colores y permitiendo controlar las salidas desde la computadora, haciendo clic sobre los recuadros correspondientes.

La comunicación se realiza de manera **bidireccional** utilizando el **puerto serial USB** a **9600 bps**, permitiendo sincronizar los cambios de estado en tiempo real entre ambos programas.

## Funcionamiento general

- Los pulsadores conectados al Arduino modifican el estado de los LEDs en la interfaz de Processing.  
- Desde Processing, el usuario puede encender o apagar los LEDs haciendo clic con el mouse.  
- Arduino recibe esas órdenes y actualiza las salidas físicas, manteniendo la comunicación continua con la PC.

## Herramientas utilizadas

- **Arduino IDE**: para la programación y carga del código en la placa.  
- **Processing 4.x**: para el desarrollo de la interfaz gráfica y la comunicación serie.  
- **Placa Arduino UNO** y componentes electrónicos: 2 pulsadores, 2 LEDs y resistencias.  

## Limitaciones

- El programa trabaja con un número fijo de dos entradas y dos salidas.  
- Se requiere mantener abierta una única conexión serial (no usar el monitor del IDE simultáneamente).  

---
