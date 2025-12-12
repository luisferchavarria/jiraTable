# Jira Table

Dashboard de visualización de tickets de Jira con tablas de datos, tableros Kanban y hojas de tiempo semanales.

## 📋 Descripción

Esta aplicación permite visualizar y gestionar tickets de Jira a través de diferentes vistas:
- Tabla de datos interactiva
- Tablero Kanban
- Hoja de tiempo semanal
- Resumen de registros de trabajo

## 🚀 Requisitos Previos

- Node.js (versión 18 o superior)
- npm o yarn
- Cuenta de Jira con acceso a la API

## 🔧 Instalación

1. Clona el repositorio:
```bash
git clone <url-del-repositorio>
cd jiraTable
```

2. Instala las dependencias:
```bash
npm install
```

3. Configura las variables de entorno:

Crea un archivo `.env` en la raíz del proyecto con las siguientes variables:
```env
JIRA_BASE_URL=https://tu-dominio.atlassian.net
JIRA_EMAIL=tu-email@ejemplo.com
JIRA_API_TOKEN=tu-token-api
```

Para obtener tu token de API de Jira:
- Ve a https://id.atlassian.com/manage-profile/security/api-tokens
- Haz clic en "Crear token de API"
- Copia el token generado

## 🏃 Uso

### Modo Desarrollo

Para iniciar el servidor de desarrollo (cliente y servidor):
```bash
npm run dev
```

El cliente estará disponible en: http://localhost:5173
El servidor estará disponible en: http://localhost:3000

### Solo Cliente
```bash
npm run dev:client
```

### Solo Servidor
```bash
npm run dev:server
```

### Compilar para Producción
```bash
npm run build
```

### Iniciar en Producción
```bash
npm start
```

## 🛠️ Tecnologías

- **Frontend**: React + TypeScript + Vite
- **Backend**: Node.js + Express + TypeScript
- **Tabla de Datos**: TanStack React Table
- **Estilos**: CSS personalizado + System.css
- **API**: Jira REST API

## 📁 Estructura del Proyecto

```
jiraTable/
├── src/               # Código fuente del cliente
│   ├── components/    # Componentes React
│   ├── styles/        # Archivos CSS
│   └── types.ts       # Definiciones de tipos TypeScript
├── server/            # Código del servidor Express
├── index.html         # Plantilla HTML principal
└── package.json       # Dependencias y scripts
```

## 📝 Licencia

Este proyecto es de código abierto y está disponible bajo la licencia MIT.
