# Los Robles

> Sistema de gestión de reservas para club de pádel.

![React](https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat&logo=supabase&logoColor=white)
![Status](https://img.shields.io/badge/status-en%20desarrollo-orange)

---

## ¿Qué es esto?

Los Robles es una aplicación web para gestionar las reservas diarias de un club de pádel. Reemplaza el registro en papel con una interfaz digital que permite ver, crear y administrar turnos por día, cancha y horario — desde cualquier dispositivo.

---

## Características

- 📅 **Calendario mensual** — visualización de días con y sin reservas de un vistazo
- 🏟️ **3 canchas** — Cancha 1 (sin techo), Cancha 2 y Cancha 3 (techadas)
- ⏱️ **Horario inicio / fin** — registro exacto del turno
- 💰 **Gestión de cobros** — seña, insumos, total y método de pago (efectivo, transferencia o combinado)
- 🔄 **Estados automáticos** — Reservado → En curso → Finalizado
- 📱 **Responsive** — funciona en celular, tablet y computadora

---

## Stack tecnológico

| Capa | Tecnología |
|------|-----------|
| Frontend | React |
| Base de datos | Supabase (PostgreSQL) |
| Auth | Supabase Auth |
| Deploy | Vercel |

---

## Instalación y uso local

### Requisitos previos

- Node.js 18+
- Una cuenta en [Supabase](https://supabase.com)

### Pasos

```bash
# 1. Clonar el repositorio
git clone https://github.com/tu-usuario/los-robles-gestor.git
cd los-robles-gestor

# 2. Instalar dependencias
npm install

# 3. Configurar variables de entorno
cp .env.example .env
```

Completar el archivo `.env` con las credenciales de tu proyecto en Supabase:

```env
VITE_SUPABASE_URL=tu_url_de_supabase
VITE_SUPABASE_ANON_KEY=tu_anon_key
```

```bash
# 4. Iniciar en modo desarrollo
npm run dev
```

---

## Estructura del proyecto

```
los-robles-app/
├── src/
│   ├── components/       # Componentes reutilizables
│   ├── pages/            # Vistas principales
│   ├── hooks/            # Custom hooks
│   ├── lib/              # Cliente de Supabase y utilidades
│   └── types/            # Tipos TypeScript
├── .env.example
└── README.md
```

---

## Contexto

Este proyecto nació en el trabajo, de anotar reservas en papel. Con el tiempo se convirtió en una herramienta real usada por el encargado de turno o la dueña del club para registrar todo lo que antes se hacía a mano.

---

## Licencia

Uso privado. No apto para distribución sin autorización.
