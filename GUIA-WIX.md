# Guía para implementar el diseño en Wix

Sitio: **Drjoaquinramirez.cl** · ID `50286075-d59f-4c68-9714-4db874020752`
Editor clásico (no Studio) · Velo habilitado · Premium con dominio propio
Referencia visual: [`sitio-web.html`](sitio-web.html)

---

## ⚠️ Antes de empezar

Este sitio está **publicado y en producción desde enero de 2021**. Tiene historial de SEO acumulado y apps activas (Blog, Bookings, Members Area, Multilingual, Forms).

1. **Trabaja sobre una copia.** En el panel de Wix: *Duplicar sitio* → trabaja sobre el duplicado → cuando esté aprobado, aplicas los cambios al sitio real. Nunca edites y publiques directo sobre el live.
2. **No cambies las URLs de las páginas existentes.** Si una página cambia de slug, pierdes su posicionamiento salvo que configures una redirección 301 (Wix lo permite en *SEO → Redirecciones de URL*).
3. **No elimines páginas** que hoy reciben tráfico. Revísalo antes en Google Search Console.

---

## 1. Paleta — configúrala en el tema del sitio

En el Editor: *Sitio → Colores del sitio → Editar colores*. Define estos 5 y úsalos siempre desde ahí (nunca colores sueltos por elemento, o el día que ajustes algo tendrás que tocar 200 elementos).

| Rol | Hex | Uso |
|---|---|---|
| Verde salvia | `#86BE9C` | Fondos de sección plenos, chips, acentos |
| Verde profundo | `#3F7256` | **Texto y botones** — el salvia es muy claro para texto |
| Dorado arena | `#CBB984` | Fondos de sección, acentos, barra del logo |
| Gris texto | `#58595B` | Cuerpo de texto |
| Crema | `#FAF8F4` | Fondo general del sitio |

**Regla de contraste, verificada:** sobre fondo claro usa gris `#58595B` o verde profundo `#3F7256`. El salvia y el dorado **solo como fondo**, con texto oscuro encima. Nunca texto salvia sobre blanco: no cumple accesibilidad y se lee mal en celular con sol.

## 2. Tipografía

El logo usa una sans humanista ligera con versalitas espaciadas. Para que no peleen:

- **Si tienes el archivo de la fuente del logo**, súbela: *Sitio → Fuentes → Subir fuente* (disponible en Premium). Es la mejor opción.
- **Si no**, usa de la biblioteca de Wix la más cercana. Candidatas, en orden: **Lato Light**, **Jost Light**, **Work Sans Light**. Compara en pantalla contra el logo antes de decidir.

Escala de tamaños (desktop):

| Elemento | Tamaño | Peso | Extra |
|---|---|---|---|
| Titular hero | 56-80 px | Light / 200-300 | Interlineado 1.0 |
| Título de sección | 32-46 px | Light | Interlineado 1.05 |
| Bajada / lead | 20 px | Light | |
| Cuerpo | 17 px | Regular | Interlineado 1.7 |
| Etiquetas ("CIRUGÍA FACIAL") | 13 px | Semibold | **Mayúsculas + tracking 0.2em** |

La jerarquía va **por tamaño, no por peso**. Nada de negritas grandes.

## 3. Estructura de secciones

En el mismo orden del HTML. Cada una es una *Sección* del Editor con su color de fondo:

| # | Sección | Fondo | Contenido |
|---|---|---|---|
| 1 | Hero | Crema | Titular, bajada, 2 botones, fila de chips de credenciales |
| 2 | Historia | **Salvia pleno** | Foto retrato + bio (texto oscuro) |
| 3 | Cirugías | Crema | 3 grupos: facial, corporal, no quirúrgicos |
| 4 | Tecnología | **Dorado pleno** | Lista de plataformas como píldoras |
| 5 | Antes y después | **Blanco** | Galería + disclaimer |
| 6 | Contenido | Crema | 3 tarjetas: podcast, episodios, blog |
| 7 | Afiliaciones | Salvia muy claro `#EDF5F0` | SCCP, AEXPI, ISAPS, InMode |
| 8 | Agenda | **Verde profundo** | Contacto + botón de reserva |

**La sección 5 va en blanco a propósito.** Sin color pleno ni gráficos: es la regla de compliance — nada decorativo sobre fotos de resultados.

**Aire vertical:** 100-130 px arriba y abajo de cada sección en desktop, 60-70 px en móvil. Es lo que más diferencia un sitio cuidado de uno apretado.

## 4. Elementos concretos

- **Botones:** esquinas totalmente redondeadas (píldora). Principal = relleno verde profundo con texto crema. Secundario = solo borde. Texto en mayúsculas, 13 px, tracking 0.13em.
- **Chips de credenciales** (Pitanguy, U. de los Andes, SCCP, ISAPS, AEXPI): cajas de texto con fondo redondeado. Alterna salvia, salvia claro y dorado.
- **Índice de procedimientos:** dos columnas — nombre a la izquierda, descripción a la derecha — separadas por una línea fina de 1 px. En móvil se apilan. No uses tarjetas con sombra.
- **Motivos botánicos:** las hojas y flores del HTML. Exporta cada una como PNG transparente en verde salvia y colócalas como imagen decorativa, grandes y saliéndose por el borde, con opacidad ~15-20%. Márcalas como decorativas (sin texto alt) para que no ensucien la accesibilidad.
- **Logo:** cabecera con la variante de fondo blanco (`jr-02`), footer con la de fondo negro (`jr-05`). Sube los PNG a *Media* y ponlos como imagen, no como texto.

## 5. SEO — lo que hay que configurar en Wix

Wix ya tiene la app **Promote SEO** instalada. Por cada página, en *SEO básico*:

- **Título** único, 55-60 caracteres, con la palabra clave y la ubicación. Ej: `Rinoplastía en Santiago | Dr. Joaquín Ramírez, Cirujano Plástico`
- **Descripción** 150-160 caracteres, escrita para que la persona haga clic.
- **Slug** limpio y en español: `/cirugias/rinoplastia`, no `/page-1`.
- **Texto alt** en toda imagen con contenido.

Los valores por defecto de Wix son malos. Sobrescríbelos todos.

**Una página por procedimiento.** Hoy tienes una sola página de "Cirugías y procedimientos" con todo junto: eso compite consigo mismo y no posiciona para ninguna búsqueda específica. Trece páginas individuales rinden mucho más que una general.

**E-E-A-T:** cada página con contenido clínico necesita tu nombre y credenciales visibles, y una fecha de última revisión. Google trata la salud como YMYL y exige ese estándar; es donde más fácil se gana ventaja sobre la competencia.

## 6. Datos estructurados — pégalo en Wix

Esto es lo que más pesa para que ChatGPT, Perplexity y los AI Overviews te citen (~81% de las páginas que los motores de IA citan tienen datos estructurados). Wix **no lo genera solo**.

Ve a *Configuración → Código personalizado → Agregar código* → colócalo en el `<head>`, cargado en **todas las páginas**:

```html
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Physician",
  "@id": "https://www.drjoaquinramirez.cl/#physician",
  "name": "Dr. Joaquín Ramírez Sneberger",
  "medicalSpecialty": "PlasticSurgery",
  "url": "https://www.drjoaquinramirez.cl/",
  "telephone": "+56998750386",
  "email": "contacto@drjoaquinramirez.cl",
  "address": {
    "@type": "PostalAddress",
    "streetAddress": "San Sebastián 2839, Oficina 211",
    "addressLocality": "Las Condes",
    "addressRegion": "Región Metropolitana",
    "addressCountry": "CL"
  },
  "areaServed": { "@type": "City", "name": "Santiago" },
  "availableService": [
    { "@type": "MedicalProcedure", "name": "Rinoplastía" },
    { "@type": "MedicalProcedure", "name": "Lifting facial o ritidoplastía" },
    { "@type": "MedicalProcedure", "name": "Blefaroplastía" },
    { "@type": "MedicalProcedure", "name": "Lipoinjerto facial" },
    { "@type": "MedicalProcedure", "name": "Mamoplastía de aumento" },
    { "@type": "MedicalProcedure", "name": "Mamoplastía reductora" },
    { "@type": "MedicalProcedure", "name": "Mastopexia" },
    { "@type": "MedicalProcedure", "name": "Abdominoplastía" },
    { "@type": "MedicalProcedure", "name": "Lipoaspiración" },
    { "@type": "MedicalProcedure", "name": "Ginecomastía" }
  ],
  "founder": { "@id": "https://www.drjoaquinramirez.cl/#person" }
}
</script>

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Person",
  "@id": "https://www.drjoaquinramirez.cl/#person",
  "name": "Joaquín Ramírez Sneberger",
  "honorificPrefix": "Dr.",
  "jobTitle": "Cirujano Plástico",
  "url": "https://www.drjoaquinramirez.cl/",
  "worksFor": { "@type": "MedicalClinic", "name": "Leblon Plastic Surgery" },
  "alumniOf": [
    { "@type": "CollegeOrUniversity", "name": "Universidad de los Andes" },
    { "@type": "EducationalOrganization", "name": "Instituto Ivo Pitanguy, Río de Janeiro" }
  ],
  "memberOf": [
    { "@type": "Organization", "name": "Sociedad Chilena de Cirugía Plástica, Reconstructiva y Estética (SCCP)" },
    { "@type": "Organization", "name": "International Society of Aesthetic Plastic Surgery (ISAPS)" },
    { "@type": "Organization", "name": "Asociación de Ex Alumnos del Instituto Ivo Pitanguy (AEXPI)" }
  ],
  "sameAs": [
    "https://www.instagram.com/joaquinramirezsneberger",
    "https://www.tiktok.com/@joaquinramirezs",
    "https://www.linkedin.com/in/joaquinramirezsneberger",
    "https://www.facebook.com/joaquinramirezsneberger"
  ]
}
</script>
```

> Revisa que las URLs de redes y la dirección estén exactas antes de publicarlo — un dato equivocado aquí se propaga a Google y a los modelos de IA.

Verifica después en la [prueba de resultados enriquecidos de Google](https://search.google.com/test/rich-results).

## 7. AEO — para aparecer en buscadores de IA

- **NAP idéntico** carácter por carácter en el sitio, Google Business Profile, Instagram, LinkedIn y directorios. `+56 9 9875 0386` escrito de dos formas distintas cuenta como dos entidades diferentes.
- **FAQ por procedimiento**, con la pregunta real como encabezado y la respuesta directa en las primeras dos frases. Márcala con `FAQPage`.
- **`llms.txt`** en la raíz del dominio, resumiendo quién eres y cuáles son tus páginas canónicas.
- **No bloquees los crawlers de IA** en robots.txt (`GPTBot`, `PerplexityBot`, `ClaudeBot`, `Google-Extended`). Si los bloqueas, no apareces. En Wix se edita en *SEO → Editar robots.txt*.

## 8. Rendimiento

Wix carga JavaScript pesado por defecto. Lo que sí controlas:

- Comprime toda imagen antes de subirla (WebP, bajo 200 KB).
- No instales apps que no uses — cada una suma carga.
- Modera las animaciones de entrada de Wix.
- Mide en [PageSpeed Insights](https://pagespeed.web.dev/) antes y después.

---

## Orden sugerido

1. Duplicar el sitio
2. Configurar paleta y fuentes en el tema
3. Rehacer la home sección por sección
4. Pegar los datos estructurados
5. Revisar en móvil (más de la mitad de tu tráfico)
6. Corregir títulos, descripciones y slugs de todas las páginas
7. Recién ahí, aplicar al sitio real y publicar
8. Verificar en Search Console que no cayó nada
