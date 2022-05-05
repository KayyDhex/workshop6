# Workshop6
sixth workshop of automation and control of process class

- [Workshop6](#workshop6)
  - [Introduccion](#introduccion)
  - [Elementos](#elementos)
    - [Sensor BME280](#sensor)
    - [Raspberry pi 3](#raspberry-pi-3)
    - [Raspberry Pi Azure IoT Online Simulator](#raspberry-pi-azure-iot-online-simulator)
  - [Conectividad](#conectividad)
  - [Analisis de Datos](#analisis-de-datos)

## Introduccion

Para esta practica se realizo un montaje realizado en la nube de Azure. Se utilizo un sensor de presion, temperatura y humedad BME280, una placa raspberry pi 3 model b v1.2 y un Led. Se utilizo Javascript para establecer la comunicacion mediante Node.JS. Finalmente, se uso tambien el laboratorio de pruebas de la nube de Azure para todo el tema de IoT.

## Elementos

### Sensor

Sensor digital BME280 de presión atmosferica, humedad y temperatura. Este sensor tiene un alto rendimiento en todas las aplicaciones que requieren medir humedad y presion, ademas de ser compacto para dispositivos pequeños. El sensor de humedad brinda un tiempo de respuesta extremadamente rapido. Adicionalmente, el sensor de presion, es un sensor barometrico absoluto con una presicion y resolucion extremadamente altas y un ruido menor que otros sensores como el Sensortec BMP180 de Bosch.

El rango de cada medida del sensor son los siguientes.

- Temperatura: -40 - +85°C.
- Humedad relativa: 0 - 100%.
- Presión atmosferica: 300 - 1100 hPa.

Tiene unos parametros para el sensor de humedad:

- Tiempo de respuesta: 1s.
- Tolerancia de exactitud: ±3% humedad relativa.

También para el sensor de temperatura:

- Exactitud de temperatura absoluta (0-65°C): ±1°C

Para el sensor de presión:

- Exactitud absoluta (0-65°C): ±1.0hPa.
- Exactitud relativa: ±0.12hPa.

Por ultimo, este sensor soporta 2 interfaces digitales fundamentales que son i2C y SPI. Para esta practica, el codigo fue programado para que la comunicacion sea mediante una interfaz I2C por medio de los pines GPIO2 y GPIO3 de la placa Raspberry. 

Referencia: [BME280 Datasheet](https://itbrainpower.net/downloadables/BST-BME280-DS002-1509607.pdf) 

### Raspberry pi 3

Se utiliza la Raspberry Pi 3 Modelo B, está placa contiene las siguientes espcificaciones:

- CPU de 4 nucleos Broadcom BCM2837 de 64bit con una velocidad de 1.2GHz.
- RAM de 1GB.
- Chip BCM43438 de Bluetooth y LAN inalambrica.
- 100 Base Ethernet.
- GPIO extendido de 40 pines.
- 4 puertos USB 2.
- Salida estéreo de 4 polos y puerto de vídeo compuesto.
- HDMI de tamaño completo.
- Puerto de cámara CSI para conectar una cámara Raspberry Pi.
- Puerto de pantalla DSI para conectar una pantalla táctil Raspberry Pi.
- Puerto Micro SD para cargar su sistema operativo y almacenar datos.
- Fuente de alimentación Micro USB conmutada mejorada de hasta 2,5A.

Referencia: [Raspberry Pi 3 Model B](https://www.raspberrypi.com/products/raspberry-pi-3-model-b/)

### Raspberry Pi Azure IoT Online Simulator

La plataforma de Azure provee un entorno de pruebas para dispositivos IoT. Para el Rasbperry Pi 3, utiliza las siguientes especificaciones del entorno:

- Sistema operativo Raspberry Pi OS.
- Entorno de ejecución Node.js.
- Aplicación cliente en JavaScript.
- Libreria cliente de protocolo de comunicación MQTT.
- Libreria cliente de dispositivo IoT Azure.
- Libreria sensor BME280.
- Libreria de uso de pines de Raspberry Pi.

Referencia: [Raspberry Pi Web Simulator](https://azure-samples.github.io/raspberry-pi-web-simulator/)

## Conectividad

## Analisis de Datos
