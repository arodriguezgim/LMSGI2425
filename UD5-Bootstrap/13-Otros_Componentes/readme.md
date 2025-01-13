### 13. Tooltips y Popovers  

Los **tooltips** y **popovers** son componentes interactivos que muestran mensajes o información adicional al pasar el cursor o hacer clic en un elemento.  

#### **13.1. Tooltips**  
Los tooltips son mensajes pequeños que aparecen cuando un usuario pasa el ratón sobre un elemento.  

##### **Ejemplo básico de tooltip**  
```html
<button type="button" class="btn btn-secondary" data-bs-toggle="tooltip" data-bs-placement="top" title="Este es un tooltip">
  Pasa el ratón aquí
</button>
```  

##### **Inicializar tooltips con JavaScript**  
Para que los tooltips funcionen, debes inicializarlos:  
```html
<script>
  const tooltipTriggerList = [].slice.call(document.querySelectorAll('[data-bs-toggle="tooltip"]'))
  const tooltipList = tooltipTriggerList.map(function (tooltipTriggerEl) {
    return new bootstrap.Tooltip(tooltipTriggerEl)
  })
</script>
```  

#### **13.2. Popovers**  
Los popovers son más grandes que los tooltips y permiten mostrar más contenido.  

##### **Ejemplo básico de popover**  
```html
<button type="button" class="btn btn-primary" data-bs-toggle="popover" title="Título del Popover" data-bs-content="Este es el contenido del popover.">
  Haz clic aquí
</button>
```  

##### **Inicializar popovers con JavaScript**  
Al igual que con los tooltips, es necesario inicializarlos:  
```html
<script>
  const popoverTriggerList = [].slice.call(document.querySelectorAll('[data-bs-toggle="popover"]'))
  const popoverList = popoverTriggerList.map(function (popoverTriggerEl) {
    return new bootstrap.Popover(popoverTriggerEl)
  })
</script>
```  

#### **13.3. Opciones avanzadas**  
Puedes personalizar la posición, colores o comportamiento de los tooltips y popovers mediante clases y configuraciones adicionales.  

##### **Ejemplo con opciones avanzadas**  
```html
<button type="button" class="btn btn-success" data-bs-toggle="tooltip" data-bs-placement="bottom" title="Tooltip en la parte inferior">
  Tooltip Avanzado
</button>

<button type="button" class="btn btn-warning" data-bs-toggle="popover" data-bs-trigger="hover" title="Título Personalizado" data-bs-content="Este popover aparece al pasar el ratón.">
  Popover Avanzado
</button>
```  

---

