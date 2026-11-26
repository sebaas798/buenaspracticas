# Buenas prácticas

Ejercicio de JAP para aplicar buenas prácticas y dejar el código limpio.

## Qué hace el código

`buenaspracticas.js` tiene una función que revisa si un usuario cumple dos requisitos: **ser mayor de 18** y **tener vehículo**. Con los valores de ejemplo (25 años, con vehículo) muestra `true` en la consola.

## Qué hay para mejorar

El código es el punto de partida del ejercicio, y tiene a propósito cosas para corregir:

- **Nombres:** `Edad_del_usuario` y `Comprobar_requisitos_del_usuario` mezclan estilos. En JavaScript se usa camelCase: `edadUsuario`, `cumpleRequisitos`.
- **`if` anidados innecesarios:** todo el bloque se puede escribir en una línea:
  ```js
  const cumpleRequisitos = (edad, tieneVehiculo) => edad >= 18 && tieneVehiculo;
  ```
- **Variables globales:** la edad y el vehículo deberían entrar como parámetros, no estar fijos adentro o afuera de la función.
- **`=== true`** sobra cuando la variable ya es booleana.

## Cómo probarlo

```bash
node buenaspracticas.js
```
