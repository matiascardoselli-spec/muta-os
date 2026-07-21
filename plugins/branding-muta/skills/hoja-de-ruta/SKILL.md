---
name: hoja-de-ruta
description: Convierte una reunión estratégica con un cliente o prospecto en una hoja de ruta entregable, que destila en limpio el criterio que se le dio en esa reunión, ordenado para ejecutar. Activar cuando alguien de Muta pida "armá la hoja de ruta de X", "destilá la reunión de X en un documento para el cliente", "pasale en limpio la estrategia que le di a X", "el documento ejecutable de la reunión con X". REQUIERE una reunión estratégica real (transcripción de Fathom o pegada): sin reunión no hay hoja de ruta, porque el documento no inventa consejos, ordena los que ya se dieron. NO es para pendientes internos del equipo o Asana (eso es reunion-pendientes), ni para investigar la categoría de un cliente (eso es informe-de-mercado), ni para PRDs de sitios web (eso es prd-web-primera-reunion).
---

# Hoja de Ruta

## Qué es

El destilado limpio de una reunión estratégica, convertido en un documento HTML que el cliente puede seguir y ejecutar. Toma una conversación larga, con idas y vueltas, y la ordena en decisiones, fases y advertencias, sin perder el criterio ni el porqué de cada cosa.

Se usa típicamente como cierre de una etapa de trabajo (por ejemplo, junto con la entrega de un manual de marca: "sé que quedaron con mil ideas de la reunión, acá está todo ordenado") o como pieza de valor para un prospecto después de una reunión de asesoría.

**A diferencia del informe de mercado, esta pieza SÍ es prescriptiva, y está bien que lo sea.** La diferencia es de dónde sale la autoridad: la hoja de ruta no inventa recomendaciones, **destila el consejo que el cliente ya recibió en la reunión**. Quien firmó ese criterio es la persona que dio la reunión; el documento solo lo ordena y lo desarrolla. Por eso la regla número uno:

**Todo lo afirmado tiene que ser rastreable a la reunión.** Se puede desarrollar, dar contexto, completar el porqué de algo que en la charla quedó a medias. No se puede agregar consejo nuevo que no se dio: si al redactar aparece algo que "faltó decir", se le consulta a quien dio la reunión antes de incluirlo, nunca se mete en silencio.

## Proceso

1. **Obtener la reunión.** Buscar la transcripción en Fathom (o usar la que peguen). Leerla completa antes de escribir: el criterio suele estar disperso, repetido y mezclado con charla.
2. **Extraer el esqueleto:** la lógica de fondo (la premisa única de la que cuelga todo lo demás, dicha o implícita en la reunión), las decisiones/consejos principales (típicamente entre 4 y 8), el orden o fases si se estableció uno, y los "no hagas esto" que se marcaron.
3. **Construir el documento en Markdown** (trabajo interno), auditarlo contra las reglas, y recién con el contenido cerrado pasarlo a HTML. Nunca diseñar y corregir después.

## Estructura del documento

1. **Apertura breve** (2-3 párrafos): qué es este documento y **la lógica de fondo en una sola frase destacada** (la premisa de la que cuelga todo). Ejemplo del caso que originó esta skill: "el producto es fácil de copiar, la marca no; la carrera es construir marca antes de que aparezca el segundo".
2. **"Las N decisiones que ordenan todo"**: la lista numerada de las decisiones/consejos principales, cada una en dos líneas. Es el resumen ejecutivo: si solo leen esto, ya tienen la reunión.
3. **Una sección desarrollada por decisión**: el consejo con su porqué completo, tal como se argumentó en la reunión, con los ejemplos que se usaron (sanitizados, ver reglas). Si la reunión estableció un orden de ejecución, una sección de **fases** con la regla explícita de por qué no se saltean.
4. **"Dónde NO ponerse a gastar"** (o el equivalente que haya surgido): los errores marcados en la reunión, cada uno con el mecanismo concreto por el que la plata o el esfuerzo se pierde. Es de las secciones más valiosas: el cliente recuerda mejor lo que no tiene que hacer.
5. **Cierre: la foto completa.** Un resumen en una idea de por qué todo el documento apunta al mismo lado, terminando en tono de aliento realista (qué tienen a favor, qué falta).

**Cada sección cierra con un takeaway de una línea** prefijado con "→": la instrucción concreta que queda de esa sección.

## Reglas de contenido

- **Rastreabilidad total:** nada que no se haya dicho o que no se desprenda directamente de lo dicho en la reunión. El documento habla con la voz y el criterio de quien dio la reunión.
- **Segunda persona, dirigida al cliente** ("no salgan al precio de equilibrio", "pregunten al laboratorio"). Directo, sin corporativismo. Los takeaways en imperativo.
- **Sanitización de ejemplos:** los casos de otros clientes que se contaron en la reunión se anonimizan ("una marca con la que trabajamos", "un producto altamente googleable"), nunca con nombre ni con cifras que los identifiquen. Los montos internos de Muta no entran. Los datos del propio cliente sí (son suyos).
- **Sin fechas ni cronograma de gestión.** El orden va por fases y dependencias ("esto habilita aquello"), no por calendario.
- **El criterio se explica, no se decreta.** Cada consejo lleva su porqué, con la lógica que se usó en la reunión. Un cliente que entiende el porqué ejecuta mejor y discute menos.
- Sin guión largo (—). Ortografía y tildes revisadas. Sin frases de relleno de agencia.

## Reglas del entregable

- **HTML con estética Muta**: Montserrat, negro `#232323`, amarillo `#FAD70B` (naranja/azul solo en detalles). Mismo sistema visual que el informe de mercado: header negro con título amarillo, tarjetas numeradas para las decisiones, takeaways destacados. Si existe un manual de marca de Muta en el sistema, leerlo antes de diseñar.
- Si el cliente necesita PDF: conversión única al cierre (`chrome --headless --print-to-pdf --no-pdf-header-footer`), con el contenido ya validado.
- **Ubicación**: la carpeta del cliente o prospecto en el sistema de archivos del usuario. **Versionar** (v1, v2), nunca sobrescribir.
- **El mensaje de entrega lo escribe una persona**, nunca la skill. El documento no se envía solo.

## Verificación antes de cerrar

- Releer contra la transcripción: ¿hay alguna afirmación no rastreable a la reunión? Se saca o se consulta.
- Grep de sanitización: nombres de otros clientes, montos internos.
- Sin guión largo; tildes.
- El HTML renderiza (header, tarjetas, takeaways).

## Contrato de entrada/salida

**Inputs:** cliente/prospecto · reunión (link o ID de Fathom, o transcripción pegada) · contexto de entrega (cierre de etapa, post-asesoría, acompaña un manual).

**Outputs:** `hoja-de-ruta-<slug>-vN.html` (+ su `.md` de trabajo) · resumen para quien lo pidió con: rutas, decisiones extraídas, y flags (afirmaciones dudosas que conviene revisar contra la reunión antes de entregar).

**El documento siempre pasa por revisión humana antes de llegar al cliente.**
