# 📊 Aroma Center · Dashboard Operacional

Dashboard interactivo para visualizar el historial de operaciones de aromatización: instalaciones y retiros de equipos desde noviembre 2016 hasta mayo 2026.

🔗 **[Ver en Vivo](https://parcuatro-dashboard.vercel.app)**

---

## ✨ Paneles

- **Vista General** — KPIs históricos + resumen 2026 YTD + evolución anual + flota acumulada
- **Detalle Mensual** — Tendencia mes a mes (Ene 2025 – May 2026) con cards por mes
- **Vendedores** — Neto de flota por vendedor, instalaciones vs retiros, y desglose por modelo de equipo
- **Clientes & Comunas** — Top 10 clientes, top 10 comunas, duración promedio de clientes, top 8 modelos
- **Fragancias** — Top 20 fragancias en uso por clientes activos, agrupadas por familia olfativa

---

## 📈 Datos actuales

| Métrica | Valor |
|---|---|
| Período | 16 nov 2016 – may 2026 |
| Instalaciones | 16.400 equipos |
| Retiros | 13.775 equipos |
| Flota inicial (nov 2016) | 4.283 equipos |
| Flota estimada activa | **6.908 equipos** |
| Clientes activos | 1.778 |
| Fragancias en uso | 317 |
| Duración promedio cliente | 39,3 meses |

### Criterios de procesamiento

- **Fecha de corte:** solo desde el 16/11/2016
- **Reemplazos:** excluidos de todos los cálculos
- **Servicios de música excluidos:** RB, Map, Nadcom, Cubo, Parlantes, Streaming, Amplificadores, DMX, etc.
- **Dispensadores de alcohol excluidos**
- **Tcell:** incluido como equipo de aromatización
- **C400:** agrupa las variantes C400, C400p y C400c
- **Cantidades:** se usa la columna `Cantidad` (no conteo de filas) para reflejar guías con múltiples equipos

### Modelos de equipos incluidos (top 12)

| Modelo | Instalaciones |
|---|---|
| AQ270 | 4.054 |
| AQ550 | 2.594 |
| AQ570 | 2.439 |
| C400 (agrupa C400, C400p, C400c) | 1.821 |
| DRACO | 1.365 |
| C800 | 1.161 |
| C1000 | 1.022 |
| E1000 | 587 |
| C300 | 391 |
| C700 | 236 |
| SR1000 | 193 |
| TCELL | 117 |

### Vendedores — Neto de flota

| Vendedor | Instalaciones | Retiros | Neto |
|---|---|---|---|
| Pardo | 3.929 | 2.231 | +1.698 |
| Cristobal | 4.192 | 3.276 | +916 |
| Andres | 5.496 | 4.892 | +604 |
| Sofia | 1.685 | 1.505 | +180 |
| Ana | 531 | 384 | +147 |
| Sebastian | 285 | 401 | -116 |

---

## 🛠 Tecnologías

- HTML5 + CSS3 (glassmorphism, CSS Grid, animaciones)
- [Chart.js 4.4](https://www.chartjs.org/) — gráficos interactivos
- [Inter](https://fonts.google.com/specimen/Inter) — tipografía
- Paleta de colores basada en identidad visual de **Aroma Center**
- Sin frameworks ni dependencias de build — archivo único `index.html`

## 🚀 Deploy

El proyecto se despliega en **Vercel** con `vercel --prod` desde el directorio del proyecto.

```bash
# Clonar
git clone https://github.com/cpardo1973/parcuatro-dashboard.git
cd parcuatro-dashboard

# Abrir localmente
open index.html

# Deploy
vercel --prod
```

> **Nota:** Los archivos `.xlsx` con datos fuente están excluidos del repositorio por privacidad. Los datos están procesados y embebidos directamente en el HTML.

## 📁 Estructura

```
parcuatro-dashboard/
├── index.html    # Dashboard completo (HTML + CSS + JS embebido)
├── README.md
└── .gitignore
```

## 📌 Historial de versiones

| Versión | Fecha | Descripción |
|---|---|---|
| v1.0.0 | 2026-05-18 | Primera versión — historial 2014–2026, 4 paneles |
| v2.0.0 | 2026-05-19 | Rediseño completo — paleta Aroma Center, logo, filtro nov 2016, sin reemplazos |
| v2.1.0 | 2026-05-19 | Panel Vendedores con neto de flota y desglose por equipo |
| v2.2.0 | 2026-05-19 | Panel Fragancias — top 20 en uso por clientes activos |
| v2.3.0 | 2026-05-19 | Corrección crítica: usa SUM(Cantidad) en lugar de conteo de filas |
| v2.4.0 | 2026-05-19 | Exclusión de servicios de música y dispensadores de alcohol del conteo de equipos |

---

*Desarrollado con Claude Code · Aroma Center*
