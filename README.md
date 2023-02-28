# Cats-and-Dogs
## Clasificación binaria de imágenes de perros y gatos utilizando tensorflow y keras

![image](https://user-images.githubusercontent.com/105322443/221880377-5429baee-d157-4a36-9ba7-8036ec10cab2.png)

### Definimos nuestra carpeta de trabajo con 2000 imágenes

### Entrenamos una red desde cero
* loss='binary_crossentropy'
* optimizer='adam', metrics=['accuracy']) 

### Evaluamos loss y accuracy sobre un conjunto de testeo con 1000 imágenes

---

### Mejoramos el desempeño agregando:

-Subset de validacion para monitoreo del entrenamiento (validation_split=0.2)
* 1600 imágenes para entrenamiento
* 400 imágenes para validación

-Data augmentation
* RandomFlip('horizontal')
* RandomRotation(0.2)

-Transferencia de aprendizaje (transfer-learning) usando VGG16 (imagenet)

### Guardamos en history el desempeño del modelo.

### Graficamos loss y accuracy para interpretar mejor los resultados. 

### Tomamos un batch de imagenes de test y hacemos unas predicciones:
* Etiqueta vs Predition.
---
