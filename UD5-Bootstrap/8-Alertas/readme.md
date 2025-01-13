### 8. Alertas

Bootstrap permite crear mensajes visuales para captar la atención del usuario. Las alertas son altamente personalizables y se pueden cerrar dinámicamente.

#### **8.1. Creación de alertas básicas**
Las alertas se implementan con la clase `alert`, junto con clases de color para representar distintos niveles de importancia:
```html
<div class="alert alert-primary" role="alert">
  Este es un mensaje de información.
</div>
<div class="alert alert-danger" role="alert">
  Este es un mensaje de error.
</div>
```

Clases de color disponibles:
- `alert-primary`, `alert-secondary`, `alert-success`, `alert-danger`, `alert-warning`, `alert-info`, `alert-light`, `alert-dark`.

#### **8.2. Alertas con enlaces**
Se pueden añadir enlaces dentro de las alertas para proporcionar información adicional:
```html
<div class="alert alert-warning" role="alert">
  Atención: <a href="#" class="alert-link">Consulta más detalles aquí</a>.
</div>
```

#### **8.3. Alertas con botón de cierre**
Bootstrap permite cerrar alertas utilizando botones con la clase `btn-close` y atributos como `data-bs-dismiss`:
```html
<div class="alert alert-success alert-dismissible fade show" role="alert">
  <strong>Éxito:</strong> Operación completada correctamente.
  <button type="button" class="btn-close" data-bs-dismiss="alert" aria-label="Cerrar"></button>
</div>
```

