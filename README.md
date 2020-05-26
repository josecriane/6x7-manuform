# 67Manuform
## Motivación
La idea es crear un teclado de estilo manuform más grande de lo normal, por lo que fué necesario realizar un par de modificaciones, en el modelo 3d y el firmware. La idea de este repositorio es servir de documentación/log de todo el proceso.

## Fuentes
Las pricipales fuentes de para la elaboración de este proyecto fueron:
Para el diseño del teclado se usó como base [Dactyl Manuform](https://github.com/abstracthat/dactyl-manuform)

Para el firmware se usó [QMK](https://github.com/qmk/qmk_firmware)

## Customizaciones del diseño 3d

## Construcción del teclado
#### Material
* Diodos:
* Teensy 2.0
* Resistencias 2K2: 2
* Switches:
* Extensor de puertos MCP23017*

### Soldadura de los switches.
El diseño de la carcasa hace que algunos switches sean de muy dificil acceso por lo que decidí que no soldaría los diodos directamente a los switches sino que utilizaría cables que fueran directos a una placa donde ya estuviesen soldados los diodos.

### Diseño y construcción de las placas perforadas
La idea inicial era fabricar una pcb pero para no alargar más el proyecto decidí cambiar de idea y realizarlo utilizando placas perforadas.

Primero os presento la placa `master`.

PLACA_MASTER_BLA_BLA

Un problema que se me presentó es que historicamente este teclado, como el ergodox utilizan extensores de puertos MCP23018, pero al comprarlos me equivoqué y compré MCP23017, que en principio deberían de funcionar, pero como no tenía la certeza decidí crear la placa `slave` de forma que pudiera cambiar de extensor de puertos sin tener que volver a soldar todo. (Sin tener el teclado terminado considero que este razonamiento fué erroneo y que en caso de querer cambiar de `mcp` debería de haber creado una placa nueva).

PLACA_SLAVE_BLA_BLA

### Aprendiendo de los errores

## Customización del firmware

### Otros firmwares de mis teclados.
ManuformPad (https://github.com/josecriane/qmk_firmware/tree/customization/josecriane)

## Depth data
* Número de soldaduras:

