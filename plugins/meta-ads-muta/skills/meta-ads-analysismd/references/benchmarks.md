# Benchmarks y semáforos por tipo de campaña

> Estas tablas son la ÚNICA fuente de verdad para los umbrales 🔴/🟡/🟢. No usar benchmarks generales ni promedios de la industria. Si la métrica no aparece en la tabla, marcar con "—" y no inventar umbral.

---

## Tabla de estandarización de métricas

| Métrica cruda (API / export) | Nombre estandarizado |
|---|---|
| impressions | Impresiones |
| spend | Inversión |
| clicks | Clicks (all) |
| actions_link_click / outbound_clicks | Link Clicks / Clics salientes |
| ctr | CTR (all) |
| unique_ctr | CTR único |
| cpc | CPC (all) |
| cpm | CPM |
| frequency | Frecuencia |
| reach | Alcance |
| actions_purchase | Compras |
| action_values_purchase | Valor de compras |
| website_purchase_roas / purchase_roas | ROAS |
| actions_add_to_cart | Add to Cart |
| actions_initiate_checkout | Initiate Checkout |
| actions_view_content | Ver contenido |
| actions_landing_page_view | Visitas a página de destino |
| actions_lead | Leads |
| actions_messaging_conversation_started | Conversaciones iniciadas |
| video_p25 / video_p50 / video_p75 / video_p100 | Retención de video % |
| video_plays / video_avg_time_watched_actions | Reproducciones / Tiempo promedio |
| quality_ranking / engagement_rate_ranking / conversion_rate_ranking | Diagnósticos de relevancia |

---

## Ventas

**Embudo completo:**
```
Impresiones → Clics salientes → Visitas p.d. → Ver contenido → [Carrito] → Checkout → Compra
```
El paso con el % más bajo es donde se pierde más audiencia → ahí está la oportunidad principal.

| Métrica | Semáforo | Qué señala si está mal |
|---|---|---|
| ROAS | Objetivo del usuario | Rentabilidad general |
| % Compras / Pagos iniciados | 🔴 <10% / 🟡 10-30% / 🟢 >30% | Fricción en el proceso de pago |
| % Checkout / Carritos | 🔴 <30% / 🟡 30-50% / 🟢 >50% | Abandono de carrito |
| % Carritos / Ver contenido | 🔴 <10% / 🟡 10-20% / 🟢 >20% | Producto poco atractivo |
| % Ver contenido / Visitas p.d. | 🔴 <60% / 🟡 60-100% / 🟢 >100% | Landing no convierte |
| % Visitas p.d. / Clics salientes | 🔴 <50% / 🟡 50-70% / 🟢 >70% | Página lenta o mala UX |
| CTR saliente | 🔴 <1% / 🟡 1-2% / 🟢 >2% | Creativo débil |
| % Reprod. 3s / Impresiones | 🔴 <20% / 🟡 20-30% / 🟢 >30% | Hook no engancha |
| Tiempo promedio reproducción | 🔴 <3s / 🟡 3-6s / 🟢 >6s | Contenido no retiene |
| Frecuencia | 🟢 <3 / 🟡 3-5 / 🔴 >5 | Fatiga de audiencia |
| Diagnósticos de relevancia | 🟢 ABOVE_AVERAGE / 🔴 BELOW_AVERAGE | Calidad en subasta |

**Accionables por problema:**

| Problema | Acción |
|---|---|
| ROAS < 80% del objetivo | Auditar embudo urgente; reducir presupuesto hasta corregir el cuello de botella |
| ROAS 80-100% del objetivo | Optimizar el paso del embudo con % más bajo — no pausar |
| ROAS ≥ objetivo | Escalar presupuesto (20% cada 3 días) |
| % Compras/Pagos <30% | Simplificar checkout, reducir campos, agregar métodos de pago |
| % Checkout/Carritos <30% | Mejorar página de carrito, agregar urgencia o incentivo |
| % Ver contenido/Visitas <100% | Mejorar propuesta de valor en landing |
| % Visitas/Clics <70% | Revisar velocidad de carga y UX |
| CTR saliente <2% | Testear nuevos creativos (gancho diferente, oferta más clara) |
| % Video 3s <30% | Cambiar los primeros 3 segundos del video |
| Tiempo video <6s | Acortar o mejorar el gancho inicial |
| Frecuencia >5 | Ampliar audiencia o rotar creativos |

---

## Interacción / Mensajes

| Métrica | Semáforo | Qué señala si está mal |
|---|---|---|
| Costo por conversación | Objetivo del usuario | Eficiencia general |
| Tasa conversación (conv. / clics únicos) | 🔴 <30% / 🟡 30-50% / 🟢 >50% | El ad atrae clics pero no convierte a mensajes |
| CTR único | 🔴 <1% / 🟡 1-2% / 🟢 >2% | Creativo no genera interés |
| % Reprod. 3s / Impresiones | 🔴 <20% / 🟡 20-30% / 🟢 >30% | Hook no engancha |
| Tiempo promedio reproducción | 🔴 <3s / 🟡 3-6s / 🟢 >6s | Contenido no retiene |
| Frecuencia | 🟢 <3 / 🟡 3-5 / 🔴 >5 | Fatiga de audiencia |
| Diagnósticos de relevancia | 🟢 ABOVE_AVERAGE / 🔴 BELOW_AVERAGE | Calidad en subasta |

**Accionables:**

| Problema | Acción |
|---|---|
| Tasa conversión <50% | CTA más específico: invitar a chatear directamente |
| CTR único <2% | Mejorar creativo (imagen/video, copy, oferta) |
| % Video 3s <30% | Mejorar gancho primeros 3 segundos |
| Tiempo video <6s | Mejorar guión y edición |
| Frecuencia >5 | Agregar nuevos anuncios / rotar creativos |

---

## Leads — Formulario instantáneo

| Métrica | Semáforo | Qué señala si está mal |
|---|---|---|
| CPL | Objetivo del usuario | Eficiencia general |
| Tasa conversión (leads / clics únicos) | 🔴 <20% / 🟡 20-30% / 🟢 >30% | Formulario no convierte |
| CTR único | 🔴 <1% / 🟡 1-2% / 🟢 >2% | Creativo no genera interés |
| % Reprod. 3s / Impresiones | 🔴 <20% / 🟡 20-30% / 🟢 >30% | Hook no engancha |
| Tiempo promedio reproducción | 🔴 <3s / 🟡 3-6s / 🟢 >6s | Contenido no retiene |
| Frecuencia | 🟢 <3 / 🟡 3-5 / 🔴 >5 | Fatiga de audiencia |
| Diagnósticos de relevancia | 🟢 ABOVE_AVERAGE / 🔴 BELOW_AVERAGE | Calidad en subasta |

**Accionables:**

| Problema | Acción |
|---|---|
| Tasa conversión <30% | Simplificar formulario (menos campos, mejor oferta) |
| CTR único <2% | Mejorar creativo |
| % Video 3s <30% | Mejorar gancho primeros 3 segundos |
| Frecuencia >5 | Rotar creativos |

---

## Leads — Sitio web

**Embudo:**
```
Impresiones → Clics salientes → Visitas p.d. → Lead
```

| Métrica | Semáforo | Qué señala si está mal |
|---|---|---|
| CPL | Objetivo del usuario | Eficiencia general |
| Tasa conversión (leads / visitas p.d.) | 🔴 <10% / 🟡 10-20% / 🟢 >20% | Landing no convierte |
| % Visitas p.d. / Clics salientes | 🔴 <50% / 🟡 50-70% / 🟢 >70% | Página lenta o mala UX |
| CTR saliente | 🔴 <1% / 🟡 1-2% / 🟢 >2% | Creativo débil |
| % Reprod. 3s / Impresiones | 🔴 <20% / 🟡 20-30% / 🟢 >30% | Hook no engancha |
| Tiempo promedio reproducción | 🔴 <3s / 🟡 3-6s / 🟢 >6s | Contenido no retiene |
| Frecuencia | 🟢 <3 / 🟡 3-5 / 🔴 >5 | Fatiga de audiencia |
| Diagnósticos de relevancia | 🟢 ABOVE_AVERAGE / 🔴 BELOW_AVERAGE | Calidad en subasta |

**Accionables:**

| Problema | Acción |
|---|---|
| Tasa conversión <20% | Optimizar landing: formulario simple, CTA claro, mejor oferta |
| % Visitas/Clics <70% | Reducir tiempo de carga de la página |
| CTR saliente <2% | Mejorar creativo |
| % Video 3s <30% | Mejorar gancho primeros 3 segundos |
| Frecuencia >5 | Rotar creativos |

---

## Reconocimiento / Tiendas físicas

| Métrica | Semáforo | Qué señala si está mal |
|---|---|---|
| % Reprod. 3s / Impresiones | 🔴 <20% / 🟡 20-30% / 🟢 >30% | La audiencia no se detiene |
| Tiempo promedio reproducción | 🔴 <3s / 🟡 3-6s / 🟢 >6s | El mensaje no llega |
| Frecuencia | 🟢 2-4 / 🟡 4-5 / 🔴 >5 | Audiencia saturada |
| CTR único | 🔴 <1% / 🟡 1-2% / 🟢 >2% | Creativo no genera interés |
| Diagnósticos de relevancia | 🟢 ABOVE_AVERAGE / 🔴 BELOW_AVERAGE | Calidad en subasta |

**Accionables:**

| Problema | Acción |
|---|---|
| % Video 3s <30% | Mejorar gancho primeros 3 segundos |
| Tiempo video <6s | Mejorar guión y edición |
| Frecuencia >5 | Rotar creativos |
| CPM elevado | Usar públicos más grandes, mejorar calidad del ad |

---

## Creativos — fatiga y retención de video

**Señales de fatiga:**
- CTR descendente >15% en 7 días consecutivos + frecuencia alta (>3-4)
- CPM subiendo sin cambios en audiencia
- Diagnósticos de relevancia cayendo a BELOW_AVERAGE

**Retención de video (si hay datos p25/p50/p75/p100):**

| Punto | Benchmark | Señal |
|---|---|---|
| Hook rate (3s / reproducciones) | 🔴 <20% / 🟡 20-30% / 🟢 >30% | Primeros segundos no enganchan |
| Hold rate (p25) | 🔴 <40% / 🟡 40-60% / 🟢 >60% | Video pierde audiencia rápido |
| Completion rate (p100) | 🔴 <10% / 🟡 10-25% / 🟢 >25% | Video no se termina |

---

## Audiencias y placements

**Saturación:**
- Frecuencia >5 + CTR cayendo → audiencia agotada → ampliar o rotar
- Alcance estancado con presupuesto estable → audiencia demasiado pequeña

**Concentración de resultados:**
Si el 80% de los resultados vienen de un solo adset o anuncio, la campaña es frágil. Señalarlo como riesgo.

**Análisis de ubicaciones:**
Solo recomendar excluir si se cumplen las tres condiciones:
1. CPA promedio consistentemente >40% peor que el promedio de la campaña
2. La tendencia marginal también es peor (no solo el promedio)
3. Volumen suficiente (>100 impresiones por ubicación)

---

## Fluctuaciones: normal vs preocupante

| Normal (no alarmar) | Preocupante (investigar) |
|---|---|
| Variación CPA día a día dentro de 20-30% | Aumento súbito >50% por varios días |
| Diferencias semana vs fin de semana | Delivery cayendo a casi cero |
| Cambios graduales a lo largo de semanas | CVR bajando mientras spend sube |
| Variación durante learning phase | Degradación sin cambios hechos |
