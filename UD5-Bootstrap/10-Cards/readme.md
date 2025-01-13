### 10. Cards  

Las **cards** en Bootstrap son contenedores flexibles y extensibles que se utilizan para agrupar contenido en bloques visualmente atractivos. Son ideales para mostrar información estructurada como títulos, imágenes, texto y botones.  

#### **10.1. Estructura básica de una card**  
Una card básica incluye un contenedor `div` con la clase `card` y otros elementos como encabezados, cuerpos o pies de página:  
```html
<div class="card" style="width: 18rem;">
  <img src="https://via.placeholder.com/150" class="card-img-top" alt="...">
  <div class="card-body">
    <h5 class="card-title">Título de la Card</h5>
    <p class="card-text">Este es un ejemplo de texto dentro de una card. Puedes añadir cualquier contenido aquí.</p>
    <a href="#" class="btn btn-primary">Ir a algún lugar</a>
  </div>
</div>
```  

#### **10.2. Cards con listas**  
Se pueden incluir listas dentro de las cards utilizando las clases de lista estándar:  
```html
<div class="card" style="width: 18rem;">
  <div class="card-header">
    Encabezado de la Card
  </div>
  <ul class="list-group list-group-flush">
    <li class="list-group-item">Elemento 1</li>
    <li class="list-group-item">Elemento 2</li>
    <li class="list-group-item">Elemento 3</li>
  </ul>
</div>
```  

#### **10.3. Cards en grupo**  
Las cards pueden organizarse en un grupo utilizando `card-group`:  
```html
<div class="card-group">
  <div class="card">
    <img src="https://via.placeholder.com/150" class="card-img-top" alt="...">
    <div class="card-body">
      <h5 class="card-title">Título 1</h5>
      <p class="card-text">Texto de ejemplo para la primera card.</p>
    </div>
  </div>
  <div class="card">
    <img src="https://via.placeholder.com/150" class="card-img-top" alt="...">
    <div class="card-body">
      <h5 class="card-title">Título 2</h5>
      <p class="card-text">Texto de ejemplo para la segunda card.</p>
    </div>
  </div>
</div>
```  

#### **10.4. Cards horizontales**  
Para crear una disposición horizontal, utiliza `d-flex flex-row`:  
```html
<div class="card mb-3" style="max-width: 540px;">
  <div class="row g-0">
    <div class="col-md-4">
      <img src="https://via.placeholder.com/150" class="img-fluid rounded-start" alt="...">
    </div>
    <div class="col-md-8">
      <div class="card-body">
        <h5 class="card-title">Título Horizontal</h5>
        <p class="card-text">Texto en disposición horizontal.</p>
      </div>
    </div>
  </div>
</div>
```  

