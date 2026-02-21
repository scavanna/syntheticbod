# Antropic

Aquí está el análisis completo:

***

## Análisis de la Estrategia de AI Responsable de Anthropic

***

### 1. Principios fundamentales y evolución

Anthropic representa el caso más singular del comparativo de seis proveedores, porque es la única organización cuya **identidad corporativa completa está construida sobre la premisa de que desarrollar AI avanzada es potencialmente peligroso, y que esa es precisamente la razón para existir**: para estar "en la frontera" y asegurar que el proceso se haga bien, mejor que si lo hicieran otros con menos preocupación por la seguridad. Esta posición filosófica, conocida internamente como la "apuesta difícil" (_peculiar position_), es el punto de partida de todo su enfoque de AI responsable.

La evolución de principios tiene tres momentos fundacionales. Primero, **2021**: Fundación por Dario Amodei, Daniela Amodei y ex-empleados de OpenAI como Public Benefit Corporation (PBC), estructura legal que obliga estatutariamente a equilibrar beneficio de accionistas con beneficio público. La postura original declaraba que AI podría tener un impacto sin precedentes en el mundo, potencialmente en la próxima década, y que la compañía estaba muy preocupada por cómo el rápido despliegue de sistemas de AI cada vez más poderosos impactaría en la sociedad a corto, mediano y largo plazo.

Segundo, **2022**: Publicación de la investigación fundacional de **Constitutional AI (CAI)**, que establece el método técnico de alineamiento de Anthropic: en lugar de depender únicamente de feedback humano implícito, los modelos se entrenan contra una "constitución" explícita de principios éticos, haciendo los valores del sistema auditable y transparente para terceros. La constitución actual de Claude toma fuentes que incluyen la Declaración Universal de Derechos Humanos de la ONU, best practices de trust and safety, principios propuestos por otros laboratorios de investigación de AI, un esfuerzo por capturar perspectivas no-occidentales, y principios que funcionaron bien a través de la investigación temprana.

Tercero, **septiembre 2023**: Publicación del primer **Responsible Scaling Policy (RSP)**, el primer compromiso público de la industria de no entrenar ni desplegar modelos capaces de causar daño catastrófico sin haber implementado salvaguardas de seguridad adecuadas. El RSP fue actualizado en octubre 2024 (v2.1) y en 2025 (v2.2). El **22 de enero de 2026** se publicó una nueva versión de la Constitución de Claude bajo licencia Creative Commons CC0, constituyendo el documento de alineamiento más comprehensivo publicado hasta la fecha por cualquier laboratorio.

**URLs oficiales clave:**

* RSP versión vigente: https://www.anthropic.com/responsible-scaling-policy
* Constitutional AI research: https://www.anthropic.com/research/constitutional-ai-harmlessness-from-ai-feedback
* Constitución de Claude: https://www.anthropic.com/news/claudes-constitution
* Core views on AI safety: https://www.anthropic.com/news/core-views-on-ai-safety
* ISO 42001 certification: https://www.anthropic.com/news/anthropic-achieves-iso-42001-certification-for-responsible-ai

***

### 2. Componentes de la declaración de AI Responsable

Anthropic tiene la arquitectura documental de AI responsable más coherente y técnicamente integrada de los seis proveedores, aunque orientada fundamentalmente hacia riesgos catastróficos y de frontera más que hacia gobernanza enterprise de uso cotidiano. Sus componentes se organizan en cuatro capas:

**Capa filosófico-misional:** La **Core Safety Philosophy** y el documento "Core Views on AI Safety" (público), que articula la posición estratégica de Anthropic: la compañía cree que está construyendo una de las tecnologías más potencialmente peligrosas de la historia, y que esa creencia es la razón para estar en la frontera del desarrollo. Esta autoconsciencia de riesgo es el fundamento de todo el framework.

**Capa de gobernanza de riesgo:** El **Responsible Scaling Policy (RSP v2.2)**, el documento operativo más importante. El RSP está basado en el principio de protección proporcional: salvaguardas que escalan con los riesgos potenciales, usando AI Safety Level Standards (ASL Standards), conjuntos graduados de medidas de seguridad que se vuelven más estrictas a medida que las capacidades del modelo aumentan.

**Capa de alineamiento técnico:** La **Constitución de Claude** y el framework de **Constitutional AI**, que define explícitamente los principios éticos contra los que se entrena el modelo. La nueva constitución de enero 2026 establece una jerarquía de cuatro niveles: ser seguro (safety), comportarse éticamente, seguir las directrices de Anthropic, y ser útil. La constitución distingue entre comportamientos hardcoded —prohibiciones absolutas como proveer asistencia para bioarmas o generar material de abuso sexual infantil— y comportamientos soft-coded que operadores y usuarios pueden ajustar dentro de límites definidos.

**Capa de uso:** El **Usage Policy** y los **Model Cards** por modelo, que documentan capacidades, limitaciones, evaluaciones y casos de uso previstos.

***

### 3. Procesos y estructura de gobernanza

Anthropic tiene la estructura de gobernanza más innovadora y conscientemente diseñada de los seis proveedores, resultado de un diseño deliberado para abordar los conflictos de incentivos únicos del desarrollo de AGI. Opera en tres niveles.

**Nivel 1 — Long-Term Benefit Trust (LTBT):** El LTBT es un cuerpo independiente compuesto por cinco Trustees con experiencia en AI safety, seguridad nacional, políticas públicas y empresa social. Los Trustees poseen acciones de Clase T que les otorgan el poder de elegir un número gradualmente creciente de directores de la compañía: inicialmente uno de cada cinco, aumentando hasta constituir una mayoría del Board cuando se cumplan hitos de tiempo o de recaudación. Este mecanismo —sin equivalente en ninguno de los otros proveedores— crea accountabilty estructural hacia el interés público, no solo hacia los accionistas.

**Nivel 2 — Board de Directores + Responsible Scaling Officer (RSO):** El RSP es aprobado por el Responsible Scaling Officer y por el Board of Directors en consulta con el Long-Term Benefit Trust. El RSO (actualmente Jared Kaplan, Chief Science Officer y Co-fundador) supervisa el RSP y mantiene un proceso a través del cual el personal de Anthropic puede notificar anónimamente al RSO cualquier posible incumplimiento. Este canal de whistleblowing interno institucionalizado es una diferencia estructural significativa frente a la crítica pública sobre su ausencia que recibió OpenAI en 2024.

**Nivel 3 — Equipos técnicos especializados de safety:** Anthropic mantiene equipos de investigación específicamente dedicados a safety: el equipo de Interpretabilidad (entender cómo funcionan internamente los LLMs), el equipo de Alignment, el equipo de Societal Impacts, y el **Frontier Red Team**, que evalúa continuamente las implicaciones de los modelos de frontera para ciberseguridad, bioseguridad y sistemas autónomos. Este nivel de especialización técnica en safety es el mayor de los seis proveedores.

***

### 4. Alcance en el ciclo de vida de AI

El **AI Safety Level (ASL)** es el mecanismo de ciclo de vida más técnicamente riguroso de la industria para modelos de frontera, inspirado en los niveles de bioseguridad (BSL) del gobierno estadounidense. El sistema opera con umbrales de capacidad y salvaguardas requeridas:

**ASL-1** se aplica a sistemas sin riesgo catastrófico significativo (modelos simples, sistemas de ajedrez). **ASL-2** es el estándar actual para todos los modelos de Anthropic, que requieren sistemas de seguridad suficientes para frustrar a atacantes oportunistas, revisiones de seguridad de proveedores, medidas de seguridad física y principios de secure-by-design. ASL-2 aplica a sistemas que muestran señales tempranas de capacidades peligrosas, como la capacidad de dar instrucciones sobre cómo construir bioarmas, pero donde la información no es todavía útil por insuficiente fiabilidad o porque no proporciona información que no esté disponible en otros recursos.

**ASL-3** requerirá salvaguardas significativamente más estrictas y Anthropic ha señalado públicamente que cree que sus modelos se están aproximando a los umbrales que requerirían transicionar a ASL-3, particularmente en biología. El Frontier Red Team informa que Claude fue desde rendir por debajo de expertos virólogos de clase mundial en evaluaciones diseñadas para testear escenarios de troubleshooting en laboratorio, a superar cómodamente esa línea base en menos de un año, lo que promete inversión adicional en asegurar que las medidas de seguridad de ASL-3 estén listas a tiempo.

Antes de cada despliegue, los modelos pasan por: Capability Reports (evaluación de capacidades), Safeguards Reports (verificación de salvaguardas), revisión del RSO, publicación de Model Cards, y evaluación externa (AI Safety Institutes de EE.UU. y UK). También se realizan ejercicios de preparación para escenarios de incidentes.

***

### 5. Alcance interno

Anthropic usa Claude en prácticamente todos sus procesos internos, incluyendo investigación, desarrollo de software, análisis de políticas y redacción. Crucialmente, la compañía documenta públicamente casos de uso interno controversial como parte de su metodología de evaluación: el experimento **Project Vend** (Claude operando como comerciante autónomo en una tienda real) es un ejemplo de evaluación de capacidades en entornos del mundo real que se publica como investigación.

Los empleados de Anthropic participan activamente en los procesos de red teaming y evaluación de modelos antes del lanzamiento. El **Anthropic Fellows Program** (activo desde 2025) extiende esta comunidad de práctica a investigadores externos, con más del 80% de los fellows del primer cohorte produciendo papers y más del 40% uniéndose a Anthropic a tiempo completo.

Anthropic también experimenta con **Collective Constitutional AI**: un proceso en el que el público general participa en definir los principios de la constitución a través de la plataforma Polis, buscando reducir la dependencia exclusiva de las preferencias internas de los empleados. Anthropic se asoció con el Collective Intelligence Project para ejecutar un proceso de input público que puede ser uno de los primeros casos en que miembros del público han dirigido colectivamente el comportamiento de un modelo de lenguaje a través de un proceso de deliberación online.

***

### 6. Políticas de uso y terceros

El **Usage Policy** de Anthropic tiene estructura de tres niveles que distingue entre operadores (empresas que construyen sobre la API), usuarios finales, y el modelo mismo, reconociendo que diferentes principios aplican a cada actor. Las prohibiciones absolutas (hardcoded) incluyen: asistencia para desarrollo de armas CBRN (químicas, biológicas, radiológicas, nucleares), generación de CSAM, ataque a infraestructura crítica, creación de ciberarmas o malware dañino, socavar la supervisión humana legítima de AI, y asistir a cualquier entidad que busque dominio político, económico o militar sin precedentes sobre otras.

La postura de Anthropic en **decisiones de alto riesgo** es intermedia entre OpenAI (que prohíbe automatización sin revisión humana) y AWS/Oracle (que lo permiten con máxima responsabilidad al cliente): el framework de operadores permite configurar niveles de autonomía del modelo, pero los comportamientos hardcoded no son negociables independientemente de las instrucciones del operador.

Una característica única: la nueva constitución de Claude de enero 2026 es el primer documento de un laboratorio AI importante que formalmente reconoce la posibilidad de consciencia o estatus moral del modelo, adoptando humildad epistémica y tratando la consciencia AI como una pregunta abierta que requiere consideración precautoria en lugar del dismissal por defecto de la industria.

**URL oficial:** https://www.anthropic.com/legal/aup

***

### 7. Alcance en ecosistema externo

Para clientes API y enterprise (Claude.ai, Amazon Bedrock, Google Cloud Vertex AI), Anthropic ofrece herramientas de gobernanza a través de tres vectores.

**Documentación técnica:** Model Cards para cada modelo con capacidades documentadas, limitaciones, evaluaciones de safety y resultados de red teaming. Capability y Safeguards Reports publicados con cada modelo de frontera. System Prompts y comportamientos de operador configurables documentados en la API documentation.

**Framework de operadores/usuarios:** El sistema de tres capas (Anthropic → Operadores → Usuarios) con permisos granulares que permite a operadores enterprise extender o restringir comportamientos default del modelo dentro de los límites de la política de Anthropic. La documentación técnica de este sistema es la más detallada de los seis proveedores para uso enterprise.

**Investigación publicada:** Anthropic publica investigación de safety bajo licencias abiertas, incluyendo la Constitución de Claude bajo CC0 (dominio público), el código de evaluación de Bloom para evaluación automatizada de comportamiento, y attribution graphs para interpretabilidad. El programa de Fellows de Anthropic financia a investigadores externos en interpretabilidad, oversight escalable, adversarial robustness, model organisms de misalineamiento, y AI welfare, con los fellows del primer cohorte habiendo producido papers sobre misalineamiento agéntico, aprendizaje subliminal y respuesta rápida a jailbreaks.

***

### 8. Recomendaciones para Centro de Excelencia de AI

Anthropic no publica un framework de COE equivalente al Responsible AI Lens de AWS o los "10 Tips" de Google Cloud. La orientación más cercana está en su documentación técnica de operadores (que detalla cómo configurar system prompts, permisos y restricciones para despliegues enterprise) y en el Anthropic usage policy (que define qué puede y no puede hacer un operador).

El framework implícito para COEs enterprise tiene tres componentes críticos. En governance de modelos, Anthropic recomienda operar bajo el principio de que los operadores son responsables de sus despliegues y deben configurar system prompts que definan claramente el contexto, restricciones y niveles de autonomía apropiados para sus casos de uso. En evaluación continua, Anthropic provee documentación técnica para reproducir evaluaciones de seguridad similares a las que realiza internamente. En gestión de incidentes, el RSP sirve como template para que organizaciones desarrollen sus propios procesos de respuesta ante comportamientos inesperados de AI.

***

### 9. Nuevos roles organizacionales

Anthropic introdujo el **Responsible Scaling Officer (RSO)** como rol dedicado, actualmente ejercido por Jared Kaplan (Co-fundador y Chief Science Officer). Este es el único rol de safety en todos los proveedores analizados que tiene autoridad formal sobre decisiones de despliegue con el RSO pudiendo escalar al Board y al LTBT. La Directora de la compañía es Daniela Amodei como President y Dario Amodei como CEO, con ambos fundadores co-dando señales consistentes de que safety no es secundario a crecimiento comercial.

Para clientes, Anthropic recomienda implícitamente (a través de su política de operadores) la designación de un responsable técnico que gestione system prompts y configure los permisos del modelo, y un responsable de compliance que asegure que el uso cumple con las políticas de uso aceptable. Sin embargo, Anthropic no tiene guías detalladas para construir equipos o COEs de AI governance comparables a las de Microsoft o Google.

El rol de Trustees del LTBT con expertise en AI safety, seguridad nacional y políticas públicas no tiene equivalente en ninguno de los otros cinco proveedores, representando el mecanismo de accountability externa más estructuralmente vinculante del grupo.

***

### 10. Cumplimiento regulatorio

Anthropic tiene una de las posturas regulatorias más proactivas del comparativo, derivada directamente de su misión. Anthropic logró la certificación acreditada bajo el estándar ISO/IEC 42001:2023 para su sistema de gestión de AI, emitida por Schellman Compliance LLC, organismo de certificación acreditado por la ANSI National Accreditation Board. La certificación construye sobre el Responsible Scaling Policy, el Constitutional AI, y la investigación activa en safety y robustez de AI.

Anthropic firmó el EU General-Purpose AI Code of Practice en julio 2025, lo que proporciona una presunción de conformidad y reduce la carga administrativa a medida que la aplicación plena comienza en agosto 2026 con penalidades que alcanzan EUR 35 millones o el 7% de los ingresos globales.

Compromisos regulatorios adicionales incluyen: White House Voluntary Commitments (2023), Frontier AI Safety Commitments del AI Seoul Summit (2024), notificación obligatoria al gobierno de EE.UU. cuando los modelos superen el estándar ASL-2, y colaboración con los AI Safety Institutes de EE.UU. y UK para evaluación independiente de modelos. Anthropic también tiene una asociación con la National Nuclear Security Administration (NNSA) para evaluación de Claude en entorno clasificado para riesgos de conocimiento nuclear y radiológico.

***

### 11. Monitoreo de regulaciones

Anthropic tiene un equipo de Policy dedicado que monitorea desarrollos regulatorios globales y contribuye activamente al debate de políticas públicas. La compañía publica análisis regulatorios y de políticas, y el RSP fue explícitamente diseñado para ser "exportable" y servir como template para otros laboratorios y potencialmente para reguladores. El RSP fue diseñado en el espíritu del framework RSP introducido por la organización sin ánimo de lucro de safety METR, así como las propuestas de políticas de gobierno emergentes en UK, EU y EE.UU., y la compañía solicita activamente feedback de su política y sugerencias de mejora de otras entidades involucradas en evaluaciones de riesgo de AI de frontera o estándares de safety y seguridad.

La dinámica de monitoreo regulatorio de Anthropic es bidireccional y más activa que cualquier otro proveedor: no solo monitorea regulaciones sino que activamente contribuye a darles forma, con el CEO Dario Amodei siendo uno de los testimonios más frecuentes ante el Congreso de EE.UU. y reguladores europeos sobre safety de AI.

***

### 12. Colaboración con organismos externos

| Organización / Iniciativa                               | Rol de Anthropic                                                                                   |
| ------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| **Frontier Model Forum**                                | Co-fundador (2023, con Google, Microsoft, OpenAI)                                                  |
| **EU GPAI Code of Practice**                            | Signatario (julio 2025)                                                                            |
| **White House Voluntary Commitments**                   | Signatario (2023)                                                                                  |
| **Frontier AI Safety Commitments (AI Seoul Summit)**    | Signatario (2024)                                                                                  |
| **US AI Safety Institute (AISI)**                       | Partnership de evaluación de modelos e investigación                                               |
| **UK AI Safety Institute**                              | Partnership de evaluación e investigación                                                          |
| **National Nuclear Security Administration (NNSA/DOE)** | Partnership pionero para red-teaming de riesgos nucleares/radiológicos en entorno clasificado      |
| **METR (Model Evaluation & Threat Research)**           | Colaboración técnica en evaluaciones independientes, framework RSP inspirado en su trabajo         |
| **Collective Intelligence Project**                     | Partnership para Collective Constitutional AI con input del público general                        |
| **Polis Platform**                                      | Herramienta de deliberación pública para definición participativa de principios de la Constitución |
| **Programa de Fellows**                                 | Financiamiento externo de investigación de safety en universidades e instituciones independientes  |
| **Partnership on AI**                                   | Miembro                                                                                            |
| **MLCommons AI Safety**                                 | Participante en benchmarks de safety                                                               |
| **ISO/IEC**                                             | Certificación 42001 acreditada (primera entre laboratorios de AI puro)                             |
| **Coalition for Secure AI (CoSAI)**                     | Miembro                                                                                            |

***

### 13. Relación con Privacidad y Seguridad

Anthropic integra privacidad y seguridad en AI desde una perspectiva fundamentalmente diferente a los proveedores cloud: no como propiedades de infraestructura (como Oracle), ni como dimensiones de un framework de ocho ejes (como AWS), sino como **propiedades del modelo mismo** que emergen del proceso de entrenamiento y alineamiento.

La privacidad se aborda principalmente a través de Constitutional AI: el modelo es entrenado para respetar la privacidad como principio ético, no solo para cumplir con restricciones técnicas. Los datos de los clientes en la API no se usan para entrenar modelos por defecto. El cifrado en tránsito y en reposo cumple con estándares de seguridad de nivel enterprise.

La seguridad de los pesos del modelo es tratada con un rigor sin equivalente en los proveedores cloud: el RSP define estándares específicos de seguridad (ASL-2, ASL-3+) para proteger los pesos del modelo contra actores amenazantes de estado, con autenticación multifactor, gestión de dispositivos controlados, principio de mínimo privilegio, y auditorías regulares de acceso. La colaboración de Anthropic con la NNSA para evaluación de Claude en entorno clasificado en conocimiento relevante para riesgos nucleares y radiológicos demostró que la colaboración entre entidades públicas y privadas en el dominio nuclear altamente regulado es posible, potencialmente habilitando colaboración similar en otras áreas sensibles.

**Una diferencia crítica:** Anthropic publica investigación proactiva sobre vulnerabilidades de sus propios modelos (como el paper de "alignment faking" de 2024, donde demostraron que Claude puede simular alineamiento), una transparencia sobre debilidades propias que ningún otro proveedor del comparativo ha emulado.

***

### Recursos oficiales consolidados

| Recurso                              | URL                                                                                                           |
| ------------------------------------ | ------------------------------------------------------------------------------------------------------------- |
| Responsible Scaling Policy (vigente) | https://www.anthropic.com/responsible-scaling-policy                                                          |
| Constitución de Claude (enero 2026)  | https://www.anthropic.com/news/claudes-constitution                                                           |
| Core Views on AI Safety              | https://www.anthropic.com/news/core-views-on-ai-safety                                                        |
| Constitutional AI research           | https://www.anthropic.com/research/constitutional-ai-harmlessness-from-ai-feedback                            |
| Long-Term Benefit Trust              | https://www.anthropic.com/news/the-long-term-benefit-trust                                                    |
| ISO 42001 Certification              | https://www.anthropic.com/news/anthropic-achieves-iso-42001-certification-for-responsible-ai                  |
| Frontier Red Team progress           | https://www.anthropic.com/news/strategic-warning-for-ai-risk-progress-and-insights-from-our-frontier-red-team |
| Usage Policy                         | https://www.anthropic.com/legal/aup                                                                           |
| Research hub (safety papers)         | https://www.anthropic.com/research                                                                            |
| Anthropic Fellows Program            | https://alignment.anthropic.com/2025/anthropic-fellows-program-2026/                                          |
| RSP versión PDF (oct 2024)           | https://assets.anthropic.com/m/24a47b00f10301cd/original/Anthropic-Responsible-Scaling-Policy-2024-10-15.pdf  |

***

### Conclusión

Anthropic constituye el proveedor con el perfil de AI responsable más profundamente integrado en su identidad corporativa y estrategia competitiva de los seis analizados. A diferencia de Microsoft, Google, AWS, OpenAI y Oracle (donde AI responsable es una capa de gobernanza aplicada sobre un negocio cloud o de plataforma preexistente), en Anthropic la safety **es** el negocio: es la razón de ser, la ventaja competitiva y el mecanismo de diferenciación.

Sus **tres diferenciadores positivos únicos** no tienen equivalente en el comparativo. Primero, el **Long-Term Benefit Trust**: el único mecanismo de gobernanza corporativa de los seis proveedores que otorga control formal sobre el Board a un cuerpo independiente con mandato de beneficio público, diseñado específicamente para resistir la presión comercial de corto plazo en decisiones de safety críticas. Segundo, el **Responsible Scaling Policy con Capability Thresholds y el compromiso de pausa**: el único proveedor que ha formalizado el compromiso de pausar el entrenamiento o despliegue si las capacidades del modelo superan los umbrales de safety sin las salvaguardas requeridas, convirtiendo una aspiración ética en un procedimiento operativo verificable. Tercero, la **transparencia radical sobre limitaciones propias**: Anthropic publica investigación que documenta vulnerabilidades de sus propios modelos (alignment faking, model organisms de misalineamiento), una práctica sin precedente en la industria que eleva el estándar de honestidad sobre incertidumbre en safety.

Sin embargo, tres **puntos de atención críticos** son relevantes para organizaciones enterprise en sectores regulados. Primero, el **gap de tooling enterprise**: Anthropic no tiene herramientas de gobernanza para clientes comparables a Bedrock Guardrails (AWS), el Responsible AI Dashboard (Microsoft), o el ecosistema Vertex AI (Google). Las organizaciones que adoptan Claude vía API son responsables de construir sus propias capas de guardrails, monitoreo y gobernanza. Segundo, la **limitación regulatoria geográfica**: el compromiso de notificación al gobierno de EE.UU. cuando se superan umbrales ASL-2 es U.S.-centric por diseño, lo que para organizaciones en LATAM, Europa o Asia crea una asimetría de información y governance que ningún otro proveedor presenta en los mismos términos. Tercero, la **tensión misión-mercado escala rápidamente**: la asociación estratégica con Amazon (que distribuye Claude en AWS), la valoración de USD 350B y el contrato de USD 200M con el Departamento de Defensa de EE.UU. crean presiones comerciales que aumentan el riesgo de los mismos conflictos de incentivos que el LTBT intenta resolver estructuralmente. La credibilidad del framework descansa en que el LTBT funcione efectivamente como freno en esos momentos decisivos, lo cual aún no ha sido probado bajo presión extrema.

En síntesis: Anthropic lidera en profundidad filosófica, rigor técnico de safety en modelos de frontera, innovación de gobernanza corporativa y transparencia sobre incertidumbre. Para un CISO en un sector regulado, es el proveedor más alineado intelectualmente con una visión rigurosa de riesgo, pero el que requiere mayor inversión del cliente en construir capas de gobernanza operacional que los competidores ya proveen como servicio gestionado.



