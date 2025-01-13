# 4. Tipografías y Estilos de Texto

Bootstrap incluye una tipografía moderna y flexible por defecto, con clases que permiten aplicar estilos rápidamente.

#### **4.1. Fuente predeterminada**
La fuente utilizada por defecto en Bootstrap es "Helvetica Neue", Arial, sans-serif. Sin embargo, puedes cambiarla si lo necesitas.

#### **4.2. Clases para textos**
- **`display-*`**: Clases para títulos grandes y destacados.
  ```html
  <h1 class="display-1">Display 1</h1>
  <h2 class="display-2">Display 2</h2>
  ```
- **`lead`**: Para resaltar un párrafo principal.
  ```html
  <p class="lead">Este es un párrafo destacado.</p>
  ```
- **Alineación del texto**:
  - `text-start`: Alineado a la izquierda (por defecto).
  - `text-center`: Centrado.
  - `text-end`: Alineado a la derecha.
  ```html
  <p class="text-center">Texto centrado.</p>
  ```
- **Colores del texto**:
  - Bootstrap incluye clases como `text-primary`, `text-success`, `text-danger`, etc., para aplicar colores predeterminados.
  ```html
  <p class="text-success">Texto en verde.</p>
  ```

#### **4.3. Ejemplo práctico de tipografía**
```html
<div class="container">
  <h1 class="display-3 text-primary">Título Destacado</h1>
  <p class="lead text-muted">Este es un párrafo principal con un estilo más tenue.</p>
  <p class="text-end text-danger">Texto alineado a la derecha y en rojo.</p>
</div>
```

