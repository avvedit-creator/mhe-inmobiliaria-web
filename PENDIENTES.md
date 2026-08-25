# Pendiente por decidir con el cliente (My Home Eficiente)

La web actual del cliente (mheinmobiliaria.es) corre sobre una plataforma SaaS de plantillas
para inmobiliarias (ASP.NET, "plantilla6"), con un backend propio ("Login web" + TinyMCE) donde
el agente publica y edita inmuebles sin tocar código.

Este rediseño (`Deploy MHE Inmobiliaria/`) es un sitio **estático** (HTML/CSS/JS, sin base de
datos ni backend). Los 2 inmuebles y el buscador en `inmuebles.html` son de demostración, no
funcionales.

**Antes de que esto sea la web definitiva del cliente**, hay que decidir cómo va a seguir
publicando/editando inmuebles él mismo. Opciones habladas:

1. **CMS headless ligero** (Netlify CMS, Airtable u similar) que alimente la sección de
   inmuebles — el agente rellena un formulario y la web se regenera sola.
2. **Widget externo de terceros** para los listados (como se hizo con Open Properties usando
   el widget de pisos.com), integrado dentro del diseño nuevo.
3. **Backend propio** (base de datos + panel de administración) si el volumen de inmuebles lo
   justifica — esto ya es un proyecto de desarrollo aparte, no solo diseño.

Sin resolver esto, el cliente perdería la capacidad de autogestionar sus inmuebles que ya tiene
hoy con la plataforma actual.
