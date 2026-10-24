# Retroalimentación — Taller evaluativo 02 (Funciones y POO)

**Estudiante:** Esteban Villalba · **Taller:** Taller evaluativo 02 — Funciones y POO
**Fecha límite:** 2026-10-24 23:59 · **Versión revisada:** commit `b20ac61`

Muy buen trabajo: los ocho ejercicios están resueltos y dan los resultados esperados.

## Nota

| Criterio | Puntos |
|---|---|
| Funciones: parámetros, valores por defecto y retorno (Ej. 1 a 3) | 20 / 20 |
| `map`, `filter` y `lambda` (Ej. 4) | 10 / 10 |
| Clases, atributos y métodos (Ej. 5 y 7) | 15 / 15 |
| Encapsulamiento y validación (Ej. 6) | 15 / 15 |
| `__repr__` y `__str__` (Ej. 6 a 8) | 10 / 10 |
| Integración de funciones y clases (Ej. 8) | 10 / 10 |
| Ejecución sin errores | 6 / 10 |
| Documentación | 3 / 5 |
| Entrega correcta | 1 / 5 |
| **Total** | **90 / 100** |
| **Nota (0–5)** | **4.50** |

Este taller aporta **13.5 %** de los 15 % del momento evaluativo.

## 1. Funciones: parámetros, valores por defecto y retorno (20 / 20)
**Lo que hizo bien:**
- `calibrar_lectura` tiene los valores por defecto en la firma y usa `return`.
- `es_lectura_valida` clasifica bien -999.0, 600.0, 25.0 y 0.0.
- `promedio_valido` reutiliza `es_lectura_valida`, da 27.0 y devuelve `None` si no hay lecturas válidas.

## 2. `map`, `filter` y `lambda` (10 / 10)
**Lo que hizo bien:**
- Obtuvo las 5 lecturas calibradas (de 11.5 a 61.9) y las 2 excedencias, sin bucles ni comprensiones.

## 3. Clases, atributos y métodos (15 / 15)
**Lo que hizo bien:**
- `Lectura` guarda sus tres datos con valores por defecto y convierte bien 0.0252 mg/m3 a 25.2.
- `Estacion` guarda objetos `Lectura` y `valores()` usa `a_microgramos()`; coincide con `lecturas_sbc_a`.

## 4. Encapsulamiento y validación (15 / 15)
**Lo que hizo bien:**
- `Sensor` lanza `ValueError` con código vacío o pendiente menor o igual a cero, antes de guardar datos.
- Usa `_pendiente` y `_intercepto`, y `calibrar` reutiliza `calibrar_lectura`.
- No dejó celdas de prueba que fallen.

## 5. `__repr__` y `__str__` (10 / 10)
**Lo que hizo bien:**
- Los textos de `Sensor`, `Estacion` e `InformeEstacion` coinciden exactamente con lo pedido.

## 6. Integración de funciones y clases (10 / 10)
**Lo que hizo bien:**
- `InformeEstacion` da 31.9 y "Moderada" reutilizando las funciones y el método `calibrar` del sensor.
- `categoria_pm25` usa una sola cadena `if` / `elif` / `else` y cubre bien las cuatro categorías.

## 7. Ejecución sin errores (6 / 10)
**Lo que hizo bien:** el notebook corre completo, sin ningún error.
**Lo que puede mejorar:**
- Falta la celda de verificación final, que debía copiarse al final del notebook. Por eso no aparece el mensaje "Verificación completada sin errores.".

## 8. Documentación (3 / 5)
**Lo que hizo bien:** cada ejercicio tiene su celda de texto previa, y las funciones y métodos tienen docstring de una línea. Los nombres siguen las convenciones.
**Lo que puede mejorar:**
- Las clases `Lectura`, `Sensor`, `Estacion` e `InformeEstacion` no tienen docstring propio.
- La primera celda de texto debía tener título, su nombre completo y la fecha; solo tiene el título.

## 9. Entrega correcta (1 / 5)
**Lo que puede mejorar:**
- No siguió la estructura acordada: el notebook debe estar en la carpeta `ejercicios/` con el nombre exacto `taller-evaluativo-02-funciones-y-poo.ipynb`. Su archivo está en la raíz del repositorio y se llama `Taller_evaluativo_02.ipynb`.
- Sí está en la rama `main`, visible en GitHub y subido a tiempo.

## ¿El notebook funciona?
Sí: corre completo sin errores y todos los resultados coinciden con los esperados (27.0, 5 lecturas calibradas, 2 excedencias, 25.2, 31.9 y "Moderada"). Lo único que falta es la celda de verificación final.

## Para el próximo taller
- Copie la celda de verificación al final del notebook y ejecútela antes de entregar.
- Ponga en la primera celda el título, su nombre completo y la fecha.
- Escriba también un docstring de una línea en cada clase.
- Cree la carpeta `ejercicios/` y guarde allí el notebook con el nombre exacto que indica la guía.
