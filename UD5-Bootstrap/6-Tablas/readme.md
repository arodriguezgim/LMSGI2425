
### 6. Tablas

Bootstrap facilita la creación de tablas estilizadas y responsivas.

#### **6.1. Tablas básicas**
Para crear una tabla básica con estilos predeterminados, utiliza la clase `table`:
```html
<table class="table">
  <thead>
    <tr>
      <th scope="col">#</th>
      <th scope="col">Nombre</th>
      <th scope="col">Apellido</th>
      <th scope="col">Correo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">1</th>
      <td>Juan</td>
      <td>Pérez</td>
      <td>juan@example.com</td>
    </tr>
    <tr>
      <th scope="row">2</th>
      <td>Ana</td>
      <td>López</td>
      <td>ana@example.com</td>
    </tr>
  </tbody>
</table>
```

#### **6.2. Estilos adicionales para tablas**
- **Filas sombreadas**: Añade la clase `table-striped`.
- **Bordes en las celdas**: Usa `table-bordered`.
- **Hover en las filas**: Aplica `table-hover`.
- **Tabla compacta**: Usa `table-sm` para reducir el espaciado.

Ejemplo:
```html
<table class="table table-striped table-bordered table-hover table-sm">
  <thead>
    <tr>
      <th>#</th>
      <th>Nombre</th>
      <th>Apellido</th>
      <th>Correo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>Juan</td>
      <td>Pérez</td>
      <td>juan@example.com</td>
    </tr>
    <tr>
      <td>2</td>
      <td>Ana</td>
      <td>López</td>
      <td>ana@example.com</td>
    </tr>
  </tbody>
</table>
```

#### **6.3. Tablas responsivas**
Para que las tablas se adapten a pantallas pequeñas, envuélvelas en un contenedor con la clase `table-responsive`:
```html
<div class="table-responsive">
  <table class="table">
    <!-- Contenido de la tabla -->
  </table>
</div>
```

