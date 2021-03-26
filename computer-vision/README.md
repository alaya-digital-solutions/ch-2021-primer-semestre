# COMPUTER VISION
[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

### SETUP

```sh
$ echo seteo de tu ambiente de trabajo
git clone git@github.com:alaya-digital-solutions/challenges
$ cd challenges
$ echo usa tu ambiente predefinido, venv, conda u otro para instalar los requirements
$ pip install -r requirements.txt
```

### PROBLEMA Y SOLUCIÓN BUSCADA
El desafio consiste en identificar la cantidad y tipo de moneda en una imagen (6 tipos). En primer lugar se debe realizar la detección de las monedas utilizando únicamente algoritmos o técnicas de visión computacional y a continuación deberás implementar un modelo que realice la clasificación. Las tareas de detección de objetos en imágenes es un problema típico y puede ser aplicado en un sin número de áreas, existen arquitecturas de Deep Learning como R-CNN y YOLO que se pueden implementar para estas tareas, pero en esta ocación (de acuerdo a la dificultad del DS) se debe solucionar la detección a través de técnicas de CV y la clasificación abierto a cualquier modelo.

Ejemplo imagen:

![Imagen de ejemplo](https://github.com/alaya-digital-solutions/challenges/blob/main/computer-vision/images/Ejemplo.jpg)

### PREGUNTAS
Peguntas que nos interesan saber ! 

1. Cuántas monedas hay en la imagen?
2. Es factible realizar la clasificación con un sistema no supervisado?
3. Cómo solucionarías las escasez de datos?
4. Cuáles son las métricas de clasificación?
5. Cuánto tiempo toma realizar la inferencia?

### QUE ENTREGAR?

Para las imágenes de test (data/raw/Test_Random) se debe generar un csv donde se resuma la cantidad total de monedas y la cantidad por tipo (ver archivo de ejemplo).

### DIRECTORIO IMÁGENES
- 5C: Imágenes con monedas de 5 centavo
- 1E: Imágenes con monedas de 1 euro
- 2E: Imágenes con monedas de 2 euro
- 10C: Imágens con monedas de 10 centavos
- 20C: Imágens con monedas de 20 centavos
- 50C: Imágens con monedas de 50 centavos
- Train_Random: Imágenes con monedas de los 6 tipos para entrenamiento
- Test_Random: Imágenes con monedas de los 6 tipos para Test

### ANEXOS
En caso de tener un equipo para desarrollar la solución no dudes en utilizar Google Ccolaboratory (https://colab.research.google.com/) !
