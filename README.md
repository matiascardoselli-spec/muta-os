# muta-os

Marketplace privado de skills de Claude Code de Muta Digital, para equipo y amigos.

## v1

- **meta-ads-muta** — análisis técnico multinivel de campañas de Meta Ads (ROAS, CPL, CPM, fatiga, embudo).

## Instalar

Este repo es **privado**: necesitás acceso (colaborador invitado) antes de poder agregarlo.

**Claude Code (terminal):**
```
/plugin marketplace add matiascardoselli-spec/muta-os
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
