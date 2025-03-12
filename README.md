# MovieStudio - Blog de Películas

## Descripción General
MovieStudio es una plataforma de streaming y blog de películas desarrollada como proyecto educativo. Este proyecto demuestra la implementación de un sitio web moderno utilizando HTML y CSS.

## Estructura del Sitio
El sitio web consta de 5 páginas principales:
- `index.html` (Página de inicio)
- `info.html` (Características)
- `precios.html` (Planes y precios)
- `faqs.html` (Preguntas frecuentes)
- `about.html` (Acerca de)

## Elementos Comunes

### Encabezado (Header)
- Barra de navegación con enlaces a todas las secciones
- Ícono de perfil de usuario
- Clase `nav_container` para estilo uniforme

### Pie de Página (Footer)
- Enlaces a redes sociales (Facebook, Instagram, Twitter/X)
- Créditos de los desarrolladores
- Iconos y enlaces externos que se abren en nuevas pestañas

## Características Específicas por Página

### Página de Inicio (index.html)
- Título principal con el nombre del sitio
- Sección de tarjetas de películas
- Cada tarjeta contiene:
  - Imagen de la película
  - Título
  - Descripción

### Página de Precios (precios.html)
- Tres planes diferentes:
  - Básico ($10,000 COP/mes)
  - Estándar ($20,000 COP/mes)
  - Premium ($30,000 COP/mes)
- Cada plan muestra sus características específicas

### Página de FAQs (faqs.html)
- Sección de preguntas frecuentes
- Respuestas claras sobre el servicio
- Estructura organizada de preguntas y respuestas

### Página de Características (info.html)
- Descripción de las funcionalidades principales
- Secciones sobre interfaz, calidad HD, multiplataforma
- Diseño limpio y organizado

## Aspectos Técnicos

### HTML Moderno
- Uso de HTML5 con etiquetas semánticas (`<header>`, `<main>`, `<footer>`)
- Metadatos apropiados en el `<head>`
- Estructura bien organizada

### Buenas Prácticas
- Uso de atributos `lang="es"` para especificar el idioma
- Enlaces externos con `target="_blank"` y `rel="noopener noreferrer"`
- Imágenes con atributos `alt` para accesibilidad

### Recursos Externos
- Fuente Roboto de Google Fonts
- Favicon personalizado
- Iconos para redes sociales

## Aspectos de Diseño
- Diseño responsivo con `viewport` configurado
- Sistema de tarjetas para mostrar contenido
- Navegación clara y consistente
- Paleta de colores y estilos definidos en `styles.css`

## Guía de Estilos CSS

### Estructura de Archivos
```
css/
  └── styles.css    # Archivo principal de estilos
```

### Estilos Globales
1. **Configuración Base**
   - Reset de márgenes y padding
   - Configuración de box-sizing
   - Fuente principal: Roboto
   - Colores base del sitio

2. **Variables CSS Recomendadas**
```css
:root {
  --color-primario: #your-color;
  --color-secundario: #your-color;
  --color-texto: #333333;
  --espaciado-base: 1rem;
  --border-radius: 8px;
}
```

### Componentes Principales

1. **Navegación (`nav_container`)**
   - Barra de navegación fija en la parte superior
   - Menú responsive
   - Estilo de enlaces activos/inactivos
   ```css
   .nav_container {
     position: fixed;
     width: 100%;
     padding: 1rem;
     background: white;
     box-shadow: 0 2px 4px rgba(0,0,0,0.1);
   }
   ```

2. **Tarjetas de Películas (`card_container`)**
   - Diseño flexible con grid/flexbox
   - Sombras y efectos hover
   - Imágenes responsivas
   ```css
   .card_container {
     display: flex;
     margin: var(--espaciado-base);
     border-radius: var(--border-radius);
     overflow: hidden;
     transition: transform 0.3s ease;
   }
   ```

3. **Planes de Precios (`pricing-card`)**
   - Diseño de tarjetas destacadas
   - Listas de características
   - Botones de acción
   ```css
   .pricing-card {
     padding: 2rem;
     text-align: center;
     border-radius: var(--border-radius);
     box-shadow: 0 4px 6px rgba(0,0,0,0.1);
   }
   ```

4. **FAQs**
   - Estructura de acordeón
   - Animaciones suaves
   - Estilos de preguntas/respuestas

5. **Footer (`sm_container`)**
   - Grid de iconos sociales
   - Enlaces con efectos hover
   - Créditos y copyright

### Responsive Design
1. **Breakpoints Principales**
```css
/* Móvil */
@media (max-width: 768px) {
  /* Estilos móviles */
}

/* Tablet */
@media (min-width: 769px) and (max-width: 1024px) {
  /* Estilos tablet */
}

/* Desktop */
@media (min-width: 1025px) {
  /* Estilos desktop */
}
```

2. **Consideraciones Responsive**
   - Menú hamburguesa en móvil
   - Reorganización de tarjetas
   - Ajuste de tamaños de fuente
   - Espaciado adaptativo

### Mejores Prácticas CSS
1. **Organización**
   - Usar metodología BEM para nombrar clases
   - Agrupar estilos por componentes
   - Mantener especificidad baja

2. **Optimización**
   - Minimizar anidación
   - Reutilizar clases
   - Usar variables CSS
   - Prefijos automáticos para compatibilidad

3. **Mantenimiento**
   - Comentarios descriptivos
   - Separación de concerns
   - Consistencia en naming
   - Documentación de componentes

## Desarrolladores
- Juan Esteban Mora Rojas
- Cote Dominguez

## Notas Educativas
Este proyecto es un excelente ejemplo de cómo estructurar un sitio web moderno, utilizando buenas prácticas de HTML y manteniendo una consistencia en el diseño a través de todas las páginas. Es especialmente útil como proyecto de aprendizaje porque incorpora muchos elementos fundamentales del desarrollo web front-end. 