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

```
