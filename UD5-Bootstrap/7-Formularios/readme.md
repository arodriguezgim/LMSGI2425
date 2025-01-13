### 7. Formularios

Los formularios en Bootstrap son altamente personalizables y ofrecen un diseño consistente con el resto del framework. A continuación, se describe cómo trabajar con formularios básicos, controles avanzados y formularios en línea.

#### **7.1. Formularios básicos**
Un formulario típico incluye etiquetas, entradas y botones, organizados con clases de Bootstrap para un diseño limpio:
```html
<form>
  <div class="mb-3">
    <label for="email" class="form-label">Correo Electrónico</label>
    <input type="email" class="form-control" id="email" placeholder="ejemplo@correo.com">
  </div>
  <div class="mb-3">
    <label for="password" class="form-label">Contraseña</label>
    <input type="password" class="form-control" id="password" placeholder="Ingresa tu contraseña">
  </div>
  <div class="mb-3 form-check">
    <input type="checkbox" class="form-check-input" id="remember">
    <label class="form-check-label" for="remember">Recuérdame</label>
  </div>
  <button type="submit" class="btn btn-primary">Iniciar Sesión</button>
</form>
```

#### **7.2. Campos avanzados**
Bootstrap incluye soporte para otros controles de formulario:
- **Selects**: Menús desplegables.
  ```html
  <select class="form-select">
    <option selected>Selecciona una opción</option>
    <option value="1">Opción 1</option>
    <option value="2">Opción 2</option>
    <option value="3">Opción 3</option>
  </select>
  ```
- **Checkbox y radios personalizados**:
  ```html
  <div class="form-check">
    <input type="checkbox" class="form-check-input" id="check1">
    <label class="form-check-label" for="check1">Checkbox personalizado</label>
  </div>
  <div class="form-check">
    <input type="radio" class="form-check-input" id="radio1" name="exampleRadios">
    <label class="form-check-label" for="radio1">Opción 1</label>
  </div>
  ```

#### **7.3. Formularios en línea**
Para formularios compactos, utiliza `row` y `col`:
```html
<form class="row g-3">
  <div class="col-auto">
    <label for="email" class="visually-hidden">Correo Electrónico</label>
    <input type="email" class="form-control" id="email" placeholder="Correo">
  </div>
  <div class="col-auto">
    <label for="password" class="visually-hidden">Contraseña</label>
    <input type="password" class="form-control" id="password" placeholder="Contraseña">
  </div>
  <div class="col-auto">
    <button type="submit" class="btn btn-success mb-3">Enviar</button>
  </div>
</form>
```

