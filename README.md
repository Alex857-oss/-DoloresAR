# Dolores AR

App turística con **realidad aumentada** para visitar Dolores Hidalgo, Guanajuato.
Desarrollo Móvil Integral · UTNG

## ¿Qué hace?

- **RA por ubicación:** con GPS + brújula calcula qué lugares quedan frente al usuario y dibuja etiquetas con su nombre y distancia.
- **Pasaporte turístico:** se gana un sello al acercarse a menos de 40 m de un lugar.
- **Modelo 3D:** muestra un modelo 3D con `model_viewer_plus` (ARCore / Quick Look).
- **Modo demo:** simula la posición y la brújula (con un deslizador) para practicar sin estar en Dolores Hidalgo.

## Pruebas

    flutter test

## Evidencia de TDD (ciclo Rojo → Verde por ronda)

En cada ronda se escribe primero la prueba, se ve fallar (rojo), se implementa lo mínimo para que pase (verde) y después se mejora el código.

### Ronda 1: Geo (cálculos de ubicación)
**Rojo:** la prueba falla porque aún no existe `geo.dart`.

![Ronda 1 rojo](capturas/ronda1_rojo.png)

**Verde:** con `geo.dart` implementado, la prueba pasa.

![Ronda 1 verde](capturas/ronda1_verde.png)

### Ronda 2: Motor de RA
**Rojo:**

![Ronda 2 rojo](capturas/ronda2_rojo.png)

**Verde:**

![Ronda 2 verde](capturas/ronda2_verde.png)

### Ronda 3: Pasaporte
**Rojo:**

![Ronda 3 rojo](capturas/ronda3_rojo.png)

**Verde:**

![Ronda 3 verde](capturas/ronda3_verde.png)

### Ronda 4: ARViewModel
**Rojo:**

![Ronda 4 rojo](capturas/ronda4_rojo.png)

**Verde:**

![Ronda 4 verde](capturas/ronda4_verde.png)

### Resultado final: todas las pruebas pasando
![Todas las pruebas](capturas/final_todas_verde.png)
![Todas las pruebas](capturas/final_todas_verdes.png)
![Todas las pruebas](capturas/pruebas.png)

Cubren distancia, rumbo, cruce del norte, campo de visión, motor de RA, pasaporte y ViewModel.


## Evidencias

### Funcionamiento de la App
![pruebas](capturas/imagen01.jpeg)
![pruebas](capturas/imagen02.jpeg)
![pruebas](capturas/imagen03.jpeg)
