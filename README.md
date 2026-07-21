# muta-os

Marketplace de skills de Claude Code de Muta Digital, para equipo y amigos.

## Plugins

- **meta-ads-muta** — análisis técnico multinivel de campañas de Meta Ads (ROAS, CPL, CPM, fatiga, embudo).
- **creacion-contenido** — redacción de contenido: guiones de video corto, fórmulas de copy, carruseles y laboratorio de hooks.
- **metodologia-fv** — investigación de mercado (7 Maletas), psicología del consumidor y matriz de diversificación de ángulos. Basado en la metodología de Felipe Vergara.

Los dos últimos se complementan: `metodologia-fv` define qué decir, `creacion-contenido` lo escribe. Cada skill funciona por separado.

## Instalar

**Claude Code (terminal):**
```
/plugin marketplace add matiascardoselli-spec/muta-os
/plugin install creacion-contenido@muta-os
/plugin install metodologia-fv@muta-os
/plugin install meta-ads-muta@muta-os
```

**App Claude (web/desktop/Cowork):**
Customize → Plugins → Agregar → Agregar marketplace → Add from a repository → pegar la URL de este repo.

## Actualizaciones

El auto-update viene **desactivado por default**. Para activarlo: Customize → Plugins →
Marketplaces → elegir `muta-os` → "Enable auto-update".

- Con auto-update activado: se chequea al iniciar sesión (delay random de hasta 10 min),
  se actualiza en background y pide correr `/reload-plugins`.
- Sin auto-update: correr `/plugin marketplace update muta-os` a mano cuando se avise de un cambio.

## Atribución

`metodologia-fv` implementa la metodología de Felipe Vergara (7 Maletas de Cualquier Compra, matriz de diversificación creativa). Implementación propia de Muta Digital, sin afiliación oficial.
