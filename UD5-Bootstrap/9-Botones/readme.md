### 9. Botones

Bootstrap proporciona un conjunto completo de estilos para botones que se pueden personalizar con diferentes colores, tamaños y opciones.

#### **9.1. Tipos de botones**
Las clases principales de botones incluyen:
- `btn-primary`: Estilo principal.
- `btn-secondary`: Estilo secundario.
- `btn-success`: Éxito.
- `btn-danger`: Peligro.
- `btn-warning`: Advertencia.
- `btn-info`: Información.
- `btn-light`: Claro.
- `btn-dark`: Oscuro.

Ejemplo:
```html
<button type="button" class="btn btn-primary">Primario</button>
<button type="button" class="btn btn-secondary">Secundario</button>
<button type="button" class="btn btn-danger">Peligro</button>
```

#### **9.2. Botones outline**
Los botones outline son versiones con borde que no tienen relleno de color:
```html
<button type="button" class="btn btn-outline-primary">Primario</button>
<button type="button" class="btn btn-outline-success">Éxito</button>
<button type="button" class="btn btn-outline-danger">Peligro</button>
```

#### **9.3. Tamaños de botones**
Bootstrap permite ajustar el tamaño de los botones:
- `btn-lg`: Botones grandes.
- `btn-sm`: Botones pequeños.

Ejemplo:
```html
<button type="button" class="btn btn-primary btn-lg">Grande</button>
<button type="button" class="btn btn-secondary btn-sm">Pequeño</button>
```

#### **9.4. Botones deshabilitados**
Desactiva botones añadiendo el atributo `disabled` o la clase `disabled`:
```html
<button type="button" class="btn btn-secondary" disabled>Deshabilitado</button>
```

#### **9.5. Grupos de botones**
Organiza varios botones en línea con `btn-group`:
```html
<div class="btn-group" role="group">
  <button type="button" class="btn btn-primary">Izquierda</button>
  <button type="button" class="btn btn-primary">Centro</button>
  <button type="button" class="btn btn-primary">Derecha</button>
</div>
```

