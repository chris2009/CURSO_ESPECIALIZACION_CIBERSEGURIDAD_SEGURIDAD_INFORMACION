<div align="center">

# 🛡️ Curso de Especialización en Ciberseguridad y Seguridad de la Información
### ESAN Graduate School of Business

![Status](https://img.shields.io/badge/estado-en%20progreso-yellow)
![Institución](https://img.shields.io/badge/instituci%C3%B3n-ESAN-c00000)
![Materiales](https://img.shields.io/badge/material-PDF%20%7C%20DOCX%20%7C%20XLSX%20%7C%20PPTX-blue)
![Licencia](https://img.shields.io/badge/uso-acad%C3%A9mico-lightgrey)

Repositorio personal con el material de clase, casos de discusión y trabajos grupales desarrollados durante el **Programa de Especialización en Ciberseguridad y Seguridad de la Información** de ESAN.

</div>

---

## 📑 Tabla de contenidos

- [Descripción general](#-descripción-general)
- [Estructura del repositorio](#-estructura-del-repositorio)
- [1ra Parte — Informática Forense y Evidencia Digital](#1️⃣-1ra_parte--informática-forense-y-evidencia-digital)
- [2da Parte — Arquitectura de Ciberseguridad](#2️⃣-2da_parte--arquitectura-de-ciberseguridad)
- [3ra Parte — Gestión de Riesgos de Ciberseguridad](#3️⃣-3ra_parte--gestión-de-riesgos-de-ciberseguridad)
- [Marcos y estándares cubiertos](#-marcos-y-estándares-cubiertos)
- [Archivos excluidos del repositorio](#-archivos-excluidos-del-repositorio-gitignore)
- [Tecnologías y herramientas](#-tecnologías-y-herramientas-utilizadas)
- [Autor](#-autor)

---

## 📖 Descripción general

Este repositorio documenta el recorrido completo del curso, organizado en **tres bloques temáticos** que corresponden a los módulos dictados en el programa:

| Bloque | Tema central | Caso(s) aplicado(s) |
|---|---|---|
| 🔍 **1ra Parte** | Informática Forense y Evidencia Digital | Caso forense simulado "ESAN-2026-001" (análisis con Autopsy) |
| 🏗️ **2da Parte** | Arquitectura de Ciberseguridad | Caso Bankitor (arquitectura TO-BE: corto, mediano y largo plazo) |
| 📊 **3ra Parte** | Gestión de Riesgos de Ciberseguridad | Caso SolarWinds / Sunburst (2020) — Trabajo Final Grupal |

Cada bloque incluye el material de clase (diapositivas/PDF), casos de discusión analizados en sesión, y los entregables/trabajos finales desarrollados a partir de ese material.

---

## 🗂️ Estructura del repositorio

```text
CURSO_CIBERSEGURIDAD_ESAN/
├── 1ra_Parte/                          🔍 Informática Forense
│   ├── Clase - Introducción a la Informática Forense.pdf
│   ├── Clase - Adquisición y Preservación.pdf
│   ├── Clase - Análisis Forense de Sistemas.pdf
│   ├── Clase - Documentación e Informe Forense.pdf
│   ├── SANS_DFPS_FOR500 (guía de referencia internacional).pdf
│   ├── Manuales de acceso y recojo de evidencia digital
│   └── entregables_grupo_3/            📦 Caso forense aplicado (ESAN-2026-001)
│       ├── 0_Bitacora_Tecnica
│       ├── 1_Acta_Adquisicion
│       ├── 2_Cadena_Custodia
│       └── 5_Informe_Forense_Final
│
├── 2da_Parte/                          🏗️ Arquitectura de Ciberseguridad
│   ├── Fundamentos de Ciberseguridad (redes, dispositivos, dominios).pdf
│   ├── Defensa en profundidad.pdf · Zero Trust.pdf
│   ├── Caso Bankitor.pdf
│   ├── Bankitor_Arquitectura_Seguridad_Completa.md / .pdf
│   ├── exposicion.md / .pdf
│   └── Trabajo_Arquitectura_Ciberseguridad/   📦 Trabajo final grupal
│       ├── corto_plazo/    (arquitectura + diagrama draw.io)
│       ├── mediano_plazo/  (arquitectura + diagrama draw.io)
│       ├── largo_plazo/    (arquitectura + diagrama draw.io)
│       └── Caso-Bankitor-Arquitectura-de-Seguridad-TO-BE (.docx/.pptx)
│
├── 3ra_Parte/                          📊 Gestión de Riesgos de Ciberseguridad
│   ├── Sesión 1 — Fundamentos de Gestión de Riesgos.pdf
│   ├── Sesión 2 — Identificación y Análisis de Riesgos.pdf
│   ├── Sesión 3 — Evaluación y Tratamiento de Riesgos.pdf
│   ├── Sesión 4 — Monitoreo, Mejora Continua y Gestión Aplicada.pdf
│   ├── Casos de discusión (Hospitales-Ransomware, Facebook, Uber).pdf/.pptx
│   ├── ANALISIS AMFE + CONTROLES Ciberseguridad.xlsx
│   ├── Inventario de Activos de Información.xlsx
│   ├── Resumen_Sesiones_1-4.md         📝 Resumen exhaustivo del curso (autogenerado)
│   ├── estructura_trabajo_final.png    🖼️ Lineamientos oficiales del trabajo final
│   └── Trabajo_Final_SolarWinds.docx   📦 Trabajo final grupal (caso SolarWinds 2020)
│
├── cronograma.png                      🗓️ Cronograma general del programa
└── .gitignore                          🚫 Exclusiones (ver sección correspondiente)
```

---

## 1️⃣ 1ra_Parte — Informática Forense y Evidencia Digital

Módulo centrado en el **ciclo de vida de la evidencia digital**: identificación, adquisición, preservación, análisis y elaboración del informe forense, siguiendo buenas prácticas reconocidas internacionalmente (SANS FOR500, cadena de custodia).

**Caso aplicado:** investigación forense simulada sobre una imagen de disco (`.E01`), documentada en `entregables_grupo_3/` con:
- 📓 Bitácora técnica del análisis
- 📝 Acta de adquisición de la evidencia
- 🔗 Cadena de custodia
- 📄 Informe forense final

> ⚠️ La imagen forense original (`.E01`, ~110 MB) y las carpetas de trabajos individuales/grupales detallados **no se incluyen en este repositorio** por tamaño y por contener material de trabajo en proceso (ver [exclusiones](#-archivos-excluidos-del-repositorio-gitignore)).

---

## 2️⃣ 2da_Parte — Arquitectura de Ciberseguridad

Módulo enfocado en el **diseño de arquitecturas de seguridad por capas**: defensa en profundidad, Zero Trust, dominios de ciberseguridad y administración segura de dispositivos.

**Caso aplicado — "Bankitor":** una entidad financiera ficticia para la cual se diseñó una **hoja de ruta de arquitectura de seguridad en 3 horizontes**:

| Horizonte | Enfoque |
|---|---|
| 🟢 Corto plazo | Controles básicos y cierre de brechas críticas inmediatas |
| 🟡 Mediano plazo | Fortalecimiento de la arquitectura y madurez de procesos |
| 🔴 Largo plazo | Arquitectura objetivo (TO-BE) alineada a Zero Trust |

Cada horizonte incluye su documento de arquitectura (`.md`/`.pdf`) y su diagrama editable en formato **draw.io** (`.xml`).

---

## 3️⃣ 3ra_Parte — Gestión de Riesgos de Ciberseguridad

Módulo que desarrolla el **ciclo completo de gestión de riesgos** (ISO 31000) aplicado a ciberseguridad, a través de 4 sesiones:

| Sesión | Contenido |
|---|---|
| 1 | Fundamentos: activos, amenazas, vulnerabilidades, impacto, marcos internacionales |
| 2 | Identificación y análisis de riesgos (cualitativo, cuantitativo, AMFE/FMEA) |
| 3 | Evaluación y tratamiento de riesgos (mitigar / transferir / evitar / aceptar) |
| 4 | Monitoreo continuo, KRIs, auditoría, gestión de incidentes y mejora continua (PDCA) |

Cada sesión incluyó un **caso de discusión real**: Ransomware a Hospitales (COVID-19), Equifax, Fuga de datos en Facebook e Incidente de seguridad en Uber.

📝 El archivo [`3ra_Parte/Resumen_Sesiones_1-4.md`](3ra_Parte/Resumen_Sesiones_1-4.md) contiene un **resumen exhaustivo** de las 4 sesiones (definiciones, fórmulas, tablas y matrices de riesgo, KRIs, controles y casos de discusión).

### 🎯 Trabajo Final Grupal — Caso SolarWinds / Sunburst (2020)

📄 [`3ra_Parte/Trabajo_Final_SolarWinds.docx`](3ra_Parte/Trabajo_Final_SolarWinds.docx)

Aplicación del ciclo completo de gestión de riesgos al ataque a la cadena de suministro de software que comprometió a ~18,000 organizaciones (incluyendo 9 agencias del gobierno de EE.UU.) entre 2019 y 2020, atribuido a APT29/Nobelium.

**Estructura del trabajo (8 secciones, según lineamientos oficiales del curso):**

1. Antecedentes de la organización
2. Identificación de activos de información
3. Identificación de amenazas y vulnerabilidades
4. Matriz de Riesgos (Probabilidad × Impacto)
5. Indicadores Clave de Riesgo (KRIs)
6. Propuesta de controles según marcos de referencia
7. Conclusiones y recomendaciones
8. Bibliografía (con hipervínculos a fuentes oficiales: CISA, NIST, Microsoft, Mandiant)

**Integrantes del grupo:**
- Christian Edgardo Cajusol Mio
- Freddy Saldaña Reynoso

---

## 🧭 Marcos y estándares cubiertos

A lo largo del curso se trabajó de forma transversal con los siguientes marcos de referencia internacionales:

| Categoría | Marcos / Estándares |
|---|---|
| Gestión de riesgos | `ISO 31000:2018` · `ISO/IEC 27005` · `NIST SP 800-30` · `FAIR` · `AMFE/FMEA` |
| Seguridad de la información | `ISO/IEC 27001:2022` · `NIST SP 800-53 Rev. 5` |
| Gobernanza y estrategia | `NIST CSF 2.0` · `COBIT` · `ISO/IEC 27014` |
| Cadena de suministro / desarrollo seguro | `NIST SP 800-161` · `NIST SP 800-218 (SSDF)` |
| Controles técnicos | `CIS Controls v8` · `MITRE ATT&CK` · `OWASP Top 10` |
| Continuidad y resiliencia | `ISO 22301` |
| Informática forense | `SANS FOR500` · Cadena de custodia (buenas prácticas internacionales) |

---

## 🚫 Archivos excluidos del repositorio (`.gitignore`)

Por motivos de **tamaño**, **confidencialidad académica** o por tratarse de **material de trabajo en proceso** (no entregables finales), se excluyen intencionalmente:

```gitignore
1ra_Parte/Trabajo_Investigacion_Forense_Evidencia_Digital/
1ra_Parte/Trabajo_Investigacion_Grupo_1/
1ra_Parte/DisableUSBWrite.zip
1ra_Parte/EnableUSBWrite.zip
3ra_Parte/Trabajo_Final.docx
~$*   # archivos temporales de bloqueo de Word/Office
```

> Estos archivos permanecen disponibles localmente, pero no forman parte del historial del repositorio remoto.

---

## 🛠️ Tecnologías y herramientas utilizadas

- **Análisis forense:** Autopsy, ExifTool, FTK Imager (adquisición de imágenes `.E01`)
- **Diagramación de arquitectura:** draw.io (`.xml`)
- **Gestión de riesgos:** plantillas AMFE/FMEA, matrices de riesgo en Excel
- **Documentación:** Markdown, Word, PowerPoint, Excel
- **Control de versiones:** Git / GitHub

---

## 👤 Autor

**Christian Edgardo Cajusol Mio**
Programa de Especialización en Ciberseguridad y Seguridad de la Información — ESAN Graduate School of Business

---

<div align="center">
<sub>Repositorio de uso académico. El contenido pertenece a su autor y se comparte con fines de aprendizaje y portafolio personal.</sub>
</div>
