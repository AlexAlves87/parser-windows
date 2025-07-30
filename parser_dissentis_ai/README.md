# 🧠 Dissentis.AI Parser – Backend Windows Edition

## 📌 Propósito

El backend de `parser-windows` es el **núcleo industrial del sistema Dissentis.AI Parser**, orientado a la **ingesta masiva, procesamiento estructurado y transformación semántica** de documentos multiformato, todo ello **sin conexión a internet** ni dependencia de servicios externos.

Está diseñado para operar bajo los principios de:
- ⚙️ **Robustez estructural**
- 📐 **Modularidad estricta**
- 🔐 **Control de acceso local**
- 📊 **Auditoría trazable**
- 🧱 **Preparación óptima para ingesta en LLMs**

---

## ⚙️ Funcionalidades Principales

- ✅ **Ingesta multiformato automática**:
  Procesa formatos como `.pdf`, `.docx`, `.html`, `.xml`, `.epub`, `.pptx`, `.csv`, `.json`, `.eml`, entre otros.

- ✅ **Conversión a Markdown estructurado**:
  Preserva jerarquía semántica (títulos, listas, tablas) en `.txt` con sintaxis Markdown.

- ✅ **Segmentación semántica (chunking)**:
  Fragmenta el texto para facilitar la vectorización y análisis en LLMs.

- ✅ **Salida configurable**:
  Soporte para `.txt`, `.md`, `.csv`, `.json` y exportación por chunk o documento completo.

- ✅ **Cola de procesamiento local**:
  Con priorización, reintentos y cancelación de trabajos sin necesidad de conexión.

- ✅ **Monitoreo y trazabilidad completa**:
  Logs estructurados, historial de trabajos y estadísticas locales.

- ✅ **Control de acceso y seguridad local**:
  Autenticación, roles y políticas sin servicios externos ni APIs remotas.

---

## 🗂️ Estructura del Proyecto

```

parser\_dissentis\_ai/
├── backend/             # Núcleo de procesamiento
│   ├── core/            # Engine principal, configuración y errores
│   ├── parsers/         # Módulos de extracción por formato
│   ├── processors/      # Transformación, normalización y salida
│   ├── orchestration/   # Gestión de colas
│   ├── access\_control/  # Seguridad y autenticación local
│   ├── observability/   # Logging, métricas y monitoreo
│   └── utils/           # Utilidades comunes
├── frontend/            # CLI, API REST y GUI opcional
├── tests/               # Tests estructurados
├── docs/                # Documentación técnica
├── scripts/             # Scripts de entorno y despliegue
├── pyproject.toml       # Configuración con Poetry
├── README.md            # Este archivo
└── LICENSE              # Licencia del proyecto

````

---

## 🚀 Requisitos y Uso

### 🧪 Requisitos

- Python 3.10+
- [Poetry](https://python-poetry.org/) para gestión de dependencias
- Sistema operativo Windows 10/11 (compatible con otras plataformas en versiones futuras)

### ⚙️ Instalación

```bash
git clone https://github.com/AlexAlves87/parser-windows.git
cd parser-windows
poetry install
````

### ▶️ Ejecución CLI (modo local)

```bash
poetry run python -m frontend.cli.app
```

### 🌐 Servidor API

```bash
poetry run python -m frontend.api.server
```

---

## 📚 Documentación

Consulta los archivos en el directorio `docs/`:

* `architecture.md` – Visión técnica y modular
* `usage.md` – Guía de uso por CLI o API
* `api_reference.md` – Especificación de endpoints y estructura

---

## 🛡️ Seguridad y Privacidad

El sistema opera completamente **offline**, con autenticación local y sin transferencia externa de datos. Diseñado bajo principios **privacy-first** para uso institucional o sensible.

---

## 📄 Licencia

MIT © Alex Alves — Uso libre con atribución.

---

## ✨ Contribuciones

Sistema en desarrollo activo. Pull requests y propuestas de mejora son bienvenidas bajo revisión técnica estructural.

```
