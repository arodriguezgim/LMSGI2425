### 3. El Sistema Grid

El sistema Grid de Bootstrap es una de las características más potentes del framework. Permite crear diseños responsivos fácilmente, dividiendo la pantalla en un sistema de 12 columnas. A continuación, se explican los conceptos básicos y cómo utilizarlos:

#### **3.1. Conceptos básicos**
- **Contenedor (`.container`)**: Es el elemento principal que contiene las filas y columnas. Puede ser fijo (`.container`) o fluido (`.container-fluid`).
- **Filas (`.row`)**: Agrupan las columnas para crear una estructura de diseño.
- **Columnas (`.col-*`)**: Son los elementos dentro de las filas que definen el contenido y su tamaño relativo. Se utiliza un sistema de 12 columnas.

#### **3.2. Estructura básica de Grid**
```html
<div class="container">
  <div class="row">
    <div class="col">Columna 1</div>
    <div class="col">Columna 2</div>
    <div class="col">Columna 3</div>
  </div>
</div>
```
En este ejemplo, las tres columnas ocuparán el mismo espacio dentro de la fila.

#### **3.3. Tamaños de columna y puntos de quiebre**
Bootstrap ofrece diferentes clases para controlar el ancho de las columnas según el tamaño de la pantalla:
- **`col-sm-*`**: Para pantallas pequeñas (>=576px).
- **`col-md-*`**: Para pantallas medianas (>=768px).
- **`col-lg-*`**: Para pantallas grandes (>=992px).
- **`col-xl-*`**: Para pantallas extra grandes (>=1200px).
- **`col-xxl-*`**: Para pantallas aún más grandes (>=1400px).

Ejemplo:
```html
<div class="container">
  <div class="row">
    <div class="col-md-6">Columna 1</div>
    <div class="col-md-6">Columna 2</div>
  </div>
</div>
```
En este caso, las columnas ocuparán la mitad del ancho (6/12) en pantallas medianas o más grandes.

#### **3.4. Anidación de columnas**
Puedes anidar columnas dentro de otras columnas para diseños más complejos:
```html
<div class="container">
  <div class="row">
    <div class="col">
      Columna principal
      <div class="row">
        <div class="col">Columna anidada 1</div>
        <div class="col">Columna anidada 2</div>
      </div>
    </div>
  </div>
</div>
```

#### **3.5. Ejemplo práctico de Grid**
```html
<div class="container">
  <div class="row">
    <div class="col-sm-4">Columna 1 (4/12)</div>
    <div class="col-sm-4">Columna 2 (4/12)</div>
    <div class="col-sm-4">Columna 3 (4/12)</div>
  </div>
</div>
```
Este ejemplo muestra cómo dividir el espacio en tres columnas iguales en pantallas pequeñas o más grandes.

---

