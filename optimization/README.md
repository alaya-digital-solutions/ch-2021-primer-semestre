# OPTIMIZACIÓN
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
* El contexto: Los datos son una muestra sintetica de un problema minero de transporte de mineral, el cúal conciste en mover mineral desde un punto A a un punto B, del cual se producirá una cantidad de cobre estimada de %utilización (o ley de cobre) * cantidad transportada.
* Las restricciones del problema son que en en cada punto se debe extraer como mínimo 600 toneladas de mineral, por cada ciclo de transporte (origen-destino-origen) se transportan aproximadamente 300 toneladas.
* El objetivo es encontrar la cantidad exacta de ciclos que se debe extraer en cada punto (ciclo = [origen, destino, origen]), minimizando la cantidad de distancia recorrida de la flota, de tal manera de cumplir la meta productiva de las próximas 2 semanas, que es producir 30.000 toneladas de cobre.

### PREGUNTAS
Peguntas que nos interesan saber ! 

1. ¿Es factible resolver el problema con los datos que tienes, argumenta?
2. ¿Es lineal el problema?
3. ¿omo plantearias el problema en papel y lapiz?
4. ¿Que librerías usarías? [Pulp, CVXopt, Scipy, etc..]
5. Escribe el código
6. Es escalable tu solución
7. ¿Como lo harías si te digo que ahora que las toneladas transportadas dependen del trayecto?

### QUE ENTREGAR?

Un .csv con la columna trayectos y los ciclos de transporte en cada trayecto
ver archivo de ejemplo


### DICCIONARIO DE DATOS
* trayecto: Corresponden a los trayectos disponibles, los cuales se encuetran en formato string de la forma origen / destino, son todos los posibles trayectos que pueden realizarse
* %utilizacion: ley del cobre, de ese trayecto, ejemplo: con un % de utilización del 0.1[%] si saco 300 toneladas del trayecto [alpha / beta] el cobre que produciría es 300 * 0.1 / 100 = 0.3 toneladas de cobre. 
* kms_trayecto: km que tiene el trayecto [alpha / beta] siguiendo (desde origen a destino) --> (origen-destino-origen) = 2 veces esta distancia
* tiempo_ciclo: tiempo que se tardan en recorrer este trayecto

### ANEXO
Este es un problema más que resuelto en muchas industrias, sobre todo en minería. Este desafío propone encontrar nuevas maneras de abordar estas problemáticas, que son comunes a una diversa gamma de industrias.








