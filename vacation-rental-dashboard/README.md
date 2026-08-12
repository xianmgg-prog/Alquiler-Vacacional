# 🏠 Vacation Rental Dashboard — Multi-Property Manager

Dashboard de gestión para controlar 7 pisos alquilados en **Booking.com** y **Airbnb**.  
Fase actual: **DEMO / Prueba de Concepto** con datos simulados (Mock Data).

---

## 🚀 Stack Tecnológico

| Capa | Tecnología |
|------|-----------|
| Framework | Next.js 14 (App Router) |
| Estilos | Tailwind CSS |
| Gráficos | Chart.js + react-chartjs-2 |
| Íconos | Lucide React |
| Datos | JSON local (mock) |

---

## 📦 Instalación

```bash
# Clonar o crear el proyecto
npx create-next-app@latest vacation-rental-dashboard
cd vacation-rental-dashboard

# Instalar dependencias adicionales
npm install chart.js react-chartjs-2 lucide-react

# Iniciar servidor de desarrollo
npm run dev
```

Abre [http://localhost:3000](http://localhost:3000) para ver el dashboard.

---

## 🏗️ Arquitectura del Proyecto

```
src/
├── app/           # Páginas y layout principal (Next.js App Router)
├── components/    # Componentes React reutilizables
└── data/          # Datos mock — fácilmente reemplazables por APIs reales
```

> **Nota para desarrolladores:** El archivo `src/data/mockData.js` centraliza toda la información.  
> Para migrar a APIs reales de Booking/Airbnb, solo necesitas reemplazar las funciones exportadas en ese archivo por llamadas `fetch()` a tus endpoints.

---

## 📊 Vistas Implementadas

| Bloque | Descripción |
|--------|-------------|
| **A. KPIs** | Métricas globales: Ingresos MTD, Ocupación, ADR, Beneficio Neto |
| **B. Rendimiento** | Tabla interactiva por piso con filtros |
| **C. Operativa** | Check-ins/check-outs del día + calendario de 7 días |
| **D. Calidad** | Puntuaciones y reseñas por plataforma |

---

## 🔄 Roadmap a Producción

1. [ ] Integrar API de Airbnb (Host API)
2. [ ] Integrar API de Booking.com (Content API / Connectivity)
3. [ ] Autenticación (NextAuth.js)
4. [ ] Base de datos (PostgreSQL + Prisma)
5. [ ] Notificaciones push para limpieza

---

## 📝 Licencia

Proyecto privado — Uso interno.
