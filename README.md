# ObsiAgent

ObsiAgent es una plataforma integral para analizar notas personales, crear agentes inteligentes y generar informes adaptados a lo que los usuarios están buscando. Este proyecto aprovecha las tecnologías web modernas y las capacidades de IA para transformar la manera en que los usuarios interactúan y extraen valor de sus bases de conocimiento personales.

## Descripción del Proyecto

ObsiAgent se conecta a tu repositorio de notas personales y aplica técnicas avanzadas de análisis para ayudarte a:

- **Descubrir conexiones** entre tus ideas y notas que podrías haber pasado por alto
- **Generar informes personalizados** basados en temas o consultas específicas
- **Crear agentes autónomos** que pueden interactuar con tu base de conocimiento
- **Extraer ideas clave** de tu conocimiento acumulado

## Stack Tecnológico

### Backend
- **Node.js** - Entorno de ejecución JavaScript para el servidor
- **Express** - Framework web para desarrollo de API
- **GraphQL** - Lenguaje de consulta de API para recuperación flexible de datos
- **TypeScript** - Superset de JavaScript con tipado estático
- **PostgreSQL** - Base de datos relacional primaria para datos estructurados
- **MongoDB** - Base de datos NoSQL para almacenamiento de documentos
- **Sequelize** - ORM para interacción con PostgreSQL
- **Mongoose** - Modelado de objetos para MongoDB
- **AWS S3** - Almacenamiento en la nube para gestión de archivos
- **API de Claude** - Capacidades de IA para comprensión y generación de lenguaje natural

### Frontend
- **React** - Biblioteca de UI para interfaces basadas en componentes
- **TypeScript** - Para desarrollo con tipado seguro
- **Vite** - Herramienta de construcción para desarrollo rápido
- **CSS** - Estilizado y diseño responsivo

### Infraestructura
- **GitHub** - Control de versiones y colaboración
- **Railway** - Servicios en la nube y alojamiento
- **Pipelines CI/CD** - Pruebas y despliegue automatizados

## Arquitectura

ObsiAgent sigue una arquitectura moderna orientada a servicios:

```
ObsiAgent
├── Backend (Node.js, Express, GraphQL)
│   ├── API Gateway (GraphQL)
│   ├── Servicio de Autenticación
│   ├── Motor de Análisis de Notas
│   ├── Sistema de Gestión de Agentes
│   └── Servicio de Generación de Informes
│
├── Bases de Datos
│   └── PostgreSQL (Datos de usuario, relaciones, Docs)
│
├── Almacenamiento
│   └── AWS S3 (Adjuntos, exportaciones)
│
├── Servicios de IA
│   └── Integración con API de Claude
│
└── Frontend (React, TypeScript)
    ├── Panel de Usuario
    ├── Explorador de Notas
    ├── Interfaz de Configuración de Agentes
    └── Diseñador de Informes
```

## Características Principales

- **Análisis Inteligente de Notas**: Identifica automáticamente temas, tópicos y conexiones entre tus notas.
- **Creación de Agentes Personalizados**: Define agentes especializados que pueden responder preguntas o realizar tareas utilizando tu base de conocimiento.
- **Búsqueda Avanzada**: Ve más allá de las palabras clave con capacidades de búsqueda semántica.
- **Visualizaciones Interactivas**: Observa conexiones y relaciones dentro de tu conocimiento en visualizaciones intuitivas.
- **Informes Personalizados**: Genera informes completos sobre temas específicos extraídos de todas tus notas.
- **Sincronización en la Nube**: Almacena y accede a tu base de conocimiento de forma segura desde cualquier lugar.
- **Acceso API**: Integra con otras herramientas y servicios a través de nuestra API GraphQL.

## Primeros Pasos

### Requisitos Previos

- Node.js (v18 o superior)
- PostgreSQL
- MongoDB
- Cuenta AWS (para S3)
- Credenciales de API de Claude

### Instalación

1. Clonar el repositorio
```bash
git clone https://github.com/username/ObsiAgent.git
cd ObsiAgent
```

2. Instalar dependencias del backend
```bash
cd backend
npm install
```

3. Instalar dependencias del frontend
```bash
cd ../frontend
npm install
```

4. Configurar variables de entorno

Crea un archivo `.env` en el directorio backend con las siguientes variables:
```
# Base de datos
DB_HOST=localhost
DB_USER=postgres
DB_PASSWORD=tu_contraseña
DB_NAME=obsiagent

# MongoDB
MONGO_URI=mongodb://localhost:27017/obsiagent

# AWS
AWS_ACCESS_KEY_ID=tu_access_key
AWS_SECRET_ACCESS_KEY=tu_secret_key
AWS_REGION=tu_region
S3_BUCKET=nombre_de_tu_bucket

# API de Claude
CLAUDE_API_KEY=tu_api_key

# Servidor
PORT=3000
NODE_ENV=development
```

5. Iniciar los servidores de desarrollo

Para el backend:
```bash
cd backend
npm run dev
```

Para el frontend:
```bash
cd frontend
npm run dev
```

## Licencia

Este proyecto está licenciado bajo la Licencia MIT - consulta el archivo [LICENSE](LICENSE) para más detalles.
