### 12. Acordeones  

Los **acordeones** son componentes de Bootstrap que permiten mostrar y ocultar contenido de forma dinámica al hacer clic, ideales para mostrar secciones extensas de información sin saturar la pantalla.  

#### **12.1. Acordeón básico**  
Para crear un acordeón básico, usa el componente `accordion`:  
```html
<div class="accordion" id="accordionExample">
  <div class="accordion-item">
    <h2 class="accordion-header" id="headingOne">
      <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
        Sección 1
      </button>
    </h2>
    <div id="collapseOne" class="accordion-collapse collapse show" aria-labelledby="headingOne" data-bs-parent="#accordionExample">
      <div class="accordion-body">
        Contenido de la sección 1. Puedes incluir texto, imágenes o cualquier otro elemento.
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header" id="headingTwo">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
        Sección 2
      </button>
    </h2>
    <div id="collapseTwo" class="accordion-collapse collapse" aria-labelledby="headingTwo" data-bs-parent="#accordionExample">
      <div class="accordion-body">
        Contenido de la sección 2. Personaliza según tus necesidades.
      </div>
    </div>
  </div>
</div>
```  

#### **12.2. Acordeón con múltiples secciones abiertas**  
Para permitir que varias secciones estén abiertas al mismo tiempo, elimina el atributo `data-bs-parent`:  
```html
<div class="accordion" id="accordionExample">
  <div class="accordion-item">
    <h2 class="accordion-header" id="headingOne">
      <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
        Sección 1
      </button>
    </h2>
    <div id="collapseOne" class="accordion-collapse collapse show" aria-labelledby="headingOne">
      <div class="accordion-body">
        Contenido de la sección 1.
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header" id="headingTwo">
      <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo" aria-expanded="true" aria-controls="collapseTwo">
        Sección 2
      </button>
    </h2>
    <div id="collapseTwo" class="accordion-collapse collapse" aria-labelledby="headingTwo">
      <div class="accordion-body">
        Contenido de la sección 2.
      </div>
    </div>
  </div>
</div>
```  

#### **12.3. Estilización de los acordeones**  
Puedes personalizar los estilos añadiendo clases adicionales o modificando el diseño:  
```html
<div class="accordion accordion-flush" id="accordionFlushExample">
  <div class="accordion-item">
    <h2 class="accordion-header" id="flush-headingOne">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#flush-collapseOne" aria-expanded="false" aria-controls="flush-collapseOne">
        Acordeón Estilo Flush
      </button>
    </h2>
    <div id="flush-collapseOne" class="accordion-collapse collapse" aria-labelledby="flush-headingOne" data-bs-parent="#accordionFlushExample">
      <div class="accordion-body">
        Contenido con bordes minimalistas.
      </div>
    </div>
  </div>
</div>
```  

