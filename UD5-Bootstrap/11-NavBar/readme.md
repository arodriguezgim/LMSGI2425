### 11. Navbars  

Las **navbars** en Bootstrap son barras de navegación que ofrecen una estructura lista para personalizar y utilizar en cualquier tipo de proyecto.  

#### **11.1. Navbar básica**  
Una navbar básica incluye un contenedor `nav` con la clase `navbar` y otras clases para el color, diseño y comportamiento:  
```html
<nav class="navbar navbar-expand-lg navbar-light bg-light">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Mi Sitio</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page" href="#">Inicio</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Enlace</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Contacto</a>
        </li>
      </ul>
    </div>
  </div>
</nav>
```  

#### **11.2. Navbar fija**  
Para fijar una barra de navegación en la parte superior o inferior, utiliza las clases `fixed-top` o `fixed-bottom`:  
```html
<nav class="navbar navbar-light bg-light fixed-top">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Navbar Fija</a>
  </div>
</nav>
```  

#### **11.3. Navbar con dropdowns**  
Puedes añadir menús desplegables con `dropdown`:  
```html
<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Navbar</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarDropdown" aria-controls="navbarDropdown" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarDropdown">
      <ul class="navbar-nav">
        <li class="nav-item">
          <a class="nav-link" href="#">Inicio</a>
        </li>
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" id="dropdownMenuLink" role="button" data-bs-toggle="dropdown" aria-expanded="false">Menú</a>
          <ul class="dropdown-menu" aria-labelledby="dropdownMenuLink">
            <li><a class="dropdown-item" href="#">Opción 1</a></li>
            <li><a class="dropdown-item" href="#">Opción 2</a></li>
          </ul>
        </li>
      </ul>
    </div>
  </div>
</nav>
```  

#### **11.4. Navbar con formularios**  
Es posible incluir un formulario dentro de la barra de navegación:  
```html
<nav class="navbar navbar-light bg-light">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Mi Sitio</a>
    <form class="d-flex">
      <input class="form-control me-2" type="search" placeholder="Buscar" aria-label="Buscar">
      <button class="btn btn-outline-success" type="submit">Buscar</button>
    </form>
  </div>
</nav>
```  

---

