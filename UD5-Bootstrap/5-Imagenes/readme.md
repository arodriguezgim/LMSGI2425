### 5. Imágenes

Bootstrap ofrece clases útiles para trabajar con imágenes, haciéndolas responsivas y estilizadas de manera sencilla.

#### **5.1. Imágenes responsivas**
Para hacer que una imagen se ajuste automáticamente al ancho de su contenedor, utiliza la clase `img-fluid`:
```html
<img src="imagen.jpg" class="img-fluid" alt="Descripción de la imagen">
```
Esta clase asegura que la imagen escale correctamente en dispositivos de diferentes tamaños.

#### **5.2. Estilos de imágenes**
Bootstrap proporciona clases adicionales para cambiar la forma de las imágenes:
- **`rounded`**: Bordes redondeados.
  ```html
  <img src="imagen.jpg" class="rounded" alt="Imagen con bordes redondeados">
  ```
- **`rounded-circle`**: Forma circular.
  ```html
  <img src="imagen.jpg" class="rounded-circle" alt="Imagen circular">
  ```
- **`img-thumbnail`**: Añade un borde y un fondo a la imagen, similar a una miniatura.
  ```html
  <img src="imagen.jpg" class="img-thumbnail" alt="Miniatura de imagen">
  ```

#### **5.3. Ejemplo práctico de imágenes**
```html
<div class="container">
  <img src="imagen1.jpg" class="img-fluid" alt="Imagen responsiva">
  <img src="imagen2.jpg" class="rounded" alt="Imagen con bordes redondeados">
  <img src="imagen3.jpg" class="rounded-circle" alt="Imagen circular">
  <img src="imagen4.jpg" class="img-thumbnail" alt="Miniatura de imagen">
</div>
```

---
