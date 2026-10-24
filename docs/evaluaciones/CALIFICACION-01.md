# Retroalimentación — Taller evaluativo 01

**Estudiante:** Esteban Villalba · **Taller:** Taller evaluativo 01 — Python y estructuras de datos
**Fecha límite:** 2026-10-24 23:59 · **Versión revisada:** commit `b20ac61`

Muy buen trabajo: los nueve ejercicios están bien resueltos y los resultados coinciden con los esperados.

## Nota

| Criterio | Puntos |
|---|---|
| Variables, tipos y operadores (Ej. 1 a 4) | 20 / 20 |
| Condicionales y clasificación (Ej. 5) | 14 / 15 |
| Bucles, acumuladores y control de flujo (Ej. 6 a 8) | 30 / 30 |
| Estructuras de datos nativas (Ej. 9) | 15 / 15 |
| Ejecución sin errores | 6 / 10 |
| Documentación en celdas de texto | 4 / 5 |
| Entrega correcta | 1 / 5 |
| **Total** | **90 / 100** |
| **Nota (0–5)** | **4.50** |

Este taller aporta **13.5 %** de los 15 % del momento evaluativo.

## 1. Variables, tipos y operadores (20 / 20)
**Lo que hizo bien:**
- Las siete variables tienen el tipo correcto y los verificó con `type()`.
- La conversión de unidades y los tres errores salen de operaciones, no de números escritos a mano.
- El Ejercicio 3 usa solo `//` y `%` (resultado: 25 horas, 5 lecturas sobrantes, 1 día y 1 hora).
- El Ejercicio 4 usa `and` y `not` sin ningún `if`, y da los booleanos correctos.

## 2. Condicionales y clasificación (14 / 15)
**Lo que hizo bien:**
- Las cuatro categorías están en el orden correcto y la lectura de 41.8 da "Dañina para grupos sensibles".

**Lo que puede mejorar:**
- Se pidió una sola cadena `if` / `elif` / `else`. Usted puso otro `if` por fuera (para la lectura válida) y una categoría extra "Lectura no válida". Funciona, pero se apartó de lo pedido.

## 3. Bucles, acumuladores y control de flujo (30 / 30)
**Lo que hizo bien:**
- Ejercicio 6: descarta los dos -999.0 con `continue` antes de acumular; da 10 válidas, 2 descartadas y promedio 22.55.
- Ejercicio 7: máximo 58.3, mínimo 7.5 y desviación con dos recorridos, sin `max()`, `min()` ni `sum()`.
- Ejercicio 8: el `while` actualiza la concentración dentro del bloque y termina (10 horas).

## 4. Estructuras de datos nativas (15 / 15)
**Lo que hizo bien:**
- Accede a los datos por clave, desempaqueta las coordenadas en latitud y longitud, y usa `get` con "no disponible" sin errores.

## 5. Ejecución sin errores (6 / 10)
**Lo que hizo bien:**
- El notebook corre completo, sin errores y sin bucles infinitos.

**Lo que puede mejorar:**
- Falta la celda de verificación final que debía copiarse al terminar, así que no se muestra el mensaje "Verificación completada sin errores.".

## 6. Documentación en celdas de texto (4 / 5)
**Lo que hizo bien:**
- Cada ejercicio tiene su celda de texto previa y los nombres de variables son claros.

**Lo que puede mejorar:**
- Falta la celda inicial con el título del taller, su nombre completo y la fecha.

## 7. Entrega correcta (1 / 5)
No siguió la estructura acordada: el notebook debe estar en la carpeta `ejercicios/` con el nombre exacto `taller-evaluativo-01-calidad-del-aire.ipynb`. Su archivo está en la raíz del repositorio con el nombre `Taller_evaluativo_01.ipynb`. Sí se subió a la rama `main` y antes del plazo.

## ¿El notebook funciona?
Sí, corre completo sin errores y los resultados coinciden con los esperados. Lo único que falta es la celda de verificación final.

## Para el próximo taller
- Cree la carpeta `ejercicios/` y suba allí el notebook con el nombre exacto indicado.
- Agregue al inicio una celda con el título, su nombre completo y la fecha.
- Copie al final la celda de verificación sin modificarla y compruebe que imprime el mensaje final.
- Use una sola cadena `if` / `elif` / `else` cuando la guía lo pida.
