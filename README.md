# Portal Corporativo W&M Global C.A. - Astro Project

Proyecto web moderno construido con [Astro](https://astro.build) y [Tailwind CSS](https://tailwindcss.com), migrado y optimizado a partir del diseño estático original.

## 🚀 Estructura del Proyecto

```text
├── public/                     # Recursos estáticos servidos en la raíz
│   ├── screen.png              # Captura de pantalla del diseño
│   └── images/                 # Imágenes optimizadas (logos, fondos, etc.)
│       ├── logo.png
│       ├── hero-refinery.jpg
│       ├── engineers.jpg
│       ├── location-map.jpg
│       └── screen.png
├── src/
│   ├── assets/                 # Copia de recursos y multimedia
│   ├── components/             # Componentes modulares de Astro
│   │   ├── Header.astro        # Barra de navegación fija con menú móvil
│   │   ├── Hero.astro          # Sección principal con banner y llamados a la acción
│   │   ├── About.astro         # Misión, visión, valores y certificaciones
│   │   ├── Services.astro      # Catálogo de 8 servicios con carrusel interactivo
│   │   ├── Experience.astro    # Métricas operativas con contadores y marco legal
│   │   ├── Contact.astro       # Formulario técnico, datos de contacto y mapa
│   │   └── Footer.astro        # Pie de página y enlaces
│   ├── layouts/
│   │   └── Layout.astro        # Layout base HTML5, SEO y tipografías (Google Fonts)
│   ├── pages/
│   │   └── index.astro         # Página principal del portal
│   └── styles/
│       └── global.css          # Estilos globales y animaciones Tailwind
├── astro.config.mjs            # Configuración de Astro e integración de Tailwind
├── tailwind.config.mjs         # Tokens de diseño (paleta Industrial Integrity)
└── package.json
```

## 🛠️ Comandos Disponibles

| Comando | Acción |
| :--- | :--- |
| `npm install` | Instala las dependencias del proyecto |
| `npm run dev` | Inicia el servidor de desarrollo local |
| `npm run build` | Compila el sitio estático para producción en `./dist` |
| `npm run preview` | Previsualiza localmente la compilación de producción |
