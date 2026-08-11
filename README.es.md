<p align="center">
  <a href="https://strix.ai/">
    <img src="https://github.com/usestrix/.github/raw/main/imgs/cover.png" alt="Strix Banner" width="100%">
  </a>
</p>

<div align="center">

# Strix

### La herramienta de pentesting (pruebas de seguridad) con IA de código abierto. Hackers de IA autónomos que encuentran y arreglan las vulnerabilidades de tu aplicación.

<br/>


<a href="https://docs.strix.ai"><img src="https://img.shields.io/badge/Docs-docs.strix.ai-2b9246?style=for-the-badge&logo=gitbook&logoColor=white" alt="Docs"></a>
<a href="https://strix.ai"><img src="https://img.shields.io/badge/Website-strix.ai-f0f0f0?style=for-the-badge&logoColor=000000" alt="Website"></a>
[![](https://dcbadge.limes.pink/api/server/strix-ai)](https://discord.gg/strix-ai)

<a href="https://deepwiki.com/usestrix/strix"><img src="https://deepwiki.com/badge.svg" alt="Ask DeepWiki"></a>
<a href="https://github.com/usestrix/strix"><img src="https://img.shields.io/github/stars/usestrix/strix?style=flat-square" alt="GitHub Stars"></a>
<a href="LICENSE"><img src="https://img.shields.io/badge/License-Apache%202.0-3b82f6?style=flat-square" alt="License"></a>
<a href="https://pypi.org/project/strix-agent/"><img src="https://img.shields.io/pypi/v/strix-agent?style=flat-square" alt="PyPI Version"></a>


<a href="https://discord.gg/strix-ai"><img src="https://github.com/usestrix/.github/raw/main/imgs/Discord.png" height="40" alt="Únete al Discord"></a>
<a href="https://x.com/strix_ai"><img src="https://github.com/usestrix/.github/raw/main/imgs/X.png" height="40" alt="Sigue en X"></a>


<a href="https://trendshift.io/repositories/15362?utm_source=trendshift-badge&amp;utm_medium=badge&amp;utm_campaign=badge-trendshift-15362" target="_blank" rel="noopener noreferrer"><img src="https://trendshift.io/api/badge/trendshift/repositories/15362/weekly" alt="usestrix%2Fstrix | Trendshift" width="250" height="55"/></a>
<a href="https://trendshift.io/repositories/15362" target="_blank"><img src="https://trendshift.io/api/badge/repositories/15362" alt="usestrix/strix | Trendshift" width="250" height="55"/></a>

</div>


> [!TIP]
> **¡Nuevo!** Strix se integra perfectamente con GitHub Actions y pipelines CI/CD. Escanea automáticamente vulnerabilidades en cada pull request y bloquea código inseguro antes de que llegue a producción - [Empieza sin configuración](https://app.strix.ai).

---


## Resumen de Strix

Strix son agentes autónomos de pentesting con IA que actúan como hackers reales - ejecutan tu código dinámicamente, encuentran vulnerabilidades y las validan con pruebas de concepto reales. Creado para desarrolladores y equipos de seguridad que necesitan pruebas de seguridad rápidas y precisas sin la carga del pentesting manual ni los falsos positivos de las herramientas de análisis estático.

**Capacidades clave:**

- **Kit completo de pentesting** - reconocimiento, explotación y validación listos para usar
- **Orquestación multi-agente** - equipos de pentesters de IA que colaboran y escalan
- **Validación real de exploits** - PoCs funcionales, no falsos positivos como los escáneres de vulnerabilidades tradicionales
- **CLI pensada para desarrolladores** - hallazgos accionables con guía de remediación
- **Auto-arreglo e informes** - genera parches e informes de pentest listos para compliance


<br>


<div align="center">
  <a href="https://strix.ai">
    <img src=".github/screenshot.png" alt="Strix Demo" width="1000" style="border-radius: 16px;">
  </a>
</div>


## Casos de Uso

- **Pruebas de seguridad de aplicaciones** - Detecta y valida vulnerabilidades críticas en tus aplicaciones
- **Pentesting rápido** - Pruebas de penetración en horas, no semanas, con informes de compliance
- **Automatización de Bug Bounty** - Automatiza la investigación de bug bounty y genera PoCs para reportar más rápido
- **Integración CI/CD** - Ejecuta pruebas en CI/CD para bloquear vulnerabilidades antes de producción

## 🚀 Inicio Rápido

**Requisitos:**
- Docker (en ejecución)
- Una clave API de LLM de cualquier [proveedor soportado](https://docs.strix.ai/llm-providers/overview) (OpenAI, Anthropic, Google, etc.)

### Instalación y Primer Escaneo

```bash
# Instalar Strix
curl -sSL https://strix.ai/install | bash

# Configurar tu proveedor de IA
export STRIX_LLM="openai/gpt-5.4"
export LLM_API_KEY="tu-api-key"

# Ejecutar tu primera evaluación de seguridad
strix --target ./directorio-de-la-app
```

> [!NOTE]
> El primer uso descarga automáticamente la imagen Docker de sandbox. Los resultados se guardan en `strix_runs/<nombre-del-run>`

---

## ☁️ Plataforma Strix

Prueba la plataforma completa de pentesting de Strix en **[app.strix.ai](https://app.strix.ai)** - regístrate gratis, conecta tus repos y dominios, y lanza un pentest en minutos.

- **Hallazgos validados con PoCs** - cada vulnerabilidad incluye un exploit de prueba de concepto funcional y pasos de reproducción
- **Autoarreglo con un clic** - parches de seguridad generados por IA como pull requests listos para fusionar
- **Pentesting continuo** - escaneo de vulnerabilidades siempre activo que sigue el ritmo de tus despliegues
- **Integraciones DevSecOps** - GitHub, GitLab, Bitbucket, Slack, Jira, Linear y pipelines CI/CD
- **Aprendizaje continuo** - IA que se basa en hallazgos pasados, se adapta a tu código y reduce falsos positivos con el tiempo

[**Empieza tu primer pentest →**](https://app.strix.ai)

---

## 🤖 Usa Strix desde tu Agente de Código

Strix está listo para agentes. Dale a Claude Code, Cursor, Codex o a cualquier agente compatible con [SKILL.md](https://agentskills.io) la capacidad de ejecutar pentests, arreglar hallazgos y configurar escaneos CI:

```bash
npx skills add usestrix/strix
```

Esto instala cuatro skills: **penetration-testing-with-strix** (ejecuta escaneos headless y lee resultados), **managed-pentesting-with-strix** (controla la plataforma gestionada [app.strix.ai](https://app.strix.ai) vía REST - sin Docker local ni clave LLM), **fix-security-vulnerabilities-with-strix** (remedia + re-escanea para verificar) y **ci-security-scanning-with-strix** (escaneo de PRs en CI). Los agentes pueden ejecutar Strix de dos maneras con el mismo motor - el CLI de código abierto localmente, o la nube gestionada cuando no hay infraestructura local - y leer [`AGENTS.md`](AGENTS.md) como referencia rápida, [docs.strix.ai/llms.txt](https://docs.strix.ai/llms.txt) para la documentación del CLI y [docs.app.strix.ai](https://docs.app.strix.ai) para la API.

---

## ✨ Características

### Herramientas de Pentesting Agentico

Los agentes de Strix vienen equipados con un kit completo de seguridad ofensiva - las mismas herramientas que usan los pentesters profesionales y hackers éticos:

- **Proxy de Interceptación HTTP** - Manipulación y análisis completo de peticiones/respuestas con Caido
- **Explotación de Navegador** - Navegador automatizado para probar XSS, CSRF, clickjacking y flujos de bypass de autenticación
- **Ejecución de Shell y Comandos** - Terminal interactivo para desarrollo de exploits y post-explotación
- **Runtime de Exploits Personalizados** - Sandbox de Python para escribir y validar exploits de prueba de concepto
- **Reconocimiento y OSINT** - Mapeo automatizado de superficie de ataque, enumeración de subdominios y fingerprinting
- **Análisis de Código Estático y Dinámico** - Capacidades SAST + DAST para pruebas completas de seguridad de aplicaciones
- **Base de Conocimiento de Vulnerabilidades** - Hallazgos estructurados con puntuación CVSS y clasificación OWASP

### Escáner Integral de Vulnerabilidades

Strix identifica, valida y explota una amplia gama de vulnerabilidades de seguridad del OWASP Top 10 y más allá:

- **Control de Acceso Roto** - IDOR, escalada de privilegios, bypass de autenticación
- **Ataques de Inyección** - Inyección SQL, inyección NoSQL, inyección de comandos OS, SSTI
- **Vulnerabilidades del Servidor** - SSRF, XXE, deserialización insegura, RCE
- **Ataques del Lado del Cliente** - XSS (almacenado/reflejado/DOM), contaminación de prototipos, CSRF
- **Fallos de Lógica de Negocio** - Condiciones de carrera, manipulación de pagos, bypass de flujos de trabajo
- **Autenticación y Sesión** - Ataques JWT, fijación de sesión, vectores de credential stuffing
- **Infraestructura y Nube** - Mala configuración, servicios expuestos, problemas de seguridad en la nube
- **Seguridad de APIs** - Autenticación rota, mass assignment, bypass de límite de tasa

### Grafo de Agentes (Pentesting Multi-Agente)

Orquestación multi-agente avanzada para pentesting automatizado completo:

- **Pentesting Distribuido** - Agentes de IA especializados en reconocimiento, explotación y post-explotación
- **Pruebas de Seguridad Escalables** - Ejecución paralela en múltiples objetivos para cobertura rápida y completa
- **Coordinación Dinámica** - Los agentes comparten descubrimientos, encadenan vulnerabilidades y colaboran como un equipo rojo

---

## 🖥️ Visor Web Local

Cada escaneo escribe sus resultados en disco mientras se ejecuta. Míralos en un panel local con un solo comando:

```bash
# Abrir el run más reciente
strix view

# ...o abrir un run específico por nombre
strix view nombre-del-run
```

`strix view` inicia un servidor local ligero (vinculado a `127.0.0.1` en un puerto aleatorio) y abre tu navegador con un enlace privado con token. Nada sale de tu máquina: el panel lee los archivos del run directamente del disco, sin cuenta en la nube ni subida. La interfaz viene precompilada con Strix, así que no hay instalación extra ni paso de build JS.

### Qué hay en el panel

- **Resumen**: estado del run, objetivo y desglose de severidad de todo lo encontrado hasta ahora.
- **Vulnerabilidades**: cada hallazgo validado con su severidad, detalles y pasos de reproducción.
- **Grafo de agentes**: un mapa en vivo del equipo multi-agente, mostrando qué agente hace qué.
- **Control**: envía instrucciones a un escaneo en vivo desde el navegador para redirigir a los agentes a mitad del run.
- **Historial**: navega por runs pasados en esta máquina y salta entre ellos.
- **Informes**: genera un informe compartible y envíalo por correo a ti o a tu equipo.

---

## Ejemplos de Uso

### Uso Básico

```bash
# Escanear un codebase local
strix --target ./directorio-de-la-app

# Revisión de seguridad de un repositorio de GitHub
strix --target https://github.com/org/repo

# Evaluación black-box de una aplicación web
strix --target https://tu-app.com
```

### Pruebas de API (OpenAPI / Swagger / Postman)

Apunta Strix a un contrato de API y prueba cada endpoint declarado en lugar de
tener que descubrirlos rastreando. Combina el spec con la URL base en vivo para que el
agente sepa a dónde enviar el tráfico:

```bash
# Archivo OpenAPI / Swagger (.json / .yaml)
strix --target ./openapi.yaml --target https://api.tu-app.com

# Exportación de colección Postman
strix --target ./coleccion.postman_collection.json --target https://api.tu-app.com

# Colección Postman descargada en vivo por id (sin exportación manual)
export POSTMAN_API_KEY="PMAK-..."
strix --target postman://<uuid-de-coleccion>

# ...con un entorno Postman para resolver {{baseUrl}} / variables de token
strix --target "postman://<uuid-de-coleccion>?env=<uuid-de-entorno>"
```


### Escenarios de Pruebas Avanzadas

```bash
# Pruebas autenticadas grey-box
strix --target https://tu-app.com --instruction "Realiza pruebas autenticadas usando credenciales: usuario:contraseña"

# Pruebas multi-objetivo (código fuente + app desplegada)
strix -t https://github.com/org/app -t https://tu-app.com

# Objetivos desde un archivo, uno por línea no vacía ni comentada
strix --target-list ./objetivos.txt

# Escaneo white-box consciente del código fuente (repositorio local)
strix --target ./directorio-de-la-app --scan-mode standard

# Pruebas enfocadas con instrucciones personalizadas
strix --target api.tu-app.com --instruction "Enfócate en fallos de lógica de negocio y vulnerabilidades IDOR"

# Proporciona instrucciones detalladas a través de archivo (reglas de compromiso, alcance, exclusiones)
strix --target api.tu-app.com --instruction-file ./instrucciones.md

# Fuerza el alcance de diff del PR contra una rama base específica
strix -n --target ./ --scan-mode quick --scope-mode diff --diff-base origin/main
```

### Modo Headless

Ejecuta Strix programáticamente sin interfaz interactiva con el flag `-n/--non-interactive` - perfecto para servidores y trabajos automatizados. El CLI imprime los hallazgos de vulnerabilidades en tiempo real y el informe final antes de salir. Sale con código no-cero cuando se encuentran vulnerabilidades.

```bash
strix -n --target https://tu-app.com
```

### CI/CD (GitHub Actions)

Strix se puede añadir a tu pipeline para ejecutar una prueba de seguridad en pull requests con un flujo de trabajo ligero de GitHub Actions:

```yaml
name: strix-penetration-test

on:
  pull_request:

jobs:
  security-scan:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v6
        with:
          fetch-depth: 0

      - name: Instalar Strix
        run: curl -sSL https://strix.ai/install | bash

      - name: Ejecutar Strix
        env:
          STRIX_LLM: ${{ secrets.STRIX_LLM }}
          LLM_API_KEY: ${{ secrets.LLM_API_KEY }}

        run: strix -n -t ./ --scan-mode quick
```

> [!TIP]
> En ejecuciones de CI de pull requests, Strix limita automáticamente las revisiones rápidas a los archivos cambiados.
> Si el alcance por diff no se resuelve, asegúrate de que el checkout use el historial completo (`fetch-depth: 0`) o pasa
> `--diff-base` explícitamente.

### Configuración

```bash
export STRIX_LLM="openai/gpt-5.4"
export LLM_API_KEY="tu-api-key"

# Opcional
export LLM_API_BASE="tu-url-base-api"  # si usas un modelo local, ej. Ollama, LMStudio
export PERPLEXITY_API_KEY="tu-api-key"  # para capacidades de búsqueda
export STRIX_REASONING_EFFORT="high"  # controla el esfuerzo de razonamiento (por defecto: high, escaneo rápido: medium)
```

> [!NOTE]
> Strix guarda automáticamente tu configuración en `~/.strix/cli-config.json`, para que no tengas que reingresarla en cada ejecución.

#### Inicia sesión con una suscripción de ChatGPT

En lugar de una clave API con medidor, puedes ejecutar Strix con tu suscripción de ChatGPT Plus/Pro:

```bash
strix auth login chatgpt      # inicia sesión con tu cuenta de ChatGPT

export STRIX_LLM="chatgpt/gpt-5.4"   # chatgpt/<modelo> corre con la suscripción
strix --target ./directorio-de-la-app

strix auth status             # muestra el inicio de sesión activo
strix auth logout             # olvida el inicio de sesión
```

**Modelos recomendados para mejores resultados:**

- [OpenAI GPT-5.4](https://openai.com/api/) - `openai/gpt-5.4`
- [Anthropic Claude Sonnet 4.6](https://claude.com/platform/api) - `anthropic/claude-sonnet-4-6`
- [Google Gemini 3 Pro Preview](https://cloud.google.com/vertex-ai) - `vertex_ai/gemini-3-pro-preview`

Consulta la [documentación de Proveedores de LLM](https://docs.strix.ai/llm-providers/overview) para todos los proveedores soportados incluyendo Vertex AI, Bedrock, Azure y modelos locales.

## Pentesting Empresarial

Obtén la misma experiencia de Strix con controles de [nivel empresarial](https://strix.ai/demo): SSO (SAML/OIDC), informes de pentesting personalizados listos para compliance (SOC 2, ISO 27001, PCI DSS), soporte dedicado y SLA, opciones de despliegue personalizadas (VPC/self-hosted), soporte de modelos BYOK y agentes de pentesting con IA adaptados a tu entorno. [Más información](https://strix.ai/demo).

## Documentación

La documentación completa está disponible en **[docs.strix.ai](https://docs.strix.ai)** - incluyendo guías detalladas de uso, integraciones CI/CD, skills y configuración avanzada.

## Contribuir

Aceptamos contribuciones de código, documentación y nuevas skills - consulta nuestra [Guía de Contribución](https://docs.strix.ai/contributing) para empezar o abre un [pull request](https://github.com/usestrix/strix/pulls)/[issue](https://github.com/usestrix/strix/issues).

## Únete a Nuestra Comunidad

¿Tienes preguntas? ¿Encontraste un bug? ¿Quieres contribuir? **[¡Únete a nuestro Discord!](https://discord.gg/strix-ai)**

## Apoya el Proyecto

**¿Te encanta Strix?** ¡Dale una ⭐ en GitHub!

## Agradecimientos

Strix se construye sobre el increíble trabajo de proyectos de código abierto como [LiteLLM](https://github.com/BerriAI/litellm), [Caido](https://github.com/caido/caido), [Nuclei](https://github.com/projectdiscovery/nuclei), [Playwright](https://github.com/microsoft/playwright) y [Bubble Tea](https://github.com/charmbracelet/bubbletea). ¡Muchas gracias a sus mantenedores!


> [!WARNING]
> **Solo uso autorizado.** Strix prueba activamente los objetivos a los que lo apuntas, así que solo ejecútalo contra sistemas que poseas o para los que tengas **permiso explícito y por escrito** para probar, y mantente dentro del alcance acordado. Las pruebas no autorizadas son ilegales en la mayoría de las jurisdicciones.
> Tú eres el único responsable de obtener la autorización y cumplir la ley. Strix se proporciona "tal cual" sin garantía ni responsabilidad por uso indebido.

</div>
