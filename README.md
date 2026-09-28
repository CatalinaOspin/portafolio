# Portafolio Profesional - Catalina
**Nombre del proyecto en Vercel:** `portafolio_acoc`

Portafolio web responsivo, moderno y de alto impacto visual para Estudiante de Ingeniería Informática y Desarrolladora de Software Full Stack.

## Tecnologías Utilizadas

- **HTML5 Semántico**: Estructura accesible y optimizada para SEO.
- **Tailwind CSS (CDN)**: Sistema de diseño utilitario con paleta de colores personalizada (`primary`, `secondary`, `dark`, `card`).
- **CSS3 Personalizado (`styles.css`)**: Efectos hover, animaciones suaves y scrollbar personalizada.
- **JavaScript Vanilla (`script.js`)**: Manejo de eventos, menú responsivo y formulario de contacto interactivo.
- **Lucide Icons**: Iconografía moderna y ligera.
- **Google Fonts (Plus Jakarta Sans)**: Tipografía estilizada para interfaces digitales.

---

## Estructura del Proyecto

```text
portafolio/
│
├── index.html       # Página principal
├── styles.css       # Estilos personalizados y animaciones
├── script.js        # Lógica de interactividad y eventos
├── vercel.json      # Configuración de despliegue (name: portafolio_acoc)
└── README.md        # Documentación e instrucciones
```

---

## ⚠️ Cambio de Nombre del Proyecto en Vercel

El nombre del proyecto fue actualizado de `portafolio-catalina` a **`portafolio_acoc`** para evitar conflictos con proyectos existentes en Vercel.

Este cambio ya está reflejado en:
- **`vercel.json`** → campo `"name": "portafolio_acoc"`.
- **`index.html`** → meta tag `og:site_name` y metadatos SEO actualizados.

> **Importante:** Si en algún momento aparece una carpeta `.vercel/` generada por un despliegue anterior, **elimínala** antes de volver a desplegar para que Vercel desvincule el proyecto viejo y registre el nuevo nombre correctamente:
> ```bash
> rm -rf .vercel
> ```

---

## Despliegue en Vercel

Este proyecto está 100% listo para ser desplegado como sitio estático en **Vercel**.

### Opción 1: Despliegue automático con GitHub y la consola de Vercel (Recomendado)

1. **Subir los cambios a GitHub:**
   ```bash
   git add .
   git commit -m "feat: cambiar nombre del proyecto a portafolio_acoc"
   git push origin main
   ```

2. **Conectar con Vercel:**
   - Ve a [vercel.com](https://vercel.com/) e inicia sesión.
   - Haz clic en **"Add New..."** > **"Project"**.
   - Selecciona tu repositorio `portafolio` de GitHub.
   - En **Framework Preset**, selecciona **"Other"**.
   - En el campo **Project Name**, escribe exactamente: `portafolio_acoc`.
   - Deja el **Root Directory** como `./`.
   - Haz clic en **Deploy**. ¡Tu sitio estará en línea en segundos con certificado SSL automático!

### Opción 2: Despliegue usando Vercel CLI

Si tienes instalado Vercel CLI en tu terminal:

1. Asegúrate de **no tener** carpeta `.vercel/` (si existe, elimínala con `rm -rf .vercel`).
2. Ejecuta en la raíz del proyecto:
   ```bash
   vercel --name portafolio_acoc
   ```
3. Para desplegar directamente a producción:
   ```bash
   vercel --prod --name portafolio_acoc
   ```
