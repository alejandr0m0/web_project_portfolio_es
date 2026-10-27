# Portafolio de Alejandro Márquez

Portafolio personal desarrollado como proyecto del sprint 4 del programa de
desarrollo web de TripleTen. Presenta mi perfil, habilidades, proyectos y medios de
contacto mediante una página responsiva basada en el diseño proporcionado en Figma.

## Sitio publicado

[Ver el portafolio en GitHub Pages](https://alejandr0m0.github.io/web_project_portfolio_es/)

## Contenido

- **Perfil:** presentación personal, fotografía, acceso al CV y navegación hacia el
  contacto.
- **Habilidades y herramientas:** iconos de las tecnologías y herramientas del
  perfil.
- **Proyectos destacados:** una tarjeta para la página web de una cafetería y otra
  reservada para un próximo proyecto.
- **Contacto:** correo electrónico y perfiles de LinkedIn y X.

## Tecnologías y técnicas

- HTML5 semántico y CSS3, sin JavaScript ni frameworks.
- Flexbox para organizar los elementos y media queries para adaptar el diseño.
- Metodología BEM con clases del tipo `block__element--modifier`.
- CSS separado por bloques e importado desde `styles/styles.css`.
- Normalize.css como base para los estilos del navegador.
- Fuentes Open Sans y Archivo Black cargadas localmente en formatos WOFF y WOFF2.
- Imágenes de proyectos con proporción 16:9 y recorte mediante `object-fit`.
- Degradados radiales para las luces del fondo y degradados lineales para el velo
  de las tarjetas y los subrayados del perfil.
- Estados de interacción al pasar el cursor y foco visible para la navegación con
  teclado.

## Estructura del proyecto

```text
web_project_portfolio_es/
├── index.html                 # Contenido y estructura de la página
├── README.md
├── assets/                    # CV en PDF
├── fonts/                     # Fuentes locales y sus reglas @font-face
├── images/                    # Fotografía, vistas previas e iconos
│   └── icons/
└── styles/
    ├── styles.css             # Punto de entrada de los estilos
    ├── normalize.css
    └── blocks/
        ├── page.css
        ├── profile.css
        ├── skills.css
        ├── projects.css
        ├── project-card.css
        └── contact.css
```

Cada bloque contiene sus estilos base y sus propias media queries. Los bloques
compartidos, como `project-card`, se reutilizan mediante clases BEM.

## Ejecución local

El sitio es estático y no requiere instalar dependencias ni ejecutar un proceso de
compilación.

1. Descarga o clona el proyecto y abre su carpeta en Visual Studio Code.
2. Si utilizas la extensión Live Server, haz clic derecho sobre `index.html` y
   selecciona **Open with Live Server**.
3. Abre la dirección local que indique la extensión para visualizar el sitio.

También puedes abrir `index.html` directamente en el navegador.

## Diseño responsivo

Los estilos se adaptan a tres intervalos principales:

| Dispositivo | Ancho de pantalla | Organización                                                                             |
| ----------- | ----------------- | ---------------------------------------------------------------------------------------- |
| Escritorio  | Desde 1024 px     | Perfil y fotografía en paralelo; proyectos en dos columnas.                              |
| Tableta     | De 768 a 1023 px  | Fotografía más pequeña y proyectos en una columna.                                       |
| Móvil       | Hasta 767 px      | Fotografía sobre el perfil, enlaces apilados y habilidades distribuidas en varias filas. |

El diseño toma como referencia los anchos de 320, 768 y 1440 px y también se revisó
en resoluciones intermedias. Las imágenes y los contenedores se ajustan al espacio
disponible para mantener la distribución entre los puntos de ruptura.

## Mejoras pendientes

- Incorporar un segundo proyecto cuando esté disponible.
- Revisar la biografía y la presentación profesional para reflejar con mayor
  precisión mi experiencia actual.
