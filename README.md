# Practica 2, parte 1

| usuario   | Rol               | Persona      | Actividad   |
| --------- | ------------------| ------------|--------------|
| jreyesgar93|Programación     | José        | Pipeline Kale|
| yalidt    | Programación  | Yalidt      | Revisión del paquete|
| yefovar   | Programación  | Yedam          | Revisión del paquete|
| mfrubio   | Project Manager        | Fernanda    | Montar servicios|

## Paquete Simplex
Implementamos un paquete en Python que resuelve problemas de maximización de una función objetivo lineal con restricciones:

![equation](https://latex.codecogs.com/gif.latex?max_{x}\quad&space;c^{T}x) 

sujeto a:

![equation](https://latex.codecogs.com/gif.latex?Ax\leq&space;b)

![equation](https://latex.codecogs.com/gif.latex?x\geq&space;0) 

con:

![equation](https://latex.codecogs.com/gif.latex?c,x\quad\epsilon\quad\mathbb{R}^{n})

![equation](https://latex.codecogs.com/gif.latex?A\quad\epsilon\quad\mathbb{R}^{m\times&space;n})

![equation](https://latex.codecogs.com/gif.latex?b\quad\epsilon\quad\mathbb{R}^{m})

Usamos sphynx para documentar nuestro [paquete.](https://optimizacion-2-2021-1-gh-classroom.github.io/practica-1-segunda-parte-yefovar/Simplex.html#module-Simplexs)

En particular, se indicó que existen imágenes de docker que ayudan a utilizar el paquete (sin y con Kale) tal como se muestra en la siguiente imagen.
<img src="lanzamientos_pipeline/Images/Documentacion%20paquete%20-%20Docker.png">

### Botón de binder 
Para consultar ejemplos de implementaciones usa el boton de binder y el notebook para realizar el *testing* es 3_parte_2_practica_1.ipynb

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/optimizacion-2-2021-1-gh-classroom/practica-1-segunda-parte-yefovar/main?urlpath=lab)

### Actualizacion y mejoras del paquete
Todas las actualizaciones y mejoras al código se realizaron en el repositorio [anterior.](https://github.com/optimizacion-2-2021-1-gh-classroom/practica-1-segunda-parte-yefovar) `optimizacion-2-2021-1-gh-classroom/practica-1-segunda-parte-yefovar`

### Historial de lanzamientos de kale
Para revisar la documentación de los lanzamientos se puede accesar al siguiente [reporte.](https://github.com/optimizacion-2-2021-1-gh-classroom/practica-2-primera-parte-yefovar/blob/main/lanzamientos_pipeline/Lanzamientos.ipynb) 

Se realizaron cinco lanzamientos, los cuales corresponden a lo siguiente:
1. Prueba Kale
<img src="lanzamientos_pipeline/Images/Testing Kale 1 - Success.jpeg">
2. Debugg algorithm
<img src="lanzamientos_pipeline/Images/pipeline_success_2.png">
3. Mejoras al paquete
<img src="lanzamientos_pipeline/Images/success_lanch_3.png">
4. Solución Unbounded
<img src="lanzamientos_pipeline/Images/launch_4_success.png">
5. Pipeline Práctica 1 LA Bike Share
<img src="lanzamientos_pipeline/Images/launch_5 - success 2.jpeg">
