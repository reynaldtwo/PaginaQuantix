**TAREA 1**

Tómate un tiempo para analizar EL SIGUIENTE requerimiento "Requerimiento.md" y haz LA planificación donde incluya desde la creacion del proyecto y su arquitectura hasta la entrega completa del sitio. Considerando las reglas descritas en el archivo code-rules.md y apóyate del sitio web "https://docs.astro.build/es/getting-started/" para resolver los errores que aparezcan, así como para investigar sobre las buenas prácticas a la hora de escribir código.


**Trnsformar la seccion Potencia sin límites**

Paso 1 — Cards de Servicios (Desarrollo a la medida) (12)

Título:
Servicios de desarrollo a medida

Subtítulo:
Diseñamos, construimos e integramos software listo para producción: rápido, seguro y escalable. Priorizamos modernización, datos, seguridad y capacidades de IA porque hoy es lo que más presionan las empresas.

Cards (título + texto corto)

Discovery & Roadmap (Producto)
Alineamos objetivos, alcance y entregables. Definimos roadmap, riesgos y estimación realista.

UX/UI & Design Systems
Interfaces claras y consistentes, con accesibilidad y experiencia “premium” desde el día 1.

Desarrollo Web & PWA
Apps web modernas (interna o pública) optimizadas para performance y escalabilidad.

Apps móviles iOS/Android
Desarrollo nativo o multiplataforma con enfoque en estabilidad, rendimiento y releases controlados.

APIs & Integraciones (API-first)
Integramos ERP, POS, pagos, identidad, mensajería y sistemas legados con contratos claros y trazabilidad.

Modernización de sistemas (Legacy → Modern)
Refactor/migración de monolitos y sistemas críticos para reducir deuda técnica y acelerar delivery.

Cloud-native & Microservicios
Arquitecturas modulares, contenedores, serverless cuando aplica, y despliegues seguros.

Data Engineering & BI
Pipelines, calidad de datos, modelos y dashboards ejecutivos para operar con métricas reales.

IA aplicada (GenAI con gobierno)
Asistentes internos, búsqueda inteligente (RAG) y automatizaciones con controles de seguridad y datos.

Seguridad por diseño (Security-by-Design)
Buenas prácticas, hardening, gestión de secretos, revisión de riesgos y cumplimiento desde el desarrollo.

DevOps & CI/CD
Pipelines, despliegues automatizados, rollback, ambientes y gobernanza para releases confiables.

Microsoft Dynamics 365 BC / LS Central (AL)
Extensiones en AL, integraciones, optimización y soporte experto para retail/operación.

CTAs debajo del carrusel (2 botones):

Agendar una llamada

Solicitar propuesta




Paso 2 — Cómo debe quedar el carrusel de servicios (UX + estructura)
1) Estructura de la sección

Izquierda (fijo):

Título + subtítulo

2 CTAs: Agendar una llamada / Solicitar propuesta

Derecha (carrusel):

Cards en scroll horizontal

2) Comportamiento del carrusel

Flecha izquierda / derecha para avanzar/retroceder 1 card (o “1 paso” equivalente a 1 card + gap).

Swipe/drag en móvil (scroll natural).

Sin autoplay por defecto (se percibe más “corporativo” y evita distracciones).

Deshabilitar flechas cuando:

estás al inicio (izquierda)

estás al final (derecha)

3) Responsive (recomendado)

Mobile: 1 card visible

Tablet: 2 cards visibles

Desktop: 3 cards visibles

El resto queda en carrusel.

4) Accesibilidad (obligatorio)

<section aria-labelledby="services-title">

Cards en <ul> y cada card en <li>

Botones con aria-label:

“Anterior” / “Siguiente”

Soporte teclado:

Tab a flechas

Enter/Espacio activa

Respetar prefers-reduced-motion (si hay animación “smooth”, que se reduzca).

5) Diseño de cada card (consistente y “premium”)

Ícono (simple) + título + texto 2–3 líneas

Altura consistente entre cards

Hover sutil (shadow/translate mínimo)

Opcional: link “Ver detalle” (si luego harás página /servicios)

6) Implementación técnica recomendada (sin librerías)

Usar scroll horizontal + CSS scroll-snap:

contenedor con overflow-x: auto; scroll-snap-type: x mandatory

cards con scroll-snap-align: start

Flechas hacen scrollBy() del contenedor.

Esto queda liviano, rápido y fácil de mantener (ideal para sitio global hosteado en Vercel).

**En proceso...**




