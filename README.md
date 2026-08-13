# Identidad de marca — Dr. Joaquín Ramírez Sneberger

> **Hay dos marcas en este proyecto.** Esta es la **marca personal (JR)**, del cirujano.
> La marca de la **consulta (Leblon)** vive en [`../leblon/`](../leblon/). No mezclar logos ni paletas
> sin haber definido antes cómo conviven — ver la nota de paleta en el README de Leblon.

Marca personal del cirujano plástico. **Estos activos mandan por sobre cualquier referencia estética externa** (Farm Rio, Zara Home u otra). Las referencias inspiran el tono, la fotografía y la energía; los colores y el logo son fijos.

## Logo

Monograma **JR** en trazo caligráfico manuscrito, seguido de una barra vertical divisoria y el bloque de texto:

- Línea 1: `Joaquín Ramírez Sneberger` — sans-serif humanista, peso regular
- Línea 2: `CIRUJANO PLÁSTICO` — sans-serif en versalitas, tracking amplio (~0.25em)

La barra divisoria siempre va en el **color complementario** al del monograma: si el monograma es verde, la barra es dorada; si el monograma es blanco, la barra es verde o dorada.

### Variantes disponibles (5)

| # | Fondo | Monograma y texto | Barra divisoria | Uso recomendado |
|---|---|---|---|---|
| 1 | Dorado arena | Blanco | Verde salvia | Piezas cálidas, papelería, redes |
| 2 | Blanco | Monograma verde salvia · texto gris | Dorado | **Versión principal** — documentos, sitio web, membretes |
| 3 | Verde salvia | Blanco | Dorado | Piezas de color pleno, portadas |
| 4 | Blanco | Todo blanco | Blanco | Marca de agua, relieve, estampado en seco |
| 5 | Negro | Blanco | Verde salvia | Fondos oscuros, video, fotografía |

### Archivos

Los archivos originales van en [`logos/`](logos/). Nomenclatura sugerida:

```
logos/jr-01-fondo-dorado.png
logos/jr-02-fondo-blanco.png      ← versión principal
logos/jr-03-fondo-verde.png
logos/jr-04-blanco-sobre-blanco.png
logos/jr-05-fondo-negro.png
```

Si tienes los originales vectoriales (`.svg`, `.ai`, `.eps`), guárdalos también — son los que sirven para impresión y para escalar sin pérdida.

## Paleta

> Los valores hex están **muestreados visualmente** de las imágenes entregadas, no extraídos del archivo de marca original. Antes de usarlos en imprenta, confírmalos contra el manual de marca o el archivo vectorial.

| Color | Hex aprox. | Rol |
|---|---|---|
| Verde salvia | `#86BE9C` | Color primario de marca |
| Dorado arena | `#CBB984` | Color secundario / acento |
| Gris texto | `#58595B` | Tipografía sobre fondos claros |
| Blanco | `#FFFFFF` | Fondo principal y logo invertido |
| Negro | `#000000` | Fondo oscuro |

### Contraste (accesibilidad)

- El **verde salvia y el dorado son colores claros**: no sirven como color de texto sobre fondo blanco. Úsalos como fondo pleno (con texto gris oscuro o blanco encima), como acentos gráficos, o como fondo de botones.
- Para texto de cuerpo sobre fondo claro, usa el gris `#58595B` o un tono más oscuro.
- Si necesitas una versión del verde apta para texto, oscurécelo (aprox. `#3F7256`) en vez de usar el tono del logo.

## Tipografía

El logo usa una sans-serif humanista de peso ligero con versalitas espaciadas. Para materiales que acompañen la marca, mantén ese registro: sans-serif limpia, jerarquía por tamaño más que por peso, y tracking amplio en etiquetas y versalitas.

## Reglas de uso

1. **No recolorear el logo.** Usa una de las 5 variantes existentes según el fondo.
2. **Aire alrededor:** deja un margen libre equivalente a la altura del monograma JR por cada lado.
3. **Tamaño mínimo:** que `CIRUJANO PLÁSTICO` siga siendo legible; bajo eso, usa solo el monograma JR.
4. **No deformar, rotar, agregar sombras, degradados ni contornos.**
5. **Sobre fotografía:** usa la variante blanca (#5) y solo sobre zonas de la imagen con suficiente contraste.

## Relación con las referencias estéticas del agente de marketing

La dirección de arte definida en [`../.claude/agents/jefe-marketing-cirugia-plastica.md`](../.claude/agents/jefe-marketing-cirugia-plastica.md) toma a FARM Rio como referencia principal. Eso **no** significa usar la paleta de FARM Rio (cobalto, coral, lima): esa paleta choca con el logo.

La síntesis correcta es:

- **Paleta** → verde salvia + dorado + gris + blanco (esta marca, siempre).
- **De FARM Rio se toma** → la energía: luz natural, motivos botánicos, diversidad real de cuerpos y etnias, copy cálida y cercana, alegría sin solemnidad hospitalaria.

El verde salvia ya es un verde botánico: los motivos de hoja y flor funcionan naturalmente en el color de la marca, sin necesidad de importar colores ajenos.
