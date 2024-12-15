# Tensores

Los tensores son una generalización de matrices para un número arbitrario de dimensiones.

## Tipos de Tensores

- **Escalar (0D):** Tensor que contiene solo un número. Ejemplo: `float32` → Tensor Escalar.
- **Vector (1D):** Cadena de números con un solo eje.  
  Ejemplo: `x = [1, 4, 2, 5]`
- **Matriz (2D):** Cadena de vectores, representando un tensor 2D.

Al unir matrices en una nueva cadena, se obtiene un **tensor 3D**.  
Al unir tensores 3D en una cadena, se crea un **tensor 4D**, y así sucesivamente.

## Atributos Clave de los Tensores

1. **Número de ejes (Rango):** La cantidad de dimensiones que tiene el tensor.
2. **Forma:** Las longitudes de los ejes del tensor.
3. **Tipo de datos:** El tipo de valores que contiene (e.g., `float32`, `int32`, etc.).
