# duckduinoES-keyboard
# Rubber Ducky USB para Teclado en Español (ES)

Este proyecto te permite convertir una placa Arduino Mega o Uno en un Rubber Ducky USB con la distribución de teclado en español de España, con fines éticos y educativos. El Rubber Ducky USB es una herramienta que simula un teclado en un dispositivo USB y puede automatizar secuencias de pulsaciones de teclas.

**Nota:** Este proyecto es útil si estás utilizando un sistema operativo con la distribución del teclado en español de España, ya que de lo contrario, los caracteres especiales podrían interpretarse incorrectamente.

## Requisitos

Antes de comenzar, asegúrate de tener instalado `dfu-programmer`. Puedes instalarlo utilizando el siguiente comando:

```bash
sudo apt install dfu-programmer
```
También será necesario instalar el IDE de Arduino

## Configuración de la Placa

Este repositorio está preparado para la placa Arduino Mega 2560 Rev3 y utiliza el chip Atmega16U2 para simular el dispositivo USB. Si estás utilizando otra placa Arduino o tu CPU no es el Atmega16U2, deberás seguir estos pasos:
1. Descarga el firmware correspondiente para tu placa y CPU desde: https://github.com/arduino/ArduinoCore-avr/tree/master/firmwares/atmegaxxu2
2. Reemplaza el firmware descargado en el directorio del proyecto.
3. En `script.sh` , asegúrate de actualizar el nombre del archivo de firmware correspondiente y el modelo de CPU en las variables adecuadas.

Una vez el descargado el firmware correcto, puedes seguir el siguiente video de [@s4vitar](https://github.com/s4vitar) donde explica como proceder a cargarlo en la placa, junto con el archivo .ino (timestamp 9:00): https://www.youtube.com/watch?v=W6uGHYBAhHQ 
