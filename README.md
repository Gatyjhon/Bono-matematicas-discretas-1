# Bono de Programación: Matemáticas Discretas I

**Universidad Nacional de Colombia** **John Angel Novoa Martinez**  
**Docente:** Jhoan Sebastian Tenjo García  

Este repositorio contiene la solución a dos problemas generales de conteo (Permutaciones y Combinaciones), desarrollando herramientas computacionales en Python que validan, calculan y detallan el procedimiento matemático paso a paso.

---

## Instrucciones de Ejecución

El proyecto fue desarrollado en formato *Jupyter Notebook* para integrar la explicación matemática (LaTeX) con el código en Python. Tienes dos opciones para ejecutarlo:

**Opción A: Google Colab**
1. Descarga el archivo `Bono_combinarotira_John_Novoa.ipynb` de este repositorio.
2. Abre [Google Colab](https://colab.research.google.com/).
3. Ve a `Archivo` > `Subir notebook` y carga el archivo.
4. Presiona `Entorno de ejecución` > `Ejecutar todas` para ver los resultados y pruebas automáticas.

**Opción B: Entorno Local**
Si tienes Python y Jupyter instalados en tu PC, puedes clonar este repositorio y ejecutar el notebook localmente:

git clone https://github.com/Gatyjhon/Bono-matematicas-discretas-1#
jupyter notebook Bono_combinarotira_John_Novoa.ipynb

## Explicación de los Problemas Resueltos

Problema 1: Calculadora de Permutaciones P(n,r) 
Calcula de cuántas maneras se pueden organizar r objetos tomados de un conjunto de n objetos distintos, donde el orden sí importa.

Fórmula: P(n,r) = n! / (n-r)  

El algoritmo verifica que no existan valores negativos y que r no sea mayor que n antes de realizar el cálculo mediante una función factorial propia.

Problema 2: Calculadora de Combinaciones C(n,r)
Calcula de cuántas formas se pueden escoger r objetos de un conjunto de n distintos, donde el orden no importa.

Fórmula: C(n,r) = n! / (r!*((n-r)!)) 

Adicionalmente, el código comprueba la Propiedad Simétrica C(n,r) = C(n, n-r) y cuenta con una función extra para generar gráficamente el Triángulo de Pascal.


## Ejemplos de Entrada, Salida y Pruebas

El programa está diseñado para no "romperse" si el usuario ingresa datos ilógicos, respetando el modelo matemático.

Ejemplo de un Caso Exitoso:

Entrada: calcular_permutacion(10, 3)

Salida esperada:
Procedimiento matemático: P(10,3) = 10! / (10-3)!
--> Sustituyendo valores: P(10,3) = 3628800 / 5040
Resultado: 720

Ejemplo de Validación de Error:

Entrada: calcular_combinacion(3, 5)

Salida esperada:
No se puede ordenar mas objetos de los totales
Resultado: 0

Nota: Al ejecutar el cuaderno completo, se desplegará una batería de 10 pruebas automáticas que abarcan casos pequeños, medianos, extremos y el renderizado del Triángulo de Pascal centrado.
