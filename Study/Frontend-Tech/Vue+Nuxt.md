# Guía Inicial: Vue, Nuxt e Instalación

## ¿Qué es Vue.js?

**Vue.js** es un framework progresivo para construir interfaces de usuario. Está diseñado desde cero para ser adoptado incrementalmente, lo que significa que se puede usar para añadir interactividad a una parte de tu aplicación o para desarrollar Single Page Applications (SPA) completas. Se supone que es simple de aprender lo cual debería de agilizar el proceso

### Características principales

- Reactivo y basado en componentes.
- Integración sencilla con otros proyectos.

## ¿Qué es Nuxt.js?

**Nuxt.js** es un framework construido sobre Vue.js que facilita el desarrollo de aplicaciones universales (renderizadas en el cliente y servidor), SPA, estáticas o incluso híbridas. Automatiza la configuración compleja de Vue para que uno pueda enfocarse en la lógica del negocio.

### Ventajas de usar Nuxt

- Renderizado del lado del servidor (SSR).
- Generación de sitios estáticos (SSG).
- Estructura de carpetas predefinida y eficiente.
- SEO optimizado.
- Modularidad con más de 100 módulos integrables.

## ¿Cómo se integran Vue y Nuxt?

Nuxt extiende Vue y se basa completamente en él. Mientras Vue se enfoca en la interfaz, Nuxt proporciona una estructura completa para construir aplicaciones escalables. Todo proyecto Nuxt es un proyecto Vue, pero estructurado de forma avanzada para funcionalidades como SSR y routing automático.

---

## Instalación de Vue y Nuxt

Muestro la instalación para entornos Windows, Windows Subsystem Linux (WSL), y Linux (distribución de preferencia siendo Fedora 41)

### 1. Instalación en Windows

#### Requisitos

- Node.js
- npm o Yarn

#### Pasos:

```bash
# Instalar Node.js desde https://nodejs.org
# Verificar instalación
node -v
npm -v

# Instalar Vue CLI (opcional si solo se usa Nuxt)
npm install -g @vue/cli

# Crear un nuevo proyecto Nuxt
npx nuxi init nombre-del-proyecto
cd nombre-del-proyecto
npm install

# Ejecutar en desarrollo
npm run dev
```
### 2. Instalación en WSL

#### Pasos

```bash
# Actualizar paquetes
sudo apt update && sudo apt upgrade

# Instalar Node.js y npm
sudo apt install nodejs npm

# Verificar versiones
node -v
npm -v

# Instalar nuxi y crear proyecto
npm install -g nuxi
nuxi init mi-proyecto-nuxt
cd mi-proyecto-nuxt
npm install

# Ejecutar el proyecto
npm run dev
```

Otra forma seria

```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
source ~/.bashrc
nvm install --lts
```

### 3. Instalación en Fedora 41

```bash
# Actualizar paquetes
sudo dnf update

# Habilitar repositorio Node.js (LTS)
sudo dnf module enable nodejs:18
sudo dnf install nodejs

# Verificar instalación
node -v
npm -v

# Instalar nuxi y crear un nuevo proyecto
npm install -g nuxi
nuxi init mi-proyecto-nuxt
cd mi-proyecto-nuxt
npm install

# Ejecutar en modo desarrollo
npm run dev
```