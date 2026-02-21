# OpenAI





Aquí está el análisis completo:

***

## Análisis de la Estrategia de AI Responsable de OpenAI

***

### 1. Principios fundamentales y evolución

OpenAI presenta el caso más singular y controvertido de gobernanza de AI responsable entre los cuatro proveedores analizados, por una razón estructural: es la única organización cuya **misión fundacional es explícitamente la seguridad de AGI**, no el servicio a clientes o el retorno a accionistas, lo que crea tensiones institucionales únicas.

La OpenAI Charter, documento fundacional publicado en 2018, establece que la misión es garantizar que la AGI —sistemas altamente autónomos que superen a los humanos en la mayoría del trabajo económicamente valioso— beneficie a toda la humanidad, y compromete a OpenAI a no permitir usos de AI o AGI que dañen a la humanidad o concentren el poder indebidamente.

La evolución del framework operativo pasó por tres momentos críticos. Primero, en **2023**, OpenAI publicó el Preparedness Framework v1, el primer sistema estructurado de evaluación de riesgos para modelos de frontera. Segundo, en **mayo de 2024**, en respuesta a la salida de Ilya Sutskever, Jan Leike y otros investigadores de seguridad que criticaron públicamente la cultura de safety, OpenAI creó el Safety and Security Committee a nivel de Board. Tercero, en **abril de 2025**, publicó el **Preparedness Framework v2**, con criterios más precisos para capacidades de alto riesgo y un nuevo mecanismo de Safeguards Reports.

El 12 de febrero de 2025, OpenAI también expandió significativamente su Model Spec de 10 a 63 páginas, enfatizando tres principios: customizability, transparency e intellectual freedom, con el objetivo de guiar a los modelos a relacionarse con temas sensibles con verdad mientras mantienen estándares éticos.

**URLs oficiales verificadas:**

* OpenAI Charter: https://openai.com/charter/
* Safety & Responsibility hub: https://openai.com/safety/
* Preparedness Framework v2 (PDF): https://cdn.openai.com/pdf/18a02b5d-6b67-4cec-ab64-68cdfbddebcd/preparedness-framework-v2.pdf
* Model Spec (2025): https://model-spec.openai.com/2025-12-18.html

***

### 2. Componentes de la declaración de AI Responsable

La arquitectura documental de OpenAI es la más extensa y técnicamente detallada de los cuatro proveedores, pero también la más fragmentada. Sus componentes principales son:

**Capa estratégica:** La Charter (misión y principios AGI) y los Core Safety Principles (guías de alto nivel sobre beneficio humano, evitar daño concentrado de poder y operar con honestidad).

**Capa operativa de modelos:** El **Preparedness Framework v2** que define umbrales de capacidad High y Critical para cuatro dominios de riesgo severo: CBRN (armas químicas/biológicas/radiológicas/nucleares), Ciberseguridad, Influencia a escala y Autonomía de modelos. El Safety Advisory Group (SAG), grupo cross-funcional interno, supervisa el framework y realiza recomendaciones expertas sobre el nivel y tipo de salvaguardas requeridas para desplegar capacidades de frontera de forma segura. OpenAI Leadership aprueba o rechaza esas recomendaciones, y el Safety and Security Committee del Board ejerce oversight.

**Capa de comportamiento de modelos:** El **Model Spec**, publicado bajo licencia Creative Commons CC0, que define cómo los modelos deben comportarse, priorizar instrucciones y manejar situaciones límite.

**Capa de uso:** Las **Usage Policies** (actualizadas octubre 2025) y el **Code of Conduct** para APIs.

**URLs oficiales:**

* Core Safety Principles: https://openai.com/safety/
* Usage Policies: https://openai.com/policies/usage-policies/
* Preparedness Framework (actualización): https://openai.com/index/updating-our-preparedness-framework/

***

### 3. Procesos y estructura de gobernanza

La gobernanza de OpenAI atravesó su mayor crisis en noviembre de 2023 (destitución y restitución de Sam Altman) y ha sido restructurada desde entonces de forma significativa. La arquitectura actual opera en tres niveles:

**Nivel 1 — Board of Directors con Safety and Security Committee (SSC):** El SSC se convirtió en un comité independiente de oversight del Board, presidido por Zico Kolter (director del departamento de machine learning de Carnegie Mellon). El Board, con el SSC, ejerce oversight sobre los lanzamientos de modelos e incluye autoridad para retrasar un release hasta que se resuelvan preocupaciones de seguridad. Otros miembros del SSC incluyen el ex-Jefe de la NSA, General Paul Nakasone, y la ex-counsel general de Sony, Nicole Seligman.

**Nivel 2 — Safety Advisory Group (SAG):** Cuerpo interno cross-funcional que revisa capability reports y hace recomendaciones pre-despliegue. Es el equivalente más cercano al AETHER Committee de Microsoft o al RSC de Google DeepMind, pero sin la historia de décadas de esos cuerpos.

**Nivel 3 — Equipos técnicos de safety:** Incluyendo el equipo de Preparedness (evaluaciones de modelos), el Red Team interno y el Red Teaming Network (evaluadores externos). El SAG cross-funcional revisa los capability reports de modelos y hace recomendaciones previas al despliegue. Company leadership toma las decisiones finales, con el Board of Directors ejerciendo oversight sobre esas decisiones.

**Contexto crítico de gobernanza:** La turbulencia de 2024 incluyó la disolución del equipo de Superalignment, la salida de Ilya Sutskever y Jan Leike (quien escribió públicamente que la cultura de safety había quedado en segundo plano frente a "productos brillantes"), y una carta abierta de empleados actuales y ex-empleados señalando ausencia de protecciones para whistleblowers. Estas fricciones públicas no tienen equivalente en Microsoft, Google o AWS, y son un factor relevante para organizaciones que evalúan el riesgo reputacional de la adopción.

***

### 4. Alcance en el ciclo de vida de AI

El Preparedness Framework v2 define el proceso pre-despliegue con mayor granularidad técnica que cualquier otro proveedor. Los modelos reciben ratings de capacidad (Low, Medium, High, Critical) en cada dominio de riesgo. OpenAI introdujo los Safeguards Reports como complemento a los Capabilities Reports: mientras estos evalúan si un modelo cruzó un umbral de riesgo, los Safeguards Reports detallan cómo se diseñarán salvaguardas robustas y se verificará su efectividad, consistente con el principio de defense in depth.

Antes de cada lanzamiento público, los modelos pasan por: evaluación interna con el SAG, red teaming interno + Red Teaming Network externo, revisión del SSC para modelos de frontera, y publicación de System Cards con evaluaciones de seguridad. Post-despliegue, OpenAI mantiene monitoreo continuo y publica un **Safety Evals Hub** con resultados de evaluación pública de modelos.

***

### 5. Alcance interno

OpenAI usa sus propios modelos en prácticamente todos los procesos internos (dogfooding total), incluyendo desarrollo de software con Codex/o-series, análisis de políticas, redacción y revisiones de seguridad. El **Model Spec** aplica internamente a cómo los modelos interactúan con empleados de OpenAI igual que con usuarios externos.

Los empleados reciben entrenamiento específico en safety, y el programa de Red Teaming interno actúa como mecanismo de presión continua sobre los modelos antes del lanzamiento. Sin embargo, a diferencia de Microsoft (con decenas de miles de horas de entrenamiento documentadas) o AWS, OpenAI no publica métricas comparables sobre horas de entrenamiento interno en AI responsable.

***

### 6. Políticas de uso y terceros

Las **Usage Policies** (actualizadas octubre 2025) son las más explícitas en prohibiciones concretas de los cuatro proveedores. Las categorías de uso prohibido incluyen:

* Armas de destrucción masiva (biológicas, químicas, nucleares, radiológicas)
* CSAM de cualquier tipo
* Actividades de influencia política encubierta y desinformación electoral
* Identificación biométrica en tiempo real en espacios públicos
* Bases de datos de reconocimiento facial sin consentimiento, uso de la imagen o voz de alguien sin su consentimiento, y automatización de decisiones de alto riesgo en áreas sensibles sin revisión humana.

**Postura sobre decisiones de alto riesgo:** OpenAI es el único de los cuatro proveedores que **prohíbe explícitamente en sus Usage Policies** la automatización de decisiones de alto riesgo sin revisión humana, lo que lo posiciona como el más restrictivo en este aspecto frente a Google (que lo permite con supervisión) y AWS (que lo recomienda pero no lo exige).

**URL oficial:** https://openai.com/policies/usage-policies/

***

### 7. Alcance en ecosistema externo

Para clientes B2B enterprise, OpenAI ofrece herramientas de gobernanza más limitadas que AWS o Google. El ecosistema técnico incluye: **System Cards** por modelo (documentación de capacidades, limitaciones y evaluaciones de safety), **Safety Evals Hub** (resultados públicos de evaluaciones), y **Operator-level controls** en la API para que los deployers configuren comportamiento del modelo mediante system prompts y controles de contenido.

OpenAI tiene una orientación más centrada en el **modelo como artefacto** que en herramientas de gobernanza para el cliente. No dispone de un equivalente a Bedrock Guardrails de AWS, el Responsible AI Dashboard de Azure, o el ecosistema Vertex AI de Google para que los clientes implementen gobernanza en sus propias aplicaciones. Esta brecha es significativa para arquitectos de soluciones enterprise.

Para clientes en la UE, OpenAI espera que sus clientes cumplan con los requerimientos legales aplicables, incluyendo evitar actividades prohibidas bajo el EU AI Act, ya que como proveedor de tecnología GPAI tiene controles técnicos pero también espera compliance activo del deployer.

***

### 8. Recomendaciones para Centro de Excelencia de AI

OpenAI no publica guías específicas comparables a los "10 Tips" de Google Cloud o el Well-Architected Responsible AI Lens de AWS. Su orientación para COEs enterprise se centra en la documentación de modelos (System Cards, Model Spec) y las Usage Policies como punto de partida para políticas internas.

La guía más práctica disponible son las **Best Practices for Deploying AI safely** en la documentación de la API y el **Model Spec** como referencia para definir comportamientos aceptables. Para agentes AI, OpenAI recomienda sandboxing de agentes y acceso configurable a red (como se documenta en el System Card de GPT-5-Codex), pero sin el nivel de detalle operativo de AWS o Google.

**URLs útiles:**

* Safety best practices: https://platform.openai.com/docs/guides/safety-best-practices
* System Cards: https://openai.com/research/system-card/

***

### 9. Nuevos roles organizacionales

OpenAI no tiene un "Chief Responsible AI Officer" con designación pública consolidada. Los roles de safety más visibles son el Director del Safety Advisory Group y los responsables del equipo de Preparedness. La turbulencia organizacional de 2024-2025 (disolución del equipo de Superalignment, reconstitución del Board, reasignación de responsables de safety) hace que el mapa de roles sea menos estable que en los otros tres proveedores.

Para clientes, OpenAI recomienda implícitamente a través de sus políticas la designación de un responsable de AI governance con capacidad de revisar system prompts y usage policy compliance, pero sin la guía estructurada que ofrecen Microsoft, Google o AWS para construir COEs.

La distinción clave entre OpenAI y los demás: su accountability de safety se concentra más en el **Board of Directors** (con poder de veto formal sobre lanzamientos) que en un ejecutivo designado, lo que puede ser percibido como más robusto estructuralmente o como más difuso operacionalmente según el observador.

***

### 10. Cumplimiento regulatorio

OpenAI es signatario del **EU AI Code of Practice** (enero 2025) y participó activamente en la elaboración del Code of Practice for General Purpose AI, cuyas obligaciones para GPAI tomaron efecto en agosto de 2025. OpenAI participó activamente en la implementación del texto tomando parte en la elaboración del Code of Practice para GPAI, y publicó una guía de referencia sobre el EU AI Act que incluye una actualización de julio de 2025 sobre cómo está abordando la entrada en vigor de las disposiciones aplicables a modelos GPAI.

OpenAI no tiene certificación ISO/IEC 42001 documentada públicamente, a diferencia de Microsoft (certificación corporativa) y AWS (certificación por servicio). Para el mercado estadounidense, OpenAI colabora con los AI Safety Institutes de EE.UU. y UK, con Los Alamos National Labs en bioseguridad, y es signatario de los compromisos voluntarios de la Casa Blanca.

**URL oficial:** https://openai.com/global-affairs/a-primer-on-the-eu-ai-act/

***

### 11. Monitoreo de regulaciones

OpenAI tiene un equipo de Global Affairs dedicado que monitorea desarrollos regulatorios y publica análisis sobre marcos como el EU AI Act, el National Security Memorandum de EE.UU. y otros. OpenAI considera que EE.UU. y las compañías democráticas tienen la oportunidad de liderar el establecimiento de normas sobre cómo AI se usa de forma segura y responsable en contextos de seguridad nacional, y busca establecer esas normas con transparencia y cuidado.

La documentación de monitoreo regulatorio más visible son los blog posts de Global Affairs y los análisis específicos de marcos regulatorios, pero sin el nivel de engagement institucional continuo de Microsoft (con 33 Transparency Notes publicadas desde 2019) o Google (con equipos dedicados ante reguladores en cada región).

***

### 12. Colaboración con organismos externos

| Organización                               | Rol de OpenAI                                         |
| ------------------------------------------ | ----------------------------------------------------- |
| **Frontier Model Forum**                   | Co-fundador (con Google, Microsoft, Anthropic)        |
| **Partnership on AI**                      | Miembro activo                                        |
| **C2PA / Content Authenticity Initiative** | Miembro del steering committee                        |
| **EU AI Code of Practice**                 | Signatario y participante activo en elaboración       |
| **US AI Safety Institute**                 | Partnership de investigación y evaluación de modelos  |
| **UK AI Safety Institute**                 | Acuerdos para investigación de seguridad y estándares |
| **Los Alamos National Labs**               | Partnership en bioseguridad                           |
| **MLCommons**                              | Participante en benchmarks de seguridad               |
| **White House voluntary commitments**      | Signatario (2023, renovado 2024)                      |
| **AI Seoul Summit Commitments**            | Signatario de Frontier AI Safety Commitments          |

***

### 13. Relación con Privacidad y Seguridad

OpenAI integra los tres dominios principalmente a través del **Model Spec** y las **Usage Policies**, que tratan privacidad y seguridad como restricciones de comportamiento del modelo más que como dimensiones de arquitectura de sistemas (como hace AWS) o frameworks corporativos separados (como hace Microsoft con el SAIF). Las salvaguardas específicas incluyen: prohibición de bases de datos de reconocimiento facial sin consentimiento, protecciones contra exfiltración de datos en agentes, Prompt Shields contra jailbreak (vía partnership con Microsoft Azure OpenAI), y C2PA metadata en imágenes generadas por DALL-E.

Para enterprise, la privacidad de datos de clientes está gobernada contractualmente: los datos de API no se usan para entrenar modelos por defecto (opt-in requerido), con controles de retención de datos configurables por el cliente.

***

### Recursos oficiales consolidados

| Recurso                            | URL                                                               |
| ---------------------------------- | ----------------------------------------------------------------- |
| Safety & Responsibility hub        | https://openai.com/safety/                                        |
| OpenAI Charter                     | https://openai.com/charter/                                       |
| Model Spec (diciembre 2025)        | https://model-spec.openai.com/2025-12-18.html                     |
| Preparedness Framework v2          | https://openai.com/index/updating-our-preparedness-framework/     |
| Usage Policies                     | https://openai.com/policies/usage-policies/                       |
| Safety Evals Hub                   | https://openai.com/safety/evaluations/                            |
| Safety & Security Committee update | https://openai.com/index/update-on-safety-and-security-practices/ |
| EU AI Act primer                   | https://openai.com/global-affairs/a-primer-on-the-eu-ai-act/      |
| System Cards (catálogo)            | https://openai.com/research/system-card/                          |
| Safety best practices (API)        | https://platform.openai.com/docs/guides/safety-best-practices     |

***

### Conclusión

OpenAI es el proveedor con el perfil de AI Responsable más polarizante del mercado, con fortalezas y debilidades que no tienen equivalente en Microsoft, Google ni AWS.

Sus **tres diferenciadores positivos** son: primero, el **Preparedness Framework v2** es el sistema de evaluación de riesgos de modelos de frontera más técnicamente riguroso y públicamente detallado de la industria, con umbrales de capacidad definidos, dominios de riesgo explícitos y Safeguards Reports auditables. Segundo, el **Model Spec publicado bajo CC0** es el único documento de su tipo en la industria que define el comportamiento esperado de los modelos con granularidad suficiente para uso externo, estableciendo un estándar de transparencia sin precedente. Tercero, las **Usage Policies prohíben explícitamente la automatización de decisiones de alto riesgo sin revisión humana**, siendo la postura más protectora de los cuatro proveedores en este aspecto crítico para sectores regulados.

Sin embargo, para organizaciones en sectores como finanzas, salud o sector público, los **tres puntos de atención críticos** son: primero, la **inestabilidad demostrada de la estructura de safety**: la disolución del equipo de Superalignment, las renuncias de alto perfil con críticas públicas a la cultura de seguridad, y la reconstitución del Board en 2024-2025 crean un riesgo reputacional y operacional sin equivalente entre sus competidores. Segundo, la **ausencia de herramientas de gobernanza enterprise** comparables a Bedrock Guardrails, el Responsible AI Dashboard de Azure o el ecosistema Vertex AI, lo que transfiere más responsabilidad de implementación al cliente sin el tooling de soporte equivalente. Tercero, la **falta de certificación ISO/IEC 42001** documentada, relevante para organizaciones en jurisdicciones donde esta certificación está emergiendo como requisito de due diligence. En síntesis: OpenAI lidera en la rigurosidad técnica de evaluación de sus propios modelos, pero presenta la gobernanza corporativa más volátil y el menor soporte de herramientas enterprise del cuarteto analizado.
