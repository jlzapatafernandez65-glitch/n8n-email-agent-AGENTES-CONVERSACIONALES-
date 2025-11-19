# N8N Email Agent - Sistema de Automatización Inteligente

Sistema avanzado de automatización de correos electrónicos con IA usando n8n, Evolution API y OpenAI. Procesa emails de forma inteligente, mantiene conversaciones contextuales con clientes, guía a usuarios hacia la agenda de citas mediante flujos conversacionales naturales, recopila y valida datos relevantes del prospecto, y registra automáticamente nuevos leads en el CRM.

## 🚀 Características

- **Procesamiento automático de emails** - Monitoreo IMAP en tiempo real
- **Respuestas inteligentes con IA** - OpenAI/Claude para conversaciones naturales
- **Integración WhatsApp** - Notificaciones vía Evolution API
- **Gestión de conversaciones** - Sistema de memoria y contexto
- **Registro automático de leads** - Captura de datos y almacenamiento en CRM
- **Agendamiento inteligente** - Guía conversacional hacia reservas

## 🛠️ Stack Tecnológico

- **n8n** - Plataforma de automatización
- **OpenAI / Anthropic** - Modelos de lenguaje
- **Evolution API** - Integración WhatsApp
- **Docker** - Contenedorización
- **Redis** - Sistema de caché
- **Qdrant** - Base de datos vectorial

## 📋 Requisitos

- Docker 20.10+
- Docker Compose 2.0+
- Node.js 18+
- Cuenta OpenAI o Anthropic
- VPS con mínimo 2GB RAM

## ⚡ Instalación Rápida
```bash
# Clonar repositorio
git clone https://github.com/jlzapatafernandez65-glitch/n8n-email-agent-AGENTES-CONVERSACIONALES-.git
cd n8n-email-agent-AGENTES-CONVERSACIONALES-

# Configurar variables de entorno
cp .env.example .env
nano .env

# Levantar servicios
docker-compose up -d

# Acceder a n8n
# http://localhost:5678
```

Ver [QUICKSTART.md](QUICKSTART.md.pdf) para instrucciones detalladas.

## 📁 Estructura del Proyecto
```
├── docs/
│   ├── INSTALLATION.md.pdf    # Guía de instalación completa
│   └── TECHNICAL.md.pdf       # Documentación técnica
├── workflow/
│   └── AI-AGENT-CORREO.json  # Workflow principal de n8n
├── screenshots/               # Capturas de ejemplo
├── .env.example              # Variables de entorno de ejemplo
├── .gitignore
└── LICENSE
```

## 🔧 Configuración

1. **Variables de Entorno**: Edita `.env` con tus credenciales
2. **Importar Workflow**: Importa `workflow/AI-AGENT-CORREO.json` en n8n
3. **Configurar Credenciales**: OpenAI, Evolution API, IMAP
4. **Activar Workflow**: Activa el flujo principal

## 📚 Documentación

- [Instalación Completa](docs/INSTALLATION.md.pdf)
- [Documentación Técnica](docs/TECHNICAL.md.pdf)
- [Guía Rápida](QUICKSTART.md.pdf)

## 🎯 Casos de Uso

- Automatización de respuestas de correo electrónico
- Calificación automática de leads
- Agendamiento de citas sin intervención humana
- Notificaciones instantáneas por WhatsApp
- CRM conversacional automatizado

## 📸 Screenshots

![Calendar Management](screenshots/calendar-management)
![Gmail Integration](screenshots/gmail-integration)
![Workflow Overview](screenshots/workflow-overview.png)

## 📝 Licencia

MIT License - ver [LICENSE](LICENSE)

## 👤 Autor

**José Luis Zapata**
- Website: [joseluiszapataia.com](https://joseluiszapataia.com)
- GitHub: [@jlzapatafernandez65-glitch](https://github.com/jlzapatafernandez65-glitch)

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Por favor, abre un issue primero para discutir cambios importantes.

## ⭐ Soporte

Si este proyecto te resulta útil, considera darle una estrella ⭐
