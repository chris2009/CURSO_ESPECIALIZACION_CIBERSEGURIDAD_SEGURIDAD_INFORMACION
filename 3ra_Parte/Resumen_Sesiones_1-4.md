# Resumen del Curso: Gestión de Riesgos de la Ciberseguridad (ESAN)
### Profesor: Freddy Alvarado Vargas (falvarado@esan.edu.pe)

Este documento integra el contenido de las cuatro sesiones del curso, siguiendo el ciclo de gestión de riesgos: Fundamentos → Identificación y Análisis → Evaluación y Tratamiento → Monitoreo y Mejora Continua.

---

## Sesión 1: Fundamentos de la Gestión de Riesgos de Ciberseguridad

**Logro de aprendizaje:** Comprender los fundamentos de la gestión de riesgos de ciberseguridad: identificar activos, amenazas, vulnerabilidades e impactos, y aplicar marcos internacionales para la protección de la información y continuidad del negocio.

**Estadísticas globales (2024):**
- 5.5 billones de ataques cibernéticos en el mundo (phishing, ransomware, DDoS, malware, brechas de datos) - Check Point Research 2024.
- USD 10.5 billones (trillions) costo global de ciberataques 2024 - Cybersecurity Ventures.
- Sectores más afectados: financiero, sector público, sector sanitario - World Economic Forum.
- Ciberseguridad es la 4ta mayor preocupación de la humanidad (WEF Global Risk Report 2024).
- Phishing: ataque más común, ~3,400 millones de correos spam diarios (2024).
- 60% de CEOs no incorpora ciberseguridad en estrategia empresarial (Accenture, dic. 2023, 1000 CEOs).
- 54% de CEOs creen que el costo de la ciberseguridad es mayor al de sufrir un ciberataque.
- 300,000 nuevas versiones de malware al día; 92% distribuido por correo; media de 49 días para detección.
- $12.8 mil millones en pérdidas por cibercrimen (FBI Internet Crime Complaint Center 2018-2023; 2023: 880,418 quejas, $12.5 billion losses).
- Costo promedio global de filtración de datos (IBM): de $4.00M (2016) a $4.35M (2022).

**Perú:**
- 2020: BCR sufrió ransomware.
- 2021: Ministerio de Salud, robo de información confidencial de pacientes.
- 2022: Filtración de datos a Sedapal, Petroperú y Reniec (denuncia ASBANC).
- 2023: 5,000 millones de intentos de ciberataque (Fortinet); sectores: energía, minería, banca, retail, turismo.
- USD 100 millones en pérdidas anuales por ciberataques (APETI).
- 2024: Interbank (data breach).
- Normatividad de ciberseguridad incipiente; desconfianza digital.

**Conceptos fundamentales (norma UNE 71504:2008):**
- **Activo:** componente o funcionalidad de un sistema de información susceptible de ser atacado, con consecuencias para la organización (información, datos, servicios, software, hardware, comunicaciones, recursos administrativos, físicos y humanos).
- **Infraestructuras críticas:** sistemas esenciales para servicios vitales (transporte, energía, agua, telecomunicaciones, seguridad); su paralización afecta a toda la sociedad; son blanco de terroristas.
- **Amenaza:** causa potencial de un incidente que puede causar daños a un sistema de información o a una organización. Origen: natural, del entorno/industrial, defectos de aplicaciones, accidental por personas, deliberada por personas (intencionados). Ciberamenazas: ciberespionaje industrial/gubernamental, ciberataques a infraestructuras críticas, ciberdelincuencia financiera, robo/comercialización de información, cibersabotaje, ciberhacktivismo.
- **Tipos de amenazas de ciberseguridad** (ISO/IEC 27001:2022, NIST CSF, ENISA): (1) Malware (virus, gusanos, troyanos, spyware, ransomware, adware); (2) Phishing e ingeniería social (phishing, spear phishing, smishing, vishing, suplantación); (3) Amenazas internas (empleados maliciosos, negligencia, uso indebido de privilegios, fuga de información); (4) Amenazas aplicativas (inyección SQL, XSS, autenticación débil, componentes vulnerables); (5) Amenazas de red (sniffing, suplantación ARP/DNS, MITM, DoS/DDoS); (6) Amenazas avanzadas/APT (spear targeting, zero-day, movimiento lateral, exfiltración); (7) Amenazas físicas y ambientales (robo de equipos, incendios, inundaciones, fallas eléctricas).
- **Vulnerabilidad:** debilidad de un activo o de sus medidas de protección que puede ser aprovechada por una amenaza; ausencia o ineficacia de salvaguardas. Ejemplos comunes: software desactualizado, contraseñas débiles, configuraciones incorrectas, falta de MFA, ausencia de segmentación de red, permisos excesivos, falta de copias de seguridad/backups.
- **Riesgo:** posibilidad de que una amenaza explote una vulnerabilidad generando impacto negativo sobre un activo. ISO 31000: "efecto de la incertidumbre sobre los objetivos". Fórmula: **Riesgo = Impacto × Frecuencia × Detección** (también referenciada como Probabilidad × Impacto en sesiones posteriores). Análisis de riesgos = proceso sistemático para estimar la magnitud de los riesgos a los que está expuesta una organización.
- **Impacto:** medida del daño sobre el activo derivado de la materialización de una amenaza; depende del valor del activo (tangible/intangible) y su relevancia para los procesos.

**Tabla comparativa de impacto - casos reales mencionados:** Colonial Pipeline (2021, ransomware DarkSide, USD 4.4M rescate), Equifax (2017, explotación vulnerabilidad web, USD 1,400M en multas), Maersk (2017, NotPetya, USD 300M), Sony Pictures (2014, APT, USD 100M+), Target (2013, robo tarjetas POS, USD 200M+), Marriott (2018, brecha 500M huéspedes, USD 100M+), WannaCry (ransomware, USD 4,000M pérdidas globales, afectó NHS Reino Unido), Uber (2022, ingeniería social), **SolarWinds (2020, ataque a cadena de suministro, compromiso de agencias gubernamentales y grandes empresas, impacto geopolítico y revisión global de proveedores TI)**, British Airways (2018, multa GDPR ~GBP 20M), JBS (2021, ransomware, rescate USD 11M), SingHealth (2018, APT, 1.5M pacientes).

**Tipos de ciberataques detallados:**
- **Phishing:** ingeniería social para obtener credenciales/info financiera o instalar malware. Variantes: spear phishing, whaling, smishing, vishing.
- **Ransomware:** malware que cifra información y exige pago. Fases: infección inicial → movimiento lateral → escalamiento de privilegios → cifrado → extorsión. Casos: WannaCry (2017), Colonial Pipeline (2021), ataques a hospitales COVID-19.
- **APT (Advanced Persistent Threat):** ataques avanzados, persistentes, dirigidos por grupos especializados (ej. APT29). "Avanzada" = herramientas personalizadas/zero-days; "Persistente" = mantener acceso a largo plazo con puertas traseras; "Amenaza" = operadores humanos organizados y financiados.

**Marcos internacionales (introducción):**
- **ISO 31000 (Gestión de Riesgos):** principios (integración organizacional, personalización, inclusión de stakeholders, mejora continua, basado en información disponible). Proceso: 1) Establecimiento del contexto, 2) Identificación de riesgos, 3) Análisis de riesgos, 4) Evaluación de riesgos, 5) Tratamiento de riesgos, 6) Monitoreo y revisión. Aplicable a cualquier tipo/tamaño de organización, no es certificable (es guía, no requisito).
- **ISO/IEC 27001:2022:** estándar para Sistema de Gestión de Seguridad de la Información (SGSI). Objetivos: proteger información, gestionar riesgos, continuidad operativa, cumplimiento regulatorio. Tríada CIA. Controles: redujo de 14 grupos/114 controles (2013) a 4 grupos/93 controles (2022): 37 organizativos, 8 de personas, 14 físicos, 34 tecnológicos.
- **NIST Risk Management Framework (RMF):** 7 etapas: Prepare, Categorize, Select, Implement, Assess, Authorize, Monitor. Integración con NIST SP 800-53. Documentos clave: NIST SP 800-37 Rev.2, SP 800-53 Rev.5, SP 800-30 Rev.1, SP 800-18 Rev.1.
- **Pirámide de marcos de referencia de ciberseguridad** (5 niveles): 1) Estratégico/Gobernanza (ISO/IEC 27014, COBIT, NIST CSF), 2) Táctico/Gestión de Riesgos (ISO/IEC 27005, NIST SP 800-30, FAIR), 3) Operativo/Gestión y Controles (ISO/IEC 27001, NIST SP 800-53, CIS Controls), 4) Técnico/Implementación (NIST SP 800-171, CIS Benchmarks, MITRE ATT&CK), 5) Operación y Mejora Continua (NIST SP 800-137, ISO/IEC 27004, ITIL, ISACA). Clave: no implementar todos los marcos, sino integrar los más adecuados según contexto y madurez.
- **NIST CSF 2.0 - Gobernanza:** Nivel estratégico (Gobernar: dirección, supervisión, gestión, cultura/ética, comunicación) + Nivel de gestión (6 funciones: Identificar, Proteger, Detectar, Responder, Recuperar, Mejorar). Resultados para el negocio: gestión efectiva de riesgos, resiliencia organizacional, confianza y reputación, cumplimiento y valor.
- **Capas de seguridad** (modelo de 7 capas, similar a OSI): Física, Enlace de datos, Red, Transporte, Sesión, Presentación, Aplicación - cada una con controles específicos.

**Relación riesgos - seguridad de información - continuidad del negocio:** la gestión de riesgos es el eje integrador. Seguridad de información protege CIA; continuidad de negocio garantiza operación de procesos críticos ante incidentes (vía BIA, planes de contingencia, DRP/BCP).

**Caso de discusión Sesión 1: "Ataque de Ransomware a Hospitales durante la pandemia COVID-19"** - consorcio ficticio "Red Salud Integral" (RSI): 12 hospitales, 35 clínicas, 8,000 empleados, 2M historias clínicas. Fase 1: phishing con Excel malicioso (macro) suplantando al Ministerio de Salud. Fase 2: movimiento lateral 12 días (parches desactualizados, cuentas compartidas, sin MFA, sin segmentación, SOC limitado). Fase 3: ransomware simultáneo, rescate USD 8M. Impacto: paralización 9 días, 4,500 citas suspendidas, USD 25M pérdidas, daño reputacional y legal. Controles ausentes: gestión de vulnerabilidades débil, sin Zero Trust, monitoreo limitado, baja concientización, sin simulacros, sin BCP maduro.

**Conclusión de la sesión:** la gestión de riesgos protege la información, reduce amenazas y mejora la toma de decisiones; los riesgos surgen cuando una amenaza explota una vulnerabilidad sobre un activo; el error humano es causa frecuente de ataques; marcos como ISO 31000, ISO/IEC 27001 y NIST RMF dan metodología; la continuidad del negocio depende de la gestión de riesgos.

---

## Sesión 2: Identificación y Análisis de Riesgos

**Logro de aprendizaje:** Al finalizar la sesión, el participante será capaz de identificar activos críticos, amenazas y vulnerabilidades, así como analizar y evaluar riesgos de ciberseguridad mediante métodos cualitativos y cuantitativos, aplicando matrices de riesgo y metodologías internacionales para apoyar la toma de decisiones.

### 1. Introducción

La gestión de riesgos de ciberseguridad inicia con la comprensión de qué se debe proteger, de qué amenazas debe protegerse y cuáles son las debilidades que podrían ser explotadas. Según **NIST SP 800-30**, la evaluación de riesgos permite identificar eventos potenciales que pueden afectar los objetivos organizacionales y estimar su impacto sobre los activos críticos.

Una adecuada identificación y análisis de riesgos permite:
- Priorizar inversiones en seguridad.
- Reducir pérdidas económicas.
- Cumplir requisitos regulatorios.
- Incrementar la resiliencia organizacional.
- Mejorar la continuidad del negocio.

### NIST SP 800-30 — Guía para la Realización de Evaluaciones de Riesgos

El NIST SP 800-30 (Rev. 1) es una guía publicada por el National Institute of Standards and Technology (NIST) que proporciona un marco estructurado para que las organizaciones identifiquen, evalúen y gestionen los riesgos que pueden afectar el logro de sus objetivos.

**Marco del proceso de evaluación de riesgos (5 pasos, iterativo):**
1. Planificar la evaluación (definir alcance, objetivos, roles, requisitos y supuestos).
2. Recopilar información (sobre activos, amenazas, vulnerabilidades y controles existentes).
3. Identificar riesgos (determinar qué puede suceder, cómo y qué controles podrían verse afectados).
4. Analizar riesgos (estima la probabilidad de ocurrencia y el impacto para determinar el nivel de riesgo).
5. Documentar resultados (registra los hallazgos, supuestos, métodos y resultados de la evaluación).

*Proceso iterativo: debe revisarse y actualizarse periódicamente.*

**Principios clave:** la evaluación de riesgos es un proceso sistemático e iterativo; debe estar alineada con los objetivos de la organización; considera amenazas, vulnerabilidades e impacto; proporciona información para decisiones sobre tratamiento del riesgo; es parte del ciclo continuo de gestión de riesgos.

**Componentes clave del riesgo:** Amenazas (eventos o actores con potencial de causar daño), Vulnerabilidades (debilidades que pueden ser explotadas por una amenaza), Activos (recursos valiosos que la organización debe proteger).

**Fórmula NIST SP 800-30:** Riesgo = Amenaza × Vulnerabilidad × Impacto (el riesgo existe cuando una amenaza aprovecha una vulnerabilidad y afecta un activo, generando un impacto en la organización).

**Análisis cualitativo vs. cuantitativo (resumen del infográfico NIST SP 800-30):**
- Cualitativo: utiliza escalas descriptivas (matriz probabilidad × impacto 1-5).
- Cuantitativo: estima el valor del riesgo en términos monetarios mediante SLE y ALE.

Ejemplo rápido NIST: AV (valor del activo) = $500,000; EF (factor de exposición) = 40% (0.40); ARO (tasa anual de ocurrencia) = 0.5 → SLE = 500,000 × 0.40 = $200,000; ALE = 200,000 × 0.5 = $100,000.

**Referencia del NIST SP 800-30:** se alinea con marcos como MIST 8M, ISO/IEC 27005, ISO 31000 e ISO/IEC 27001.

**Beneficios:** mejora la comprensión de los riesgos que pueden afectar a la organización; apoya la toma de decisiones informadas; ayuda a priorizar recursos de manera efectiva; facilita el cumplimiento de requisitos normativos; fortalece la resiliencia y continuidad del negocio.

### 2. Activos críticos de información de la SCM (Supply Chain Management)

**¿Qué es un activo?** Es cualquier recurso que posee valor para la organización y cuya pérdida, alteración o indisponibilidad puede afectar el cumplimiento de sus objetivos.

**Activos críticos de la información en cadenas de suministro (SCM):**
1. **Datos de clientes:** información personal y financiera (identificación, contacto, pago, historial de compras).
2. **Información de inventario:** esencial para el funcionamiento de la cadena de suministros; su interrupción afecta la capacidad de entrega.
3. **Propiedad intelectual:** patentes, marcas registradas, diseños, secretos comerciales.
4. **Información financiera:** ingresos, gastos, cuentas bancarias, transacciones; usada para fraude/extorsión si se compromete.
5. **Información de proveedores:** contratos y acuerdos comerciales; su interrupción afecta entregas a tiempo.
6. **Información de empleados:** personal, contacto, pago, registros de empleo, historial de salud.

**Tabla de Activos de Información de SCM (ejemplo referencial):**

| Activo de información | Descripción | Ubicación física/virtual | Responsable | Nivel de confidencialidad | Riesgos y amenazas |
|---|---|---|---|---|---|
| Datos de clientes | Nombres, direcciones, teléfonos, correos, historial de compras | Base de datos | Ventas y marketing | Alta | Acceso no autorizado, robo de datos, phishing, malware |
| Diseños de productos | Planos y diseños | Servidor de diseño | Ingeniería | Muy alta | Acceso no autorizado, robo de propiedad intelectual, malware |
| Información financiera | Ingresos, gastos, cuentas, transacciones | Software de contabilidad | Finanzas | Muy alta | Fraude, robo de datos, phishing |
| Información de proveedores | Datos personales/financieros, contratos | Base de datos de proveedores | Compras | Alta | Acceso no autorizado, robo de datos, phishing |
| Contratos y acuerdos comerciales | Contratos, confidencialidad, documentos legales | Repositorio de documentos | Legal | Muy alta | Acceso no autorizado, robo de propiedad intelectual |
| Planes de producción | Planes y estrategias de fabricación | Servidor de planificación | Operaciones | Muy alta | Acceso no autorizado, robo de propiedad intelectual, malware |

**Tabla Tipo de Activos de Información de SCM (ejemplo referencial):**

| Tipo de activo | Activo de información | Descripción | Ubicación | Responsable | Confidencialidad | Riesgos y amenazas |
|---|---|---|---|---|---|---|
| Hardware | Servidores | Servicios de red y almacenamiento | Sala de servidores | Equipo de TI | Muy alta | Robo, daño, pérdida de datos, interrupción del servicio |
| Hardware | Dispositivos móviles | Smartphones, tabletas | En posesión del usuario | Usuarios | Alta | Pérdida, robo, acceso no autorizado, malware |
| Hardware | Equipos de red | Routers, switches | Sala de servidores | Equipo de TI | Alta | Acceso no autorizado, mala configuración, interrupción |
| Software | Sistemas operativos | Controlan hardware | Computadoras/servidores | Equipo de TI | Muy alta | Vulnerabilidades, malware, acceso no autorizado |
| Software | Aplicaciones de negocio | Finanzas, RRHH, producción | Computadoras/servidores | Departamentos específicos | Alta | Acceso no autorizado, vulnerabilidades, interrupción |
| Software | Herramientas de colaboración | Correo, mensajería, videoconferencia | Computadoras/móviles | Usuarios | Media | Vulnerabilidades, acceso no autorizado, malware |

**Nivel de Confidencialidad de los Activos de Información:**

| Nivel | Descripción |
|---|---|
| Muy Alta | Compromiso catastrófico: secretos comerciales, propiedad intelectual, datos financieros/investigación, información personal de clientes y empleados. |
| Alta | Compromiso significativo: planes de negocio, estrategias de marketing, planes de producción y operación. |
| Media | Compromiso moderado: correos electrónicos, memorandos, informes, listas de contactos. |
| Baja | Información de dominio público o no confidencial; sin impacto significativo si se compromete. |

*Dinámica grupal:* elaborar inventario de activos de información de la organización identificando criticidad y riesgos asociados (plantilla Excel ESAN Virtual, 10 min).

### 3. Identificación de Amenazas y Vulnerabilidades

**Amenaza:** evento o actor con capacidad para causar daño. Ejemplos: ciberdelincuentes, hacktivistas, empleados maliciosos, errores humanos, desastres naturales.

**Vulnerabilidad:** debilidad que puede ser explotada por una amenaza. Ejemplos: software sin actualizar, contraseñas débiles, falta de MFA, mala configuración cloud, ausencia de backups.

**Relación práctica activo-amenaza-vulnerabilidad:**

| Activo | Amenaza | Vulnerabilidad |
|---|---|---|
| Portal municipal | Ransomware | Sistema sin parches |
| Base de datos tributaria | Robo de datos | Contraseñas débiles |
| Servidor web | Ataque web | Vulnerabilidades OWASP Top 10 |
| Red interna | Movimiento lateral | Ausencia de segmentación |

**Las 10 vulnerabilidades críticas de OWASP (OWASP Top 10):** documento de referencia global de la fundación Open Web Application Security Project (OWASP) sobre las diez vulnerabilidades de seguridad más críticas en aplicaciones web.
1. **Control de acceso roto:** usuarios acceden a funciones/datos fuera de sus permisos.
2. **Fallas criptográficas:** exposición de datos sensibles por falta de cifrado o algoritmos obsoletos.
3. **Inyección:** entrada de datos dañinos (SQL, XSS) ejecutados como comandos válidos.
4. **Diseño inseguro:** defectos desde la arquitectura del código.
5. **Mala configuración de seguridad:** falta de hardening, credenciales por defecto activas.
6. **Componentes vulnerables y obsoletos:** librerías/dependencias desactualizadas con fallas conocidas.
7. **Fallos de identificación y autenticación:** debilidades al validar identidad, robo de sesiones.
8. **Fallas de integridad de datos y software:** pipelines CI/CD sin verificación de legitimidad de actualizaciones.
9. **Fallas en el registro y monitoreo:** incapacidad de detectar/alertar/registrar brechas en tiempo real.
10. **SSRF (Falsificación de solicitudes del lado del servidor):** manipulación para peticiones involuntarias hacia servidores internos/externos.

**Riesgos de los Activos Críticos de la información:**
1. Ciberataques (phishing, malware, ransomware).
2. Robo y pérdida de datos (dispositivos, eliminación accidental, exposición en nube/correo).
3. Interrupciones del servicio (ataques, fallos de hardware, errores humanos).
4. Errores humanos (envío a destinatario equivocado, clic en enlace malicioso).
5. Desastres naturales (inundaciones, terremotos, tormentas que dañan servidores).
6. Amenazas internas (empleados descontentos o ex empleados).

**Tipos de Hackers:** Black hat (habilidades extraordinarias usadas maliciosamente), Grey hat (trabajan ofensiva y defensivamente), White hat (hacker ético / analista de seguridad), Suicide hacker (buscan derribar infraestructura crítica por una causa, sin temor a consecuencias legales).

**Otras amenazas (no solo hackers):** errores humanos en TI, empleados descontentos, competencia desleal, no cumplimiento legal/contractual, falta de Plan de Continuidad, formación insuficiente, falta de medidas técnicas.

### 4. Métodos de Análisis de Riesgos

#### 4.1 Método Cualitativo
Utiliza escalas descriptivas.

| Probabilidad (Valor) | Descripción |
|---|---|
| 1 | Muy Baja |
| 2 | Baja |
| 3 | Media |
| 4 | Alta |
| 5 | Muy Alta |

| Impacto (Valor) | Descripción |
|---|---|
| 1 | Insignificante |
| 2 | Menor |
| 3 | Moderado |
| 4 | Mayor |
| 5 | Crítico |

**Ejemplo:** Riesgo "Ransomware en sistema de pagos municipales": Probabilidad = 4 (Alta), Impacto = 5 (Crítico). Nivel de riesgo = Probabilidad × Impacto = 4×5 = 20 → **Riesgo Muy Alto**.

#### 4.2 Método Cuantitativo
Permite expresar riesgos en términos monetarios.

**SLE (Single Loss Expectancy):** pérdida económica de un incidente individual.
- Fórmula: **SLE = AV × EF**
  - AV = Asset Value (valor del activo)
  - EF = Exposure Factor (porcentaje de pérdida)
- Ejemplo: Valor del sistema = USD 500,000; Impacto estimado = 40% → SLE = 500,000 × 0.40 = **USD 200,000**.

**ALE (Annual Loss Expectancy):** pérdida anual esperada.
- Fórmula: **ALE = SLE × ARO**
  - ARO = Annual Rate of Occurrence (tasa de ocurrencia anual)
- Ejemplo: SLE = USD 200,000; ARO = 0.5 → ALE = 200,000 × 0.5 = **USD 100,000 anuales**.
- Interpretación: si un control cuesta USD 30,000 y reduce significativamente el riesgo, resulta económicamente justificable (análisis costo-beneficio).

### 5. Matriz de Riesgos (Sesión 2)

La matriz de riesgos permite visualizar y priorizar los riesgos según su probabilidad de ocurrencia y su impacto sobre la organización.

| Impacto \ Probabilidad | 1 Muy Baja | 2 Baja | 3 Media | 4 Alta | 5 Muy Alta |
|---|---|---|---|---|---|
| **5 Crítico** | Medio | Alto | Alto | Crítico | Crítico |
| **4 Mayor** | Medio | Medio | Alto | Alto | Crítico |
| **3 Moderado** | Bajo | Medio | Medio | Alto | Alto |
| **2 Menor** | Bajo | Bajo | Medio | Medio | Alto |
| **1 Insignificante** | Bajo | Bajo | Bajo | Medio | Medio |

**Leyenda de niveles de riesgo y acción recomendada:**

| Nivel de Riesgo | Acción recomendada |
|---|---|
| Crítico | Acción inmediata. Implementar controles urgentes y seguimiento permanente. |
| Alto | Elaborar e implementar un plan de tratamiento en el corto plazo. |
| Medio | Monitorear periódicamente y evaluar controles adicionales. |
| Bajo | Aceptar el riesgo y mantener vigilancia básica. |

**Ejemplos de aplicación:**

| Riesgo | Probabilidad | Impacto | Nivel |
|---|---|---|---|
| Ransomware en sistema de pagos municipales | Alta (4) | Crítico (5) | Crítico |
| Phishing a funcionarios públicos | Muy Alta (5) | Moderado (3) | Alto |
| Falla de un servidor secundario | Baja (2) | Menor (2) | Bajo |
| Acceso no autorizado a base de datos tributaria | Media (3) | Crítico (5) | Alto |
| Ataque DDoS a portal institucional | Alta (4) | Mayor (4) | Alto |

### Caso de Discusión Sesión 2: Brecha de Datos en Equifax (2017)

**Antecedentes:** Equifax, una de las principales agencias de información crediticia del mundo, sufrió en 2017 una de las brechas de datos más importantes de la historia.

**Datos del incidente — información comprometida:**
- 147 millones de personas.
- Nombres completos.
- Fechas de nacimiento.
- Números de seguro social.
- Direcciones.
- Información financiera.

**Vulnerabilidad explotada:** Apache Struts (**CVE-2017-5638**). Existía un parche disponible que no fue aplicado oportunamente.

**Impactos:**
- *Financiero:* más de USD 1,400 millones entre multas, litigios, compensaciones y remediación tecnológica.
- *Reputacional:* pérdida de confianza global, renuncia de ejecutivos, investigación del Congreso de EE.UU.
- *Operacional:* programas masivos de respuesta, auditorías de seguridad, transformación de procesos.

### Análisis de Riesgos AMFE (FMEA)

El **AMFE** (Análisis Modal de Fallos y Efectos), internacionalmente **FMEA** (Failure Mode and Effects Analysis), es una metodología preventiva para identificar posibles fallos, evaluar sus efectos y priorizar acciones de mejora antes de que ocurran incidentes. En ciberseguridad resulta útil para analizar vulnerabilidades, amenazas y controles en procesos críticos. Debe ser preparado por un equipo multidisciplinario (diseño, manufactura, ensamble, servicio, calidad, seguridad).

**Componentes del AMFE:**
- **Severity (S) — Gravedad del fallo:** escala 1-10.
- **Occurrence (O) — Probabilidad de ocurrencia:** escala 1-10.
- **Detection (D) — Probabilidad de no detección:** escala 1-10.
- **Número de Prioridad de Riesgo: NPR (RPN) = S × O × D**

**Escala de Severidad (criterio: severidad del impacto):**

| Efecto | Criterio | Escala |
|---|---|---|
| Peligroso: Sin alarma | Riesgo a personas, transgrede regulaciones, falla sin previo aviso | 10 |
| Peligroso: Con alarma | Riesgo a personas, transgrede regulaciones, falla con aviso | 9 |
| Muy Alto | Interrupción grave; 100% de los activos/información podría perderse | 8 |
| Alto | Interrupción importante; información debe revisarse, parte se pierde | 7 |
| Moderado | Interrupción moderada; parte de información se pierde; disconformidad del cliente | 6 |
| Bajo | Interrupción menor; 100% de información debe recuperarse | 5 |
| Muy Bajo | Interrupción menor; información con errores cuestionada por usuarios | 4 |
| Menor | Interrupción menor; errores detectados por el promedio de usuarios | 3 |
| Mucho Menor | Interrupción mínima; distorsión detectada por pocos usuarios | 2 |
| Sin efecto | No afecta el proceso ni la información | 1 |

**Escala de Ocurrencia (Probabilidad de Falla):**

| Probabilidad de Falla | Posibilidad | Cpk | Escala |
|---|---|---|---|
| Muy Alto (falla casi inevitable) | ≥1 en 2 / 1 en 3 | <0.33 / ≥0.33 | 10 / 9 |
| Alto | 1 en 8 / 1 en 20 | ≥0.51 / ≥0.67 | 8 / 7 |
| Moderado | 1 en 80 / 1 en 400 / 1 en 2,000 | ≥0.83 / ≥1.00 / ≥1.17 | 6 / 5 / 4 |
| Bajo | 1 en 15,000 | ≥1.33 | 3 |
| Muy Bajo | 1 en 150,000 | ≥1.5 | 2 |
| Remoto | ≤1 en 1,500,000 | ≥1.67 | 1 |

**Escala de Detección:**

| Nivel de Detección | Probabilidad del test | Escala |
|---|---|---|
| Casi imposible | Detecta <80% de fallas | 10 |
| Muy remoto | Detecta 80% de fallas | 9 |
| Remoto / Muy bajo / Bajo | Detecta <82.5% / <85% / <87.5% | 8 / 7 / 6 |
| Moderado / Mod. Alto | Detecta <90% / <92.5% | 5 / 4 |
| Alto / Muy Alto | Detecta <95% / <97.5% | 3 / 2 |
| Casi Certero | Detecta <99.5% de fallas | 1 |

**Current Process Controls** (tres tipos): a) previenen la causa o reducen su ocurrencia; b) detectan la causa; c) detectan el modo de falla (ej. Poka Yoke — sistema japonés "anti-tonto" para prevenir errores, y sistemas de alarma Andon).

**Potential Causes/Mechanisms of Failure:** causas raíz descritas de forma específica (evitar generalidades). Ejemplos: *Desarrollo* (error de programación, datos errados, deficiente integración); *Infraestructura de TI* (mantenimiento deficiente, desconocimiento, accesos); *Usuario* (deficiente comportamiento de ciberseguridad). Se apoya en Análisis Causa-Efecto / Árbol de Fallas para determinación de causas raíz.

**Recommended Actions / Responsibility / Actions Taken / Resulting RPN:** se priorizan acciones correctivas para los RPN más altos, se asigna responsable, se documentan acciones tomadas y se recalcula el RPN tras la mejora ("empezar a corregir las fallas con los RPN más altos").

**Tabla AMFE de Ciberseguridad (ejemplo aplicado):**

| Proceso / Activo | Modo de fallo (riesgo) | Efecto potencial | Causa potencial | S | O | D | NPR |
|---|---|---|---|---|---|---|---|
| Portal de pagos web | Ataque ransomware | Interrupción del servicio | Software desactualizado | 10 | 6 | 7 | 420 |
| Base de datos tributaria | Robo de información | Fuga de datos personales | Contraseñas débiles | 9 | 7 | 6 | 378 |
| Infraestructura de red | Movimiento lateral | Propagación del ataque | Falta de segmentación | 9 | 6 | 6 | 324 |
| Acceso de funcionarios | Compromiso de credenciales | Acceso no autorizado | Phishing | 8 | 8 | 5 | 320 |
| Centro de datos | Pérdida de información | Imposibilidad de recuperación | Backups insuficientes | 10 | 4 | 8 | 320 |
| Servicios cloud | Exposición de información | Incumplimiento legal | Configuración incorrecta | 8 | 5 | 7 | 280 |

*Dinámica:* desarrollar al menos dos riesgos en plantilla AMFE, calculando el RPN y proponiendo mejora de control (10 min).

### Conclusión de la Sesión 2

1. Para gestionar los riesgos de ciberseguridad, primero es necesario identificar y conocer los activos más importantes de la organización.
2. Los riesgos aparecen cuando una amenaza aprovecha una vulnerabilidad y afecta un activo crítico.
3. El análisis cualitativo y cuantitativo ayuda a comprender mejor los riesgos y a tomar decisiones más informadas.
4. La matriz de riesgos permite priorizar cuáles riesgos requieren atención inmediata y cuáles pueden ser monitoreados.
5. Casos como Equifax demuestran que una vulnerabilidad no gestionada puede generar grandes pérdidas económicas, legales y reputacionales.

*Frase de cierre:* "En un mundo cada vez más digital, el riesgo es inevitable, pero la vulnerabilidad es gestionable. Las organizaciones que identifican, analizan y gestionan sus riesgos de manera proactiva transforman la incertidumbre en una ventaja estratégica."

### Referencias bibliográficas — Sesión 2
- National Institute of Standards and Technology. (2012). *Guide for Conducting Risk Assessments (NIST SP 800-30 Rev. 1)*. U.S. Department of Commerce.
- OWASP Foundation. (2023). *OWASP Risk Rating Methodology*. https://owasp.org/www-community/OWASP_Risk_Rating_Methodology
- National Institute of Standards and Technology. (2023). *Risk Management Framework (RMF)*. https://csrc.nist.gov/projects/risk-management/about-rmf
- ENISA. (2023). *ENISA Threat Landscape 2023*. European Union Agency for Cybersecurity.
- International Organization for Standardization. (2022). *ISO/IEC 27001:2022 Information security, cybersecurity and privacy protection — Information security management systems — Requirements*. ISO.

---

## Sesión 3: Evaluación y Tratamiento de Riesgos

**Logro de aprendizaje:** Al finalizar la sesión, el participante será capaz de evaluar y priorizar riesgos de ciberseguridad, seleccionar estrategias adecuadas de tratamiento y proponer controles alineados a estándares internacionales como **ISO/IEC 27001:2022** y **NIST SP 800-53** para reducir la exposición al riesgo organizacional.

### 1. Introducción

Una vez identificados y analizados los riesgos, el siguiente paso consiste en determinar cuáles requieren atención inmediata y qué acciones deben implementarse para reducirlos a niveles aceptables. La evaluación y tratamiento de riesgos permite responder preguntas fundamentales:
- ¿Qué riesgos son más importantes?
- ¿Qué impacto tendrían sobre la organización?
- ¿Qué controles deben implementarse?
- ¿Cuál es el costo-beneficio del tratamiento?
- ¿Qué riesgos pueden aceptarse?

La finalidad es **reducir el riesgo residual** a niveles compatibles con el apetito y tolerancia al riesgo definidos por la organización.

### 2. Evaluación de Impacto y Probabilidad

**2.1 Impacto** — representa las consecuencias que tendría la materialización de un riesgo.

**Tipos de impacto:**
- *Financiero:* multas regulatorias, costos de recuperación, pérdida de ingresos.
- *Operacional:* interrupción de servicios, paralización de procesos.
- *Reputacional:* pérdida de confianza, daño a la imagen institucional.
- *Legal:* demandas, incumplimiento normativo.
- *Estratégico:* pérdida de ventaja competitiva.

Ejemplo: Riesgo "Fuga de información de estudiantes en una universidad" → impactos posibles: multas por protección de datos, daño reputacional, pérdida de confianza de alumnos, investigaciones regulatorias.

**2.2 Probabilidad** — representa la posibilidad de que el riesgo ocurra.

**Factores que influyen:** historial de incidentes, nivel de exposición, vulnerabilidades existentes, nivel de controles actuales, tendencias de amenazas.

**Escala de Probabilidad:**

| Valor | Probabilidad |
|---|---|
| 1 | Muy Baja |
| 2 | Baja |
| 3 | Media |
| 4 | Alta |
| 5 | Muy Alta |

**Escala de Impacto:**

| Valor | Impacto |
|---|---|
| 1 | Insignificante |
| 2 | Menor |
| 3 | Moderado |
| 4 | Mayor |
| 5 | Crítico |

### 3. Priorización de Riesgos — Matriz de Riesgos

La priorización permite asignar recursos a los riesgos más relevantes.

| Impacto \ Probabilidad | 1 Muy Baja | 2 Baja | 3 Media | 4 Alta | 5 Muy Alta |
|---|---|---|---|---|---|
| **5 Crítico** | Medio | Alto | Alto | Crítico | Crítico |
| **4 Mayor** | Medio | Medio | Alto | Alto | Crítico |
| **3 Moderado** | Bajo | Medio | Medio | Alto | Alto |
| **2 Menor** | Bajo | Bajo | Medio | Medio | Alto |
| **1 Insignificante** | Bajo | Bajo | Bajo | Medio | Medio |

**Leyenda de niveles de riesgo:**

| Nivel de Riesgo | Acción recomendada |
|---|---|
| Crítico | Acción inmediata. Implementar controles urgentes y seguimiento permanente. |
| Alto | Elaborar e implementar un plan de tratamiento en el corto plazo. |
| Medio | Monitorear periódicamente y evaluar controles adicionales. |
| Bajo | Aceptar el riesgo y mantener vigilancia básica. |

**Ejemplos de aplicación:**

| Riesgo | Probabilidad | Impacto | Nivel |
|---|---|---|---|
| Ransomware en sistema de pagos municipales | Alta (4) | Crítico (5) | Crítico |
| Phishing a funcionarios públicos | Muy Alta (5) | Moderado (3) | Alto |
| Falla de un servidor secundario | Baja (2) | Menor (2) | Bajo |
| Acceso no autorizado a base de datos tributaria | Media (3) | Crítico (5) | Alto |
| Ataque DDoS a portal institucional | Alta (4) | Mayor (4) | Alto |

*(Nota: esta matriz es consistente con la presentada en la Sesión 2; se reutiliza como herramienta central de priorización en el ciclo de evaluación).*

### 4. Estrategias de Tratamiento de Riesgos

Según **ISO 31000** e **ISO/IEC 27001**, existen cuatro estrategias principales:

**4.1 Mitigar** — Reducir la probabilidad o impacto mediante controles.
- Ejemplo: Riesgo "Phishing institucional". Controles: MFA, capacitación, filtro antispam. Resultado: disminuye la probabilidad de compromiso.

**4.2 Transferir** — Trasladar parcial o totalmente el impacto financiero a un tercero.
- Ejemplo: seguro de riesgos cibernéticos, servicios cloud con SLA, servicios SOC tercerizados. Resultado: reduce el impacto económico.

**4.3 Evitar** — Eliminar la actividad que genera el riesgo.
- Ejemplo: Riesgo "Uso de software obsoleto sin soporte". Acción: retirar la plataforma. Resultado: el riesgo desaparece.

**4.4 Aceptar** — La organización decide asumir el riesgo.
- Ejemplo: Riesgo "Caída temporal de portal informativo institucional". Impacto: bajo. Costo de mitigación: muy elevado. Resultado: se acepta el riesgo.

### 5. Riesgo Residual

Es el riesgo que permanece después de implementar controles.

**Ejemplo:**
- Antes del tratamiento: Probabilidad = 5, Impacto = 5 → Riesgo = 25.
- Después de implementar MFA, SIEM y monitoreo: Probabilidad = 2, Impacto = 5 → **Riesgo residual = 10**.
- La organización evalúa si dicho nivel es aceptable (según su apetito de riesgo).

### 6. Controles de Seguridad

**6.1 ISO/IEC 27001:2022** — establece controles organizacionales, humanos, físicos y tecnológicos (4 categorías, 93 controles totales: 37 organizativos, 8 de personas, 14 físicos, 34 tecnológicos — detallado en Sesión 1).

**6.2 NIST SP 800-53** — Contiene más de mil controles de seguridad y privacidad.

**Familias relevantes:**

| Familia | Objetivo |
|---|---|
| AC | Access Control |
| IA | Identification and Authentication |
| AU | Audit and Accountability |
| SI | System and Information Integrity |
| IR | Incident Response |
| CP | Contingency Planning |
| RA | Risk Assessment |

Ejemplo de aplicación: Riesgo "Acceso indebido a información académica" → Controles: **AC-2** (Account Management), **IA-2** (MFA), **AU-6** (Log Monitoring).

**Controles propuestos — Diseño de Plan de Tratamiento (Caso: Universidad Nacional Digital):**

| Control | Marco |
|---|---|
| MFA | ISO 27001 / NIST IA-2 |
| DLP | ISO 27001 |
| Capacitación | CIS Control 14 |
| SIEM | NIST AU |
| Backups | ISO 27001 |

**Riesgo identificado:** Fuga de información académica y personal de estudiantes.

| Evaluación | Valor | Riesgo residual | Valor |
|---|---|---|---|
| Probabilidad | 4 | Probabilidad | 2 |
| Impacto | 5 | Impacto | 5 |
| **Riesgo** | **20 (Crítico)** | **Riesgo residual** | **10** |

### Caso de Discusión Sesión 3: Fuga de Datos en Facebook (2019)

**Antecedentes:** En 2019 se reportó la exposición de más de **540 millones de registros** de usuarios de Facebook almacenados en servidores de terceros. Los datos incluían: identificadores de usuarios, nombres, comentarios, reacciones, información de perfiles. La exposición se produjo por **configuraciones inseguras y controles insuficientes** sobre datos compartidos con terceros.

**Impactos:**
- *Reputacional:* pérdida de confianza global.
- *Financiero:* multas regulatorias multimillonarias.
- *Legal:* investigaciones y sanciones.
- *Estratégico:* mayor escrutinio regulatorio.

**Preguntas para discusión y respuestas ideales:**

| Pregunta | Respuesta ideal | Fundamentación |
|---|---|---|
| 1. ¿Qué tipo de riesgo se materializó? | Riesgo de seguridad de la información asociado a la pérdida de confidencialidad de datos personales por exposición masiva. También riesgos reputacionales, legales y regulatorios. | Comprometió información personal de millones de usuarios, afectando el principio de Confidencialidad de la tríada CIA; generó consecuencias legales y pérdida de confianza. |
| 2. ¿Se trató adecuadamente el riesgo? | No. No se implementaron controles suficientes para prevenir/detectar oportunamente la exposición ni se gestionaron adecuadamente los riesgos de terceros. | Una gestión efectiva habría identificado previamente la posibilidad de fuga y establecido controles preventivos y de monitoreo continuo. |
| 3. ¿Qué controles faltaron? | Gestión de accesos, monitoreo continuo, protección de datos, auditorías de seguridad, gestión de terceros y privacidad por diseño. | Debieron limitar el acceso, supervisar el uso de datos y detectar configuraciones inseguras o comportamientos anómalos. |
| 4. ¿Qué controles de ISO/IEC 27001 o NIST SP 800-53 hubieran ayudado? | ISO/IEC 27001: gestión de accesos, gestión de identidades, monitoreo de actividades, protección de datos, gestión de proveedores y respuesta a incidentes. NIST SP 800-53: AC, IA, AU, SI, IR y RA. | Ayudan a limitar accesos no autorizados, proteger datos sensibles, monitorear actividades y responder oportunamente. |
| 5. ¿Qué estrategia de tratamiento debió priorizar Facebook? | Principalmente **Mitigar** (controles técnicos, organizacionales y de monitoreo); complementariamente **Transferir** parte del impacto financiero mediante seguros cibernéticos. | El riesgo no podía evitarse completamente ni aceptarse por su alto impacto; la mejor alternativa era reducir probabilidad e impacto. |

### Conclusiones de la Sesión 3

1. La evaluación de riesgos permite comprender cuáles representan una mayor amenaza para los objetivos de la organización.
2. La combinación de impacto y probabilidad facilita priorizar recursos y esfuerzos de protección.
3. Las estrategias de mitigar, transferir, evitar o aceptar deben seleccionarse según el nivel de riesgo y el contexto organizacional.
4. Los controles de **ISO/IEC 27001**, **NIST SP 800-53** y **CIS Controls** proporcionan mecanismos efectivos para reducir la exposición al riesgo.
5. El objetivo final del tratamiento de riesgos es disminuir el riesgo residual hasta niveles aceptables para la organización.

*Frase de cierre:* "Un riesgo identificado es una preocupación; un riesgo evaluado y tratado es una oportunidad para fortalecer la seguridad y la continuidad del negocio."

### Referencias bibliográficas — Sesión 3
- Center for Internet Security. (2023). *CIS Critical Security Controls v8*. CIS.
- International Organization for Standardization. (2022). *ISO/IEC 27001:2022 Information security, cybersecurity and privacy protection — Information security management systems — Requirements*. ISO.
- National Institute of Standards and Technology. (2020). *Security and Privacy Controls for Information Systems and Organizations (NIST SP 800-53 Rev. 5)*. U.S. Department of Commerce.
- National Institute of Standards and Technology. (2012). *Guide for Conducting Risk Assessments (NIST SP 800-30 Rev. 1)*. U.S. Department of Commerce.
- International Organization for Standardization. (2018). *ISO 31000:2018 Risk management — Guidelines*. ISO.

---

## Sesión 4: Monitoreo, Mejora Continua y Gestión Aplicada

**Logro de aprendizaje:** Al finalizar la sesión, el participante será capaz de monitorear riesgos de ciberseguridad mediante indicadores clave de riesgo (KRI), gestionar incidentes, realizar seguimiento continuo de controles, aplicar procesos de auditoría y mejora continua, e identificar riesgos emergentes asociados a la transformación digital, la computación en la nube, la inteligencia artificial y el Internet de las Cosas (IoT).

### 1. Introducción

La gestión de riesgos no culmina con la implementación de controles. Los riesgos evolucionan constantemente debido a nuevas amenazas, cambios tecnológicos, vulnerabilidades emergentes y transformaciones en el entorno organizacional. Por ello, las organizaciones deben implementar mecanismos permanentes de:
- Monitoreo.
- Medición.
- Auditoría.
- Gestión de incidentes.
- Mejora continua.

El objetivo es garantizar que los riesgos permanezcan dentro de niveles aceptables y que los controles continúen siendo efectivos.

### 2. Indicadores Clave de Riesgo (KRI)

**¿Qué es un KRI?** Un **Key Risk Indicator (KRI)** es una métrica que permite monitorear la evolución de un riesgo y alertar oportunamente sobre posibles desviaciones. Ayuda a responder preguntas como: ¿Está aumentando el riesgo? ¿Los controles están funcionando? ¿Existen señales tempranas de un incidente?

**Características de un buen KRI:** medible, relevante, oportuno, predictivo, fácil de interpretar.

**Ejemplos de KRIs de Ciberseguridad:**

| Riesgo | Indicador (KRI) | Umbral |
|---|---|---|
| Ransomware | % de equipos sin parches críticos | >10% |
| Phishing | Número de usuarios que hacen clic en correos simulados | >15% (o >20 eventos) |
| Fuga de datos | Cantidad de transferencias no autorizadas | >500 por día |
| Accesos indebidos | Intentos fallidos de autenticación | >30 días (acumulado) |
| Vulnerabilidades | Vulnerabilidades críticas abiertas | (umbral según política) |

**Ejemplo práctico — Entidad pública:**
- Objetivo: reducir ataques de phishing.
- KRI: porcentaje de funcionarios que hacen clic en simulaciones de phishing.
- Resultado actual: 20%. Meta: menor a 5%.
- Interpretación: existe una alta exposición al riesgo y se requiere capacitación adicional.

### 3. Monitoreo Continuo

**Definición:** proceso permanente de supervisión de riesgos, amenazas, vulnerabilidades y controles. Permite detectar: actividades sospechosas, incidentes, cambios en el entorno, desviaciones de los indicadores.

**Componentes y herramientas comunes:**

| Componente | Detalle | Herramientas comunes |
|---|---|---|
| Monitoreo de activos | Servidores, redes, aplicaciones | SIEM, SOAR |
| Monitoreo de vulnerabilidades | Escaneos periódicos, gestión de parches | EDR/XDR, Vulnerability Scanners |
| Monitoreo de amenazas | Inteligencia de amenazas, Indicadores de Compromiso (IoC) | Threat Intelligence Platforms |
| Monitoreo de usuarios | Accesos, privilegios, comportamientos anómalos | Dashboards de KRIs, UEBA |

### 4. Auditoría de Seguridad

**Definición:** proceso sistemático para verificar el cumplimiento de políticas, estándares y controles de seguridad.

**Objetivos:** verificar cumplimiento, identificar brechas, evaluar efectividad de controles, detectar oportunidades de mejora.

**Ejemplos por sector:**
- Sector financiero: auditoría de cumplimiento ISO/IEC 27001.
- Sector público: evaluación de cumplimiento de políticas de Gobierno Digital.
- Universidad: auditoría de accesos privilegiados.

**Tipos de auditoría:**
- **Interna:** realizada por la propia organización.
- **Externa:** realizada por terceros independientes.
- **Regulatoria:** realizada por organismos supervisores.

**Principales empresas certificadoras y organismos de evaluación en Seguridad de la Información en el Perú:**

| Empresa Certificadora | País de origen | Certificaciones relacionadas | Presencia en Perú | Sectores atendidos |
|---|---|---|---|---|
| BSI Group | Reino Unido | ISO/IEC 27001, ISO 22301, ISO 9001, ISO 31000 | Sí | Financiero, telecomunicaciones, gobierno, educación |
| DNV | Noruega | ISO/IEC 27001, ISO 22301, ISO 9001 | Sí | Energía, industria, minería, servicios |
| Bureau Veritas | Francia | ISO/IEC 27001, ISO 22301, ISO 20000-1 | Sí | Gobierno, banca, retail, industria |
| SGS | Suiza | ISO/IEC 27001, ISO 22301, ISO 9001 | Sí | Industria, minería, sector público |
| TÜV Rheinland | Alemania | ISO/IEC 27001, ISO 20000-1, ISO 22301 | Sí | Manufactura, telecomunicaciones, TI |
| TÜV SÜD | Alemania | ISO/IEC 27001, ISO 9001, ISO 22301 | Sí | Energía, industria, servicios |
| LRQA | Reino Unido | ISO/IEC 27001, ISO 22301, ISO 9001 | Sí | Logística, transporte, tecnología |
| AENOR | España | ISO/IEC 27001, ENS, ISO 22301 | Sí | Gobierno, banca, educación |
| ICONTEC | Colombia | ISO/IEC 27001, ISO 22301, ISO 9001 | Sí | Sector público y privado |
| Intertek | Reino Unido | ISO/IEC 27001, ISO 22301 | Sí | Tecnología, manufactura, servicios |

### 5. Gestión de Incidentes

**Definición:** proceso para identificar, responder, contener y recuperar operaciones después de un incidente de seguridad.

**Objetivos:** reducir impactos, restablecer operaciones, preservar evidencia, evitar recurrencias.

**Ciclo de Gestión de Incidentes (6 fases):**
1. **Preparación:** políticas, procedimientos, equipos de respuesta.
2. **Detección y análisis:** SIEM, alertas, monitoreo.
3. **Contención:** aislamiento de sistemas, bloqueo de accesos.
4. **Erradicación:** eliminación de malware, corrección de vulnerabilidades.
5. **Recuperación:** restauración de servicios, validación operativa.
6. **Lecciones aprendidas:** análisis post-incidente, mejoras de controles.

**Ejemplo — Ransomware en una entidad pública:**
- Acciones: aislamiento de servidores, activación del CSIRT, restauración desde backups, investigación forense, actualización de controles.

**Ejemplo aplicado al ciclo PDCA — Problema "Aumento de ataques phishing":**
- Plan: capacitación.
- Do: implementación del programa.
- Check: medición del KRI.
- Act: nuevas campañas de concientización.

### 6. Mejora Continua (Ciclo PDCA)

**ISO/IEC 27001** adopta el modelo de mejora continua de Deming (**Ciclo PDCA**):
- **Plan (Planificar):** identificar riesgos, diseñar controles, definir KRIs.
- **Do (Hacer):** implementar controles, ejecutar procedimientos.
- **Check (Verificar):** monitorear indicadores, realizar auditorías.
- **Act (Actuar):** corregir desviaciones, mejorar procesos.

### 7. Riesgos en la Transformación Digital

**7.1 Riesgos en Cloud Computing**
- Amenazas: configuraciones incorrectas, accesos no autorizados, dependencia del proveedor.
- Ejemplo: base de datos expuesta públicamente en AWS.

**7.2 Riesgos en Inteligencia Artificial**
- Amenazas: sesgos algorítmicos, manipulación de modelos, deepfakes, filtración de datos.
- Ejemplo: uso de IA generativa para fraude corporativo mediante suplantación de identidad.

**7.3 Riesgos en IoT**
- Amenazas: dispositivos vulnerables, falta de actualizaciones, acceso remoto no autorizado.
- Ejemplo: ataque a cámaras IP utilizadas en infraestructura crítica.

### 8. Ejemplo de Aplicación: Implementación de KRIs en una Entidad Pública

**Objetivo:** reducir ciberataques dirigidos a funcionarios.

**KRIs definidos y metas:**

| Indicador | Meta |
|---|---|
| Equipos sin parchear | <5% |
| Incidentes de phishing | <3 mensuales |
| Vulnerabilidades críticas abiertas | <10 |
| Usuarios con MFA habilitado | >95% |
| Tiempo de respuesta a incidentes | <4 horas |

**Resultados esperados:** mayor visibilidad del riesgo, detección temprana, mejor toma de decisiones.

### Estructura del Trabajo Final Grupal (presentada en Sesión 4)

**Aplicación de Gestión de Riesgos de Ciberseguridad** — Informe en Word. Fecha de presentación: 24 de junio.

1. Antecedentes de la organización.
2. Identificación de activos de información.
3. Identificación de amenazas y vulnerabilidades.
4. Elaboración de una Matriz de Riesgos.
5. Desarrollo de Indicadores de riesgos (KRIs).
6. Propuestas de controles según marcos de referencia.
7. Conclusiones y Recomendaciones.
8. Bibliografía.

### Caso de Discusión Sesión 4: Incidente de Seguridad en Uber (2022)

**Contexto del caso:** En septiembre de 2022, Uber fue víctima de un incidente de seguridad ampliamente difundido a nivel mundial. El ataque no se produjo mediante una vulnerabilidad técnica compleja, sino a través de una combinación de **ingeniería social, gestión inadecuada de identidades y deficiencias en el monitoreo continuo**.

**Trabajo a realizar:** leer y discutir el caso completo (Esan Virtual), responder las cinco preguntas y presentar en PowerPoint.

**Preguntas para discusión:**
1. Desde la perspectiva del monitoreo continuo, ¿qué señales tempranas debieron haber alertado a la organización antes de que el atacante obtuviera acceso?
2. Analizando el ciclo de gestión de incidentes (Preparación, Detección, Contención, Erradicación, Recuperación y Lecciones Aprendidas), ¿en qué fases identifica mayores debilidades y por qué?
3. Si usted fuera responsable de seguridad (CISO), ¿qué acciones inmediatas y qué acciones de largo plazo implementaría para reducir la probabilidad de un incidente similar?
4. Diseñe al menos cinco KRIs que permitan monitorear el riesgo asociado a robo de credenciales, abuso de MFA y accesos privilegiados (indicando: indicador, fórmula/métrica, umbral de alerta, acción correctiva).
5. Relacionando el caso con **ISO 27001, ISO 31000, NIST CSF 2.0** y **NIST SP 800-53**, ¿qué controles o prácticas de gestión de riesgos hubieran reducido significativamente la probabilidad o el impacto del incidente?

**Respuestas ideales (síntesis del material del curso):**

| Pregunta | Respuesta ideal |
|---|---|
| ¿Qué señales tempranas debieron detectarse? | Múltiples rechazos de MFA, accesos desde ubicaciones inusuales, comportamiento anómalo del usuario, intentos repetitivos de autenticación y alertas no investigadas oportunamente. |
| ¿Qué debilidades existieron en la gestión del incidente? | Deficiencias en preparación, monitoreo, gestión de identidades, revisión de privilegios y seguimiento de hallazgos de auditoría. |
| ¿Qué acciones debieron implementarse? | MFA resistente al phishing, Zero Trust, PAM (Privileged Access Management), monitoreo continuo, capacitación, segmentación de accesos y fortalecimiento del SOC. |
| ¿Qué KRIs hubieran ayudado? | Número de rechazos MFA por usuario, accesos desde ubicaciones anómalas, cuentas privilegiadas sin revisión, tiempo de atención de alertas críticas, porcentaje de alertas investigadas. |
| ¿Qué controles faltaron? | Gestión de identidades y accesos (IAM), gestión de accesos privilegiados (PAM), monitoreo continuo, autenticación adaptativa, auditorías periódicas, gestión de terceros y mejora continua basada en riesgos. |

### Conclusiones de la Sesión 4

1. La gestión de riesgos es un proceso continuo. Identificar, analizar y tratar riesgos no es suficiente; las organizaciones deben monitorearlos constantemente para asegurar que los controles sigan siendo efectivos frente a nuevas amenazas.
2. Los KRIs y el monitoreo ayudan a detectar problemas antes de que ocurran incidentes. Los indicadores permiten identificar señales de alerta temprana y tomar acciones oportunas para reducir la exposición al riesgo.
3. La auditoría y la gestión de incidentes fortalecen la seguridad organizacional. Las auditorías ayudan a encontrar debilidades en los controles, mientras que una adecuada respuesta a incidentes reduce sus impactos y facilita la recuperación.
4. La mejora continua permite adaptar la seguridad a un entorno cambiante. A través del ciclo PDCA, las organizaciones pueden aprender de sus experiencias, corregir errores y fortalecer continuamente sus procesos de ciberseguridad.
5. La transformación digital genera nuevos riesgos que deben gestionarse de forma proactiva. Tecnologías como la nube, la inteligencia artificial y el IoT ofrecen grandes beneficios, pero también introducen amenazas que requieren monitoreo y controles adecuados.

*Frase de cierre:* "La gestión de riesgos de ciberseguridad no termina con la implementación de controles. Su verdadero valor está en la capacidad de la organización para monitorear, aprender y mejorar continuamente, fortaleciendo su resiliencia frente a un entorno digital en constante evolución."

### Referencias bibliográficas — Sesión 4

No se listó una sección bibliográfica diferenciada adicional en las diapositivas; la sesión remite a las referencias generales de marcos ya citadas en sesiones anteriores (ISO 31000, ISO/IEC 27001:2022, NIST SP 800-53, NIST SP 800-30, CIS Controls v8) y a un video complementario: "Análisis de Riesgos Globales 2026: Geopolítica, IA, economía y ciberseguridad" (referenciado al cierre de la Sesión 3, enlazado temáticamente con los riesgos emergentes de la Sesión 4).

---

## Síntesis Integradora del Curso

El curso "Gestión de Riesgos de la Ciberseguridad" sigue de manera explícita el **ciclo de gestión de riesgos de ISO 31000** (Establecimiento del contexto → Identificación → Análisis → Evaluación → Tratamiento → Monitoreo y revisión), distribuido a lo largo de las cuatro sesiones:

**Sesión 1 — Fundamentos (Contexto):** establece el vocabulario y marco conceptual común: qué es un activo, una amenaza, una vulnerabilidad y un riesgo (Riesgo = Amenaza × Vulnerabilidad × Impacto, o Impacto × Frecuencia × Detección). Presenta el panorama de amenazas globales y locales (Perú), introduce los marcos de referencia macro (ISO 31000, ISO/IEC 27001:2022, NIST RMF, NIST CSF 2.0) y posiciona la gestión de riesgos como eje integrador entre seguridad de la información y continuidad del negocio. El caso de los hospitales COVID-19 ilustra cómo una cadena amenaza→vulnerabilidad→activo desemboca en impacto multimillonario.

**Sesión 2 — Identificación y Análisis:** opera el primer tramo del ciclo ISO 31000 aplicando el marco operativo de **NIST SP 800-30**. Aquí se construye el inventario de activos (con niveles de confidencialidad), se catalogan amenazas y vulnerabilidades (incluyendo el **OWASP Top 10**), y se introduce el doble enfoque de análisis: **cualitativo** (matriz Probabilidad × Impacto 1-5) y **cuantitativo** (SLE, ALE). Se añade el método **AMFE/FMEA** (con su Número de Prioridad de Riesgo, NPR = S×O×D) como herramienta complementaria de análisis causa-raíz. El caso Equifax (2017) ejemplifica cómo una vulnerabilidad técnica conocida y no parcheada (CVE-2017-5638) se traduce en pérdida financiera, legal y reputacional.

**Sesión 3 — Evaluación y Tratamiento:** continúa el ciclo con la priorización formal mediante la **matriz de riesgos** (idéntica estructura a la de la Sesión 2, reutilizada como herramienta transversal) y profundiza en los **tipos de impacto** (financiero, operacional, reputacional, legal, estratégico). Introduce las **cuatro estrategias de tratamiento según ISO 31000/ISO 27001**: Mitigar, Transferir, Evitar, Aceptar; y el concepto de **riesgo residual**. Aterriza los controles en dos marcos operativos concretos: **ISO/IEC 27001:2022** (controles organizacionales/humanos/físicos/tecnológicos) y **NIST SP 800-53** (familias AC, IA, AU, SI, IR, CP, RA), más una referencia a **CIS Controls v8**. El caso Facebook (2019) muestra una fuga de 540M de registros por controles de terceros insuficientes, resuelta idealmente con estrategia de Mitigar + Transferir.

**Sesión 4 — Monitoreo y Mejora Continua:** cierra el ciclo ISO 31000 con el monitoreo y revisión permanente, operacionalizado mediante **KRIs (Key Risk Indicators)**, el **monitoreo continuo** (SIEM, SOAR, EDR/XDR), la **auditoría de seguridad** (interna/externa/regulatoria, con mapeo de certificadoras ISO 27001 activas en Perú), la **gestión de incidentes** (ciclo de 6 fases) y el **ciclo PDCA de Deming** adoptado por ISO/IEC 27001 para la mejora continua. Añade una capa prospectiva de riesgos emergentes (cloud, IA, IoT) y cierra con el caso Uber (2022), que combina ingeniería social, fallas de MFA/IAM y debilidades de monitoreo — sirviendo de plantilla directa para el Trabajo Final.

**Hilo conductor:** un mismo riesgo recorre las cuatro sesiones como ejemplo recurrente (ransomware en sistemas de pagos municipales, phishing institucional) demostrando la trazabilidad completa: se **identifica** el activo y la amenaza/vulnerabilidad (Sesión 2), se **evalúa** su nivel en la matriz y se **trata** con una estrategia y controles concretos (Sesión 3), y finalmente se **monitorea** su evolución mediante KRIs y se **audita** la efectividad de los controles implementados (Sesión 4), retroalimentando el ciclo (PDCA) hacia una nueva iteración de identificación de riesgos residuales o emergentes. Los marcos normativos (ISO 31000, ISO/IEC 27001:2022, ISO/IEC 27005 implícito en la pirámide de la Sesión 1, NIST SP 800-30, NIST SP 800-53, NIST CSF 2.0, OWASP Top 10, CIS Controls v8, AMFE/FMEA) no son alternativas excluyentes sino piezas complementarias de un mismo sistema de gestión, cuya integración y nivel de madurez deben adaptarse al contexto específico de cada organización — principio que el Trabajo Final aplica directamente a un caso real (estructura de 8 secciones: antecedentes, activos, amenazas/vulnerabilidades, matriz de riesgos, KRIs, controles, conclusiones, bibliografía).
