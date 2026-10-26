# Retroalimentación — Taller evaluativo 03 (NumPy)

**Estudiante:** Esteban Villalba · **Taller:** Taller evaluativo 03 — NumPy
**Fecha límite:** 2026-10-26 23:59 · **Versión revisada:** commit `e12c042`

¡Muy buen trabajo con los ejercicios! Los resultados son correctos.

## Nota

| Criterio | Puntos |
|---|---|
| Creación y atributos de arreglos (Ej. 1) | 10 / 10 |
| Indexación y slicing (Ej. 2) | 10 / 10 |
| Máscaras booleanas (Ej. 3) | 15 / 15 |
| Vectorización y broadcasting (Ej. 4) | 11 / 15 |
| Estadística por eje y funciones universales (Ej. 5 y 6) | 20 / 20 |
| Integración (Ej. 7) | 10 / 10 |
| Ejecución sin errores | 6 / 10 |
| Documentación | 4 / 5 |
| Entrega correcta | 1 / 5 |
| **Total** | **87 / 100** |
| **Nota (0–5)** | **4.35** |

Este taller aporta **13.1 %** de los 15 % del momento evaluativo.

## 1. Creación y atributos de arreglos (10 / 10)
**Lo que hizo bien:**
- `lecturas_crudas` se creó con `np.array` desde una lista de listas y sus atributos se leyeron del arreglo.
- `dias`, `pendientes` e `interceptos` son correctos.

## 2. Indexación y slicing (10 / 10)
**Lo que hizo bien:**
- Cada resultado sale de una sola expresión, con índice negativo donde se pedía, y `bloque` tiene forma (3, 4).

## 3. Máscaras booleanas (15 / 15)
**Lo que hizo bien:**
- `es_util` une dos comparaciones entre paréntesis con `&`, hay 2 faltantes, 5 lecturas útiles y el promedio es 27.0.

## 4. Vectorización y broadcasting (11 / 15)
**Lo que hizo bien:**
- Convirtió pendientes e intercepto en columnas (5, 1) y `calibradas` da los valores esperados sin bucles.
- `promedio_calibrado_sbc_a` es 31.9.

**Lo que puede mejorar:**
- Faltó la celda de texto que explica por qué multiplicar una tabla de forma (5, 7) por un vector de forma (5,) da error. Esa explicación era parte del ejercicio.
**Cómo corregirlo:**
- Agregue, justo antes del código del Ejercicio 4, una celda de texto que diga que una tabla de 5 filas y 7 columnas no se puede multiplicar por un vector de 5 valores porque NumPy compara las formas desde la última columna (7 contra 5) y no coinciden. Añada que por eso se convierte el vector en columna de forma (5, 1), que sí se ajusta a las 5 filas.

## 5. Estadística por eje y funciones universales (20 / 20)
**Lo que hizo bien:**
- Los promedios por sensor y por día, los máximos y la media sobre 35.4 (43.275) son correctos.
- Usó `np.maximum`, `np.abs`, `np.round` y trabajó `en_alerta` sobre una copia, con 8 celdas mayores que 0.

## 6. Integración (10 / 10)
**Lo que hizo bien:**
- Los conteos (9, 18, 7 y 1) suman 35, `dia_pico` es 5 y las dos líneas de salida coinciden con lo pedido.

## 7. Ejecución sin errores (6 / 10)
**Lo que hizo bien:**
- El notebook corre completo sin ningún error.

**Lo que puede mejorar:**
- No incluyó la celda de verificación final, así que nunca aparece el mensaje "Verificación completada sin errores.". Debía copiarla al final del notebook sin cambios.
**Cómo corregirlo:**
- Abra la guía del taller, copie la celda de verificación completa en una celda de código nueva al final del notebook, sin cambiar nada, y ejecútela. Debe aparecer "Verificación completada sin errores."; si sale un error, corrija el ejercicio que menciona y vuelva a ejecutar.

## 8. Documentación (4 / 5)
**Lo que hizo bien:**
- Cada ejercicio tiene una celda de texto previa y los nombres de variables siguen `snake_case`.

**Lo que puede mejorar:**
- La celda inicial solo tiene el título: faltan su nombre completo y la fecha.
- Faltó la explicación del error de formas en el Ejercicio 4.
**Cómo corregirlo:**
- En la primera celda escriba, bajo el título, su nombre completo y la fecha de entrega.
- Añada la celda de texto del Ejercicio 4 descrita arriba.

## 9. Entrega correcta (1 / 5)
**Lo que puede mejorar:**
- No siguió la estructura acordada: el notebook debe estar en la carpeta `ejercicios/` con el nombre exacto `taller-evaluativo-03-numpy.ipynb`. Usted lo subió a la raíz del repositorio como `Taller_evaluativo_03.ipynb`.
- El trabajo sí es visible en GitHub antes del plazo.
**Cómo corregirlo:**
- Cree la carpeta `ejercicios/` en la raíz del repositorio, mueva allí el notebook y cámbiele el nombre a `taller-evaluativo-03-numpy.ipynb`. Luego súbalo a la rama `main` y revise en GitHub que se vea en esa ruta.

## ¿El notebook funciona?
Sí, corre de principio a fin sin errores y todos los resultados coinciden con los esperados. Lo único es que falta la celda de verificación final.

## Para el próximo taller
- Guarde el notebook en `ejercicios/` con el nombre exacto que pide la guía.
- Copie la celda de verificación al final y confirme que imprime el mensaje de éxito.
- Escriba en la primera celda el título, su nombre completo y la fecha.
- Lea todos los puntos de cada ejercicio, incluidos los que piden explicar con texto.
