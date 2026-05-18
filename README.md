# 📊 Parcuatro · Dashboard Operacional

Dashboard interactivo para visualizar el historial de operaciones de aromatización: instalaciones, retiros y reemplazos de equipos desde 2014 hasta 2026.

🔗 **[Ver Demo en Vivo](https://parcuatro-dashboard.vercel.app)**

---

## ✨ Funcionalidades

- **Vista General** — KPIs históricos totales + resumen del año en curso (2026 YTD)
- **Detalle Mensual** — Tendencia mes a mes (2025–2026) con cards por mes
- **Clientes & Equipos** — Top 10 clientes, modelos más usados y distribución por comuna
- **Crecimiento** — Crecimiento neto de flota, flota acumulada estimada y balance anual

## 📈 Datos

| Métrica | Total Histórico |
|---|---|
| Instalaciones | 14.062 |
| Retiros | 11.356 |
| Reemplazos | 5.763 |
| Movimientos totales | 31.194 |
| Período | 2014 – 2026 |
| Flota estimada activa | ~2.706 equipos |

## 🛠 Tecnologías

- HTML5 + CSS3 (Glassmorphism, CSS Grid, animaciones)
- [Chart.js 4.4](https://www.chartjs.org/) — gráficos interactivos
- [Inter](https://fonts.google.com/specimen/Inter) — tipografía
- Sin frameworks ni dependencias de build — archivo único `dashboard.html`

## 🚀 Deploy

El proyecto se despliega automáticamente en **Vercel** desde la rama `main`.

```bash
# Clonar
git clone https://github.com/cpardo1973/parcuatro-dashboard.git
cd parcuatro-dashboard

# Abrir localmente
open dashboard.html
```

> **Nota:** Los archivos `.xlsx` con datos fuente están excluidos del repositorio por privacidad. El dashboard contiene los datos ya procesados embebidos en el HTML.

## 📁 Estructura

```
parcuatro-dashboard/
├── dashboard.html     # Dashboard completo (HTML + CSS + JS embebido)
├── .gitignore
└── README.md
```

## 📌 Versiones

| Versión | Fecha | Descripción |
|---|---|---|
| v1.0.0 | 2026-05-18 | Primera versión — historial 2014–2026, 4 paneles |

---

*Desarrollado con Claude Code · Parcuatro Aromatización*
