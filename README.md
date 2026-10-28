# EcoMarket - Tienda de Productos Ecológicos y Sostenibles 🌱

**EcoMarket** es una plataforma de e-commerce maquetada exclusivamente con **HTML5 semántico** y **CSS3 puro** (sin JavaScript ni frameworks externos). Está orientada a impulsar el consumo consciente, ofreciendo una experiencia de usuario limpia, accesible, fluida y con enfoque **Mobile-First**.

---

## 📁 Estructura del Proyecto

```text
EcoMarket/
├── css/
│   ├── main.css          # Reset, variables globales de color, tipografía y base
│   ├── layout.css        # Sistema de grid, header, footer y contenedores responsivos
│   ├── components.css    # Tarjetas de producto, botones, filtros, buscador y validaciones
│   └── animations.css    # Transiciones, keyframes y efectos hover
├── img/
│   ├── hero/             # Fondo e imágenes del banner principal
│   ├── icons/            # Iconos vectoriales e imagen estática de ubicación (mapa)
│   └── products/         # Catálogo de imágenes vectoriales de productos (p1.svg a p20.svg)
├── views/
│   ├── productos.html    # Vista B: Catálogo completo de 20 productos con filtros sticky
│   ├── sobre-nosotros.html # Vista C: Historia de marca, principios y carrusel de testimonios
│   └── contacto.html     # Vista D: Formulario con validación CSS y mapa estilizado
├── index.html            # Vista A: Página de Inicio (Home) con hero y productos destacados
└── README.md             # Documentación completa del proyecto
```

---

## 🚀 Especificaciones Técnicas y Funcionalidades

### 1. Requerimientos Funcionales por Vista
- **A. Página de Inicio (`index.html`)**:
  - Header con logotipo, menú de navegación y accesos directos (Carrito con badge contador y Búsqueda).
  - Banner Hero con mensaje motivador (*"Compra responsable, vive sostenible"*) y botón de llamada a la acción (CTA).
  - Grid de productos destacados con efectos hover de elevación suave (`translateY` + `box-shadow`).
  - Footer corporativo con enlaces legales, datos de contacto y redes sociales.
- **B. Catálogo de Productos (`views/productos.html`)**:
  - **Sidebar de Filtros Sticky**: Permanece fija al hacer scroll. Incluye categorías (*Hogar, Moda, Cuidado Personal, Alimentos*), rango de precios y estado de stock.
  - **Grid de 20 Productos**: Layout responsivo en CSS Grid (4 columnas en Desktop, 2 en Tablet, 1 en Móvil).
  - **Interactividad sin JS**: Botón de favoritos funcional mediante el truco de checkbox CSS (`:checked`).
  - **Paginación Visual**: Bloque estilizado al final de la matriz.
- **C. Sobre Nosotros (`views/sobre-nosotros.html`)**:
  - Sección Historia con maquetación en Flexbox.
  - Cuadrícula de Principios Ecológicos (*Sin Plástico, Comercio Justo, Carbono Neutro, Materiales Reciclados*).
  - **Carrusel de Testimonios CSS**: Scroll horizontal fluido (`scroll-snap`) con tarjetas animadas al pasar el cursor.
- **D. Contacto (`views/contacto.html`)**:
  - **Formulario Inteligente**: Campos para Nombre, Email y Mensaje.
  - **Validación Visual CSS Puro**: Retroalimentación automática mediante pseudoclases `:valid` (borde verde) e `:invalid` (borde rojo).
  - **Mapa de Ubicación Estilizado**: Ilustración vectorial estática con indicador pin de localización.
  - **Iconos Sociales**: Animación de escala `scale(1.25)` al hacer hover.

---

## 🎨 Paleta de Colores y Estilo Visual

- **Verde Principal (Sostenibilidad)**: `#2ecc71` / `#27ae60`
- **Verde Menta Claro**: `#e8f8f5`
- **Beige / Tierra Natural**: `#f5f5dc` / `#d35400`
- **Gris Oscuro (Lectura)**: `#2c3e50`
- **Tipografía**: System UI Sans-Serif clara y accesible.

---

## 🛠️ Instrucciones de Visualización y Despliegue

### Visualización Local
1. Descarga y descomprime el archivo `EcoMarket_ProyectoCompleto.zip`.
2. Abre la carpeta `EcoMarket/`.
3. Haz doble clic sobre `index.html` para abrir la plataforma en cualquier navegador web moderno (Chrome, Firefox, Edge, Safari).

### Despliegue Inmediato en Internet
Para desplegar el proyecto en servicios como **Vercel** o **Netlify**:
1. Sube la carpeta a un repositorio de GitHub (ej. `EcoMarket_NombreApellido`).
2. Conecta tu cuenta de GitHub a **Vercel** o **Netlify**.
3. Selecciona el repositorio. Al ser un sitio estático (`HTML/CSS`), la raíz del despliegue es `./` e `index.html` se cargará de manera inmediata.

---

## 🌿 Gestión de Versiones (Git Workflow)

Organización recomendada siguiendo la metodología **Conventional Commits** y **GitFlow**:

### Ramas
- `main`: Producción lista para despliegue.
- `develop`: Desarrollo de integración.
- `feature/home`: Maquetación de `index.html` y Hero.
- `feature/catalogo`: Desarrollo del catálogo de 20 productos y filtros sticky.
- `feature/sobre-nosotros`: Implementación de historia y carrusel CSS de testimonios.
- `feature/contact-form`: Formulario de contacto con validaciones visuales CSS.

### Historial de Commits del Proyecto
1. `feat(init): inicializar estructura de carpetas y config base`
2. `feat(css): crear variables globales, reset y sistema de grid en CSS`
3. `feat(home): maquetar header, hero banner y productos destacados en index.html`
4. `feat(catalog): construir grid de 20 productos con etiquetas de stock y boton favoritos`
5. `feat(filters): agregar sidebar de filtros sticky y barra de busqueda`
6. `feat(about): implementar seccion historia, principios ecologicos y carrusel CSS`
7. `feat(contact): crear formulario de contacto con validacion CSS :valid/:invalid`
8. `docs(readme): agregar documentacion completa del proyecto EcoMarket`