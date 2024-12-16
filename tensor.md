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


# Manipular tensor

## Seleccionar Elementos en un Tensor

Seleccionar elementos específicos en un tensor se llama **"Cortar el tensor"**.

El siguiente ejemplo selecciona los números del índice `#10` al índice `#100`:

```python
my_slice = train_images[10:100]
print(my_slice.shape)
# Salida: (90, 28, 28)
```
otras formas de escribir lo mismo :  
```python
  my_slice = train_images[10:100, :, :]   
```
   ó
```python 
  my_slice = train_images[10:100, 0:28, 0:28]
```
## La noción de lotes de datos

En general, el primer eje (el 0 porque el indice empieza en 0) de todos los tensores de datos
con los que se encuentre en el deep learning van a ser el **"eje de muestras"**

## Ejemplos de tensores de datos en el mundo real

- **Datos vectoriales:** Tensores 2D  con forma (muestra, caracteristica)
- **Datos de series temporales o de secuencia:** Tensores 3D con forma (muestras, pasos de tiempo, caracteristicas)
- **Imágenes:** Tensores de 4D con forma (muestra, altura, anchura, canales) ó (muestras, canales, altura, anchura)
- **Vídeo:** Tensores 5D con forma (muestra, fotogramas, altura, anchura, canales) ó (Muestras, fotogramas, canales, altura, anchura)




