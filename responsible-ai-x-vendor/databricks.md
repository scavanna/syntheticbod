# Databricks



## Análisis de la Estrategia de AI Responsable de Databricks

***

### Nota metodológica preliminar

Databricks es el duodécimo proveedor del comparativo y el que más obliga a preguntarse qué significa "AI responsable" para un actor que históricamente no es un proveedor de AI sino de **infraestructura de datos y plataforma de ML/datos**. La identidad fundacional de Databricks —los creadores originales de Apache Spark, Delta Lake, MLflow, y el concepto de Data Lakehouse— define la lente a través de la cual entiende AI responsable: no como ética de modelos ni como governance de outputs de modelos de frontera, sino como **gobernanza del ciclo de vida completo de datos y modelos en entornos enterprise**. La adquisición de MosaicML en 2023 por $1.3B añadió una capa genuina de desarrollo de modelos propios (DBRX, los modelos MPT) y atrajo talento de AI research de alto nivel (Jonathan Frankle, autor de la Lottery Ticket Hypothesis, llegó como Chief AI Scientist). Sin embargo, el posicionamiento de Databricks sigue siendo estructuralmente diferente al de un OpenAI, Anthropic, o Google: su campo de batalla es el data+AI stack del enterprise, no la competencia en benchmarks de frontera. Esta distinción es central para interpretar correctamente el perfil de AI responsable de la empresa.

***

### 1. Principios fundamentales y evolución

El corpus de principios de AI responsable de Databricks es relativamente reciente y se articula más como filosofía de producto que como declaración ética autónoma. La trayectoria tiene cinco momentos identificables:

**2013-2022 — Era de plataforma de datos sin frame de AI ética**: Databricks se funda en 2013 por investigadores de UC Berkeley como empresa de datos. Durante este período, la narrativa de responsible AI no existe explícitamente en la comunicación de Databricks, porque el portafolio no incluye modelos de AI sino infraestructura de datos y procesamiento (Spark, Delta Lake, MLflow). La responsabilidad es pensada en términos de data governance, no de AI ethics.

**2023 — Adquisición de MosaicML y giro estratégico**: La adquisición de MosaicML por $1.3B en julio 2023 es el punto de inflexión. Databricks y MosaicML combinaron sus plataformas con la visión de que toda organización puede construir, poseer y asegurar modelos de AI generativa de primer nivel manteniendo el control de sus datos. [Databricks](https://www.databricks.com/company/newsroom/press-releases/databricks-signs-definitive-agreement-acquire-mosaicml-leading-generative-ai-platform) Con MosaicML llegan los modelos MPT, la filosofía de democratización de AI a través de modelos propios y open-source, y el talento de investigación. En el mismo período, Databricks publica sus primeras declaraciones explícitas de "Responsible AI" como marco de principios.

**2023-2024 — Formalización del DASF y postura pública**: Databricks lanza el Databricks AI Security Framework (DASF) v1.0, el primer documento de gobernanza técnica publicado por la empresa con alcance de industria (no solo para sus propios clientes). El DASF fue desarrollado por el equipo de Seguridad y ML de Databricks en asociación con expertos de la industria, bridging la brecha entre equipos de negocio, datos, gobernanza y seguridad. [Databricks](https://www.databricks.com/blog/introducing-databricks-ai-security-framework-dasf) Este marco posiciona a Databricks como actor de gobernanza más allá de su propia plataforma.

**2024 — DBRX y Responsible AI Testing Framework**: En marzo 2024, Databricks lanza DBRX, su LLM propio con arquitectura MoE, y junto con él publica el **Databricks Responsible AI Testing Framework** — el documento más cercano a un model card responsable que Databricks ha publicado. También en 2024, Jonathan Frankle participa como panelista en el FTC Tech Summit sobre AI, siendo el ejecutivo técnico más visible de Databricks en debates de política de AI. Databricks participa como miembro inicial del Consortium de apoyo al USAISI (US AI Safety Institute). [Databricks](https://www.databricks.com/blog/ai-regulation-rolling-out-and-data-intelligence-platform-here-help)

**2025 — DAGF, DASF 2.0 y posicionamiento de gobernanza enterprise**: Databricks lanza el **Databricks AI Governance Framework (DAGF)** como marco comprehensivo de cinco pilares, y actualiza el DASF a la versión 2.0 con 62 riesgos técnicos mapeados a 64 controles recomendados. Con más de 15,000 clientes en diversas geografías y segmentos de mercado, Databricks ha cumplido su compromiso con los principios de desarrollo responsable e innovación open source. [Databricks](https://www.databricks.com/blog/introducing-databricks-ai-governance-framework)

La **filosofía de AI responsable de Databricks** se puede sintetizar en tres proposiciones: (1) La soberanía de datos es la base de la AI responsable — si el cliente controla sus datos, controla los fundamentos de su AI; (2) la AI responsable requiere gobernanza de ciclo de vida completo, no solo de outputs; y (3) el open source es un vector de AI responsable porque democratiza el acceso y permite auditoría externa.

Lo que **no tiene** Databricks que los proveedores más maduros del comparativo sí tienen: no hay un documento maestro de principios de AI ética comparables a los IBM Principles for Trust and Transparency (2018), el Anthropic Core Views, o el Google AI Principles. Los principios de Databricks están distribuidos en blogs, whitepapers técnicos, y páginas de producto — sin un documento fundacional unificado y firmado a nivel ejecutivo.

**URLs oficiales de referencia**: [https://www.databricks.com/trust/responsibleAI](https://www.databricks.com/trust/responsibleAI) | [https://www.databricks.com/blog/introducing-databricks-ai-governance-framework](https://www.databricks.com/blog/introducing-databricks-ai-governance-framework) | [https://www.databricks.com/resources/whitepaper/databricks-ai-security-framework-dasf](https://www.databricks.com/resources/whitepaper/databricks-ai-security-framework-dasf)

***

### 2. Componentes de la declaración de AI Responsable

El corpus documental de AI responsable de Databricks tiene una estructura asimétrica: profundo en el dominio técnico de security y governance operacional, más delgado en el dominio de principios éticos y accountability institucional.

**Databricks AI Governance Framework (DAGF, 2025)**: El documento de mayor alcance de gobernanza de AI que Databricks ha publicado. Organizado en cinco pilares: organización de AI, ética, cumplimiento legal y regulatorio, transparencia e interpretabilidad, operaciones e infraestructura de AI, y seguridad de AI. [Databricks](https://www.databricks.com/dataaisummit/session/building-responsible-and-resilient-ai-databricks-ai-governance) El DAGF es un framework descriptivo-prescriptivo para organizaciones que buscan construir programas de AI governance, no una declaración de principios de Databricks como empresa. Esta distinción es importante: el DAGF instruye a los clientes sobre cómo gobernar su AI, no necesariamente documenta cómo Databricks gobierna la suya.

**Databricks AI Security Framework (DASF 2.0, 2025)**: El documento técnico más maduro del portafolio de AI responsable de Databricks. El DASF 2.0 identifica 62 riesgos técnicos de seguridad mapeados a 64 controles recomendados para gestionar el riesgo de modelos de AI, construyendo sobre estándares existentes para proporcionar un perfil de riesgo end-to-end para despliegues de AI. [Databricks](https://www.databricks.com/blog/announcing-databricks-ai-security-framework-20) El DASF mapea sus riesgos y controles a MITRE ATLAS, OWASP Top 10 for LLMs, NIST AML Taxonomy, ISO, y HITRUST — el trabajo de alineación con frameworks externos de seguridad más completo del comparativo de proveedores de plataforma (aunque IBM tiene mayor alcance en frameworks de governance de negocio). El DASF está disponible como recurso público para cualquier organización, no solo para clientes de Databricks.

**Responsible AI Testing Framework (2024)**: Framework para testing de modelos de AI generativa, diseñado para evaluar modelos antes de su despliegue en cuanto a safety, bias, y calidad. Fue publicado en el contexto del lanzamiento de DBRX y del posicionamiento de Databricks como actor de desarrollo de modelos.

**Página de Responsible AI (databricks.com/trust/responsibleAI)**: La página hub de AI responsable de Databricks, más escueta que las páginas equivalentes de IBM, Microsoft, o Google. Documenta el "point of view" de Databricks sobre AI responsable y enlaza al Responsible AI Testing Framework.

**Databricks AI Assistive Features Trust and Safety documentation**: Documentación técnica específica para las funciones de AI asistidas (Assistant, Genie, AI/BI) que cubre: qué datos se envían a modelos externos, cómo se protegen en tránsito y en reposo, qué controles de residencia de datos existen, y qué garantías de no-uso de datos de clientes para entrenamiento se proveen. Databricks no entrena modelos de fundación generativos con los datos, prompts o respuestas que los clientes envían a estas funciones. Databricks no usa estos datos para generar sugerencias mostradas a otros clientes. [Databricks](https://docs.databricks.com/aws/en/databricks-ai/databricks-ai-trust)

**Lo que el corpus no cubre con profundidad suficiente**: No hay Responsible Scaling Policy, no hay compromisos de frontier safety con umbrales de capacidad documentados, no hay un AI ethics board comparable al IBM Responsible Technology Board o al Google AI Safety Council, y no hay Responsible Use Guide para DBRX con la granularidad del IBM Granite Responsible Use Guide (el Responsible AI Testing Framework es más delgado en disclosure de training data que el Granite Guide). El hecho de que no se hayan revelado las fuentes exactas de datos de entrenamiento de DBRX es una brecha explícitamente señalada por TechCrunch en la cobertura del lanzamiento.

***

### 3. Procesos y estructura de gobernanza

La estructura de gobernanza de AI responsable de Databricks es la menos formalizada del comparativo de proveedores enterprise (junto con xAI, aunque por razones muy diferentes). Esto no significa que Databricks sea irresponsable con su AI — significa que su governance se expresa más en decisiones de arquitectura de producto que en estructuras institucionales documentadas.

**Liderazgo ejecutivo visible**: **Ali Ghodsi** (Co-founder y CEO) hace declaraciones públicas sobre democratización de AI y data sovereignty como principios rectores, aunque con menor frecuencia en el dominio de AI ethics que los CEOs de IBM, Microsoft, o Google. **Jonathan Frankle** (Chief AI Scientist, ex-MosaicML) es el ejecutivo técnico más visible en debates de política de AI — participó en el FTC Tech Summit 2024 como panelista y está vinculado al OECD.AI como experto. **Trâm Phi** (General Counsel) tiene declaraciones públicas sobre el equilibrio entre privacidad, seguridad, y acceso en AI governance. No hay equivalente documentado a un Chief Ethics Officer, Chief Responsible AI Officer, o Chief Trust Officer.

**No hay AI Ethics Board documentado**: A diferencia de IBM (Responsible Technology Board desde 2018), Microsoft (AI for Good Board), o Google (Google AI Safety Council con miembros externos), Databricks no tiene un órgano de gobernanza dedicado a AI ethics con composición y mandato publicados. La gobernanza de AI responsable parece ejercerse principalmente a través de decisiones de arquitectura de producto (Unity Catalog como herramienta de governance, MLflow como herramienta de trazabilidad) y de revisiones técnicas internas del equipo de Seguridad.

**Equipo de Seguridad como actor central de governance**: La parte más madura de la gobernanza de AI de Databricks es ejercida por su equipo de Seguridad, que desarrolló el DASF en colaboración con 15 líderes de seguridad de AI de la industria (incluyendo HITRUST, Carnegie Mellon University, Capital One, Protect AI, y Barracuda). Esta co-creación con actores externos para el DASF es una forma de accountability externo que no tiene equivalente exacto en el comparativo.

**Participación en governance regulatoria**: Databricks participa como miembro fundador del **CAISI (Consortium para el US AI Safety Institute)** y tiene representación en debates regulatorios ante el FTC (Jonathan Frankle) y publicaciones sobre el EU AI Act en el OECD.AI. Esta participación regulatoria es moderada comparada con IBM o Microsoft, pero significativamente mayor que la de actores como xAI o Huawei Cloud.

***

### 4. Alcance en el ciclo de vida de AI

El perfil de cobertura del ciclo de vida de AI de Databricks es el más distintivo del comparativo: está diseñado para cubrir el ciclo de vida de AI de **los clientes de Databricks** más que el ciclo de vida de los modelos propios de Databricks. Esta inversión — ser el proveedor de gobernanza de ciclo de vida más que el desarrollador responsable de modelos — es la característica más definitoria de su postura de AI responsable.

**Pre-entrenamiento (para clientes)**: Unity Catalog provee gobernanza de datos de entrenamiento con linaje, control de acceso, catalogación, y auditoría. Unity Catalog simplifica el cumplimiento al proporcionar un único lugar para gestionar descubrimiento, acceso y auditoría a través de todo el estate de datos, lo que reduce significativamente el riesgo y simplifica las auditorías — permitiendo demostrar qué datos utilizó qué modelo y que los controles apropiados estaban en lugar. [Techfabric](https://www.techfabric.com/blog/dasf---databricks-ai-security-framework)

**Pre-entrenamiento de modelos propios (DBRX)**: El Responsible AI Testing Framework cubre la evaluación pre-lanzamiento de modelos propios. DBRX fue sometido a safety testing y red teaming antes de su lanzamiento, pero las fuentes exactas de datos de entrenamiento no fueron completamente reveladas en el lanzamiento — una brecha de transparencia respecto al estándar establecido por IBM Granite, Meta Llama 3, o Anthropic.

**Evaluación pre-despliegue (herramientas para clientes)**: El Mosaic Eval Gauntlet es la herramienta de benchmarking de evaluación de modelos más completa de la plataforma. Mosaic AI Model Evaluation incluye evaluaciones de calidad de respuestas generativas, groundedness para RAG, y detección de toxicidad. El Responsible AI Testing Framework provee metodología para que organizaciones evalúen sus propios modelos.

**Monitoreo post-despliegue**: Lakehouse Monitoring es la herramienta de monitoreo continuo de modelos en producción de Databricks, con capacidades de detección de drift, monitoreo de calidad de datos, y alertas. MLflow captura toda la trazabilidad de experimentos, versiones de modelos, y linaje de ejecuciones para auditoría completa. Mosaic AI Gateway centraliza el control de los sistemas de AI de las organizaciones, estandarizando el acceso, protegiendo el uso y entregando observabilidad completa a través de todos los modelos y agentes. [Databricks](https://www.databricks.com/product/artificial-intelligence/ai-gateway)

**Trazabilidad de compound AI systems**: Una contribución técnica genuina de Databricks al dominio de AI responsable es su arquitectura de trazabilidad para sistemas de AI compuestos (RAG + LLM + herramientas). Los modelos de AI generativa registrados en MLflow, incluyendo LLMs habilitados con herramientas, pueden ser fácilmente trazados para explicabilidad completa. Cada paso de recuperación, uso de herramientas y respuesta, y referencias están disponibles para cada solicitud/llamada registrada. [Databricks](https://www.databricks.com/blog/responsible-ai-databricks-data-intelligence-platform) Esta capacidad de trazabilidad end-to-end de sistemas agénticos es una de las más maduras del comparativo para el caso de uso de enterprise.

***

### 5. Alcance interno

Databricks usa su propia plataforma de forma extensiva para sus operaciones de datos e AI internas, aunque el nivel de disclosure sobre ese uso auto-referido es menor que el de IBM (que documenta métricas específicas de eficiencia de su uso de watsonx.governance internamente).

La señal más relevante del uso interno es la migración de las operaciones de datos de MosaicML a la plataforma de Databricks tras la adquisición, que según Jonathan Frankle redujo el tiempo de preparación de datos de semanas a minutos — un resultado que Databricks usa como caso de estudio de su propia plataforma. Databricks también despliega sus herramientas de governance (Unity Catalog, MLflow) para gestionar sus propios assets de datos y modelos, aunque sin la granularidad de métricas documentadas que IBM provee para su uso interno de watsonx.governance.

La **Databricks Academy** incluye formación en AI security (AI Security Fundamentals) para los propios empleados y clientes, y fue reforzada con el lanzamiento del DASF 2.0 como recurso educativo de la empresa.

***

### 6. Políticas de uso y terceros

**Databricks Open Model License (DBRX)**: Databricks publicó DBRX bajo la **Databricks Open Model License**, una licencia propietaria (no Apache 2.0 ni MIT). Esta licencia permite uso comercial y redistribución, pero con restricciones: las empresas con más de 700 millones de usuarios activos enfrentarán "ciertas restricciones" comparables a las de Meta para Llama 2, y todos los usuarios deben acordar términos que aseguren que usen DBRX "responsablemente." [TechCrunch](https://techcrunch.com/2024/03/27/databricks-spent-10m-on-a-generative-ai-model-that-still-cant-beat-gpt-4/) La Databricks Open Model License incluye una cláusula de acceptable use que prohibe usos ilegales o dañinos, aunque la taxonomía de usos prohibidos es menos detallada que la de las AUPs de OpenAI, Anthropic, o IBM. Adicionalmente, la licencia establece explícitamente que el modelo se provee "as is" sin garantías, y que el licenciatario es responsable de los outputs y sus usos subsiguientes.

**Platform Terms of Service**: Las condiciones de uso de la plataforma Databricks incluyen prohibiciones de usos ilegales y dañinos, con mecanismos de enforcement a nivel de cuenta. Para los modelos externos accedidos a través de Mosaic AI Foundation Model APIs (Anthropic, OpenAI, Meta, Mistral, etc.), las AUPs de esos proveedores aplican adicionalmente.

**Mosaic AI Gateway**: La herramienta de governance de acceso a modelos incluye capacidades para que las organizaciones implementen sus propias políticas de uso sobre todos los modelos en su stack — incluyendo guardrails de seguridad y PII. El AI Gateway permite aplicar el uso conforme de LLMs con guardrails de seguridad y PII por defecto, y controlar quién puede acceder a los modelos de AI y cuánto acceso tienen con permisos personalizables y rate limits. [Databricks](https://www.databricks.com/product/artificial-intelligence/ai-gateway)

**Política de residencia de datos para AI assistive features**: Para las funciones de AI asistidas, Databricks provee garantías explícitas de que los datos de clientes no se usan para entrenar modelos de proveedores externos, que el tráfico entre Databricks y socios de modelos está encriptado en tránsito con TLS, y que los datos almacenados están encriptados AES-256.

***

### 7. Alcance en ecosistema externo

El ecosistema de herramientas de AI responsable de Databricks para el mercado externo está construido alrededor de tres pilares: gobernanza de datos y modelos (Unity Catalog + MLflow), seguridad de AI (DASF + Mosaic AI Gateway), y evaluación de modelos (Mosaic Eval Gauntlet + Responsible AI Testing Framework).

**MLflow (open-source, gobernanza de ML lifecycle más adoptada del mercado)**: MLflow es la contribución open-source más significativa de Databricks al ecosistema de AI responsable. Con más de 20 millones de descargas mensuales al momento de la publicación de este análisis, MLflow es el estándar de facto para tracking de experimentos, versionado de modelos, y reproducibilidad de ML en el sector enterprise. Ningún otro proveedor del comparativo tiene una contribución de software libre al ML lifecycle con la adopción de MLflow — ni siquiera IBM con AIF360 o Meta con PyTorch (aunque PyTorch es mayor en el segmento de research). La trazabilidad que MLflow provee es un habilitador fundamental de AI responsable para miles de organizaciones que no son clientes de Databricks.

**Unity Catalog (open-source, 2024)**: La decisión de Databricks de open-source Unity Catalog en 2024 fue un paso estratégico significativo. Unity Catalog es la solución de gobernanza unificada de datos y AI — catalogación, control de acceso, linaje, auditoría — para multiple clouds, formatos de datos, y workloads. Como herramienta abierta, Unity Catalog puede ser adoptada por organizaciones independientemente de si usan la plataforma cloud de Databricks. Unity Catalog es la única solución unificada de la industria para gobernanza de datos y AI a través de clouds, formatos de datos y workloads. [Databricks](https://www.databricks.com/blog/introducing-databricks-ai-governance-framework)

**DASF 2.0 (recurso público gratuito)**: El Databricks AI Security Framework es un recurso abierto para cualquier organización, con el DASF compendium disponible como Google Sheet y Excel con los 62 riesgos y 64 controles mapeados a estándares de la industria. Este nivel de apertura para un framework de seguridad de AI operacional — incluyendo mapeos a MITRE ATLAS, OWASP, NIST, ISO, y HITRUST — es el trabajo de alineación a estándares externos más completo del comparativo de proveedores de plataforma.

**DAGF (Databricks AI Governance Framework)**: Framework de gobernanza de AI publicado en 2025, disponible como whitepaper con presentación en el Data + AI Summit 2025. Los cinco pilares — organización de AI, ética, cumplimiento legal y regulatorio, transparencia e interpretabilidad, operaciones e infraestructura de AI, y seguridad de AI — proveen un roadmap de madurez de gobernanza para organizaciones en cualquier etapa de adopción de AI.

**Mosaic AI Tools Catalog + Agent Evaluation**: Para agentes de AI, Databricks provee evaluación con LLM judges (modelos especializados en evaluar outputs de agentes) que permiten testing sistemático de behavior de agentes antes de despliegue. Esta capacidad de evaluación agéntica es una de las más avanzadas del comparativo para el caso de uso de enterprise agentic AI.

***

### 8. Recomendaciones para Centro de Excelencia de AI

Databricks tiene el material de orientación para CoE de AI más orientado al data engineering y ML operations del comparativo, con recursos que van desde la arquitectura de seguridad hasta la formación técnica:

**Databricks Academy — AI Security Fundamentals**: Curso de una hora disponible en Databricks Academy, lanzado como parte del DASF 2.0, que introduce los conceptos de seguridad de AI y los aplica al contexto del ML lifecycle. Gratuito y disponible para cualquier organización.

**Solution Accelerators**: Guías construidas para acelerar resultados en casos de uso de AI de alto impacto, incluyendo casos de uso regulados (compliance, fraud detection, clinical AI). Cada Solution Accelerator incluye consideraciones de governance y security específicas del dominio.

**DASF Compendium como herramienta operacional de CoE**: El spreadsheet del DASF compendium permite a equipos de CoE hacer un inventario de sus sistemas de AI, mapear sus riesgos, y priorizar controles de mitigación. Con sus links a documentación específica de Databricks para cada control, el compendium es la herramienta más operacional del comparativo para implementación de governance de AI security.

**Data + AI Summit**: Conferencia anual de Databricks que incluye sesiones específicas de AI governance, responsible AI, y AI security. Con acceso on-demand a grabaciones, es una fuente de orientación práctica para CoEs que trabajan sobre la plataforma Databricks.

**Databricks Solution Architects y Customer Success**: Para clientes enterprise, Databricks tiene un equipo de arquitectos y CSMs que incluyen expertise en governance y security de AI, con talleres interactivos específicos de AI governance para organizaciones en diferentes etapas de madurez. Databricks ofrece talleres interactivos para educar a organizaciones sobre cómo gestionar exitosamente su journey de AI de manera consciente con el riesgo. [Databricks](https://www.databricks.com/blog/introducing-databricks-ai-governance-framework)

***

### 9. Nuevos roles organizacionales

**Jonathan Frankle** — Chief AI Scientist, el rol más relevante para AI responsable como práctica técnica dentro de Databricks. Con PhD en AI del MIT (Lottery Ticket Hypothesis) y experiencia como co-founder de MosaicML, Frankle representa el nivel de seniedad técnica más alto que Databricks tiene en el dominio de AI. Su participación en el FTC Tech Summit y en la OECD.AI como experto lo posiciona como voz de Databricks en debate de política de AI. Sin embargo, no hay evidencia de un mandato explícito de AI ethics o AI safety en su rol — su foco documentado es eficiencia de entrenamiento y avances técnicos en LLMs y RL.

**Trâm Phi** — General Counsel, con declaraciones públicas sobre governance de datos y AI que posicionan la función legal como un actor en AI responsable. No hay un Chief Privacy and Trust Officer equivalente al de IBM o Microsoft.

**Arun Pamulapati** — Senior Security Field Engineer, figura técnica visible en el desarrollo y divulgación del DASF. Aunque no es un rol C-suite, su presencia en Data + AI Summit y en publicaciones externas lo posiciona como la voz técnica principal de Databricks en AI security.

**Ausencia notable**: No hay Chief Ethics Officer, Chief Responsible AI Officer, AI Safety Research Lead, o AI Ethics Board con composición y mandato publicados. Para una empresa con 15,000+ clientes enterprise y una plataforma sobre la que corren algunos de los modelos de AI más sensibles del mundo (banca, salud, gobierno), esta ausencia de roles ejecutivos dedicados a AI responsable es la brecha de gobernanza más significativa del comparativo en el segmento de plataformas enterprise.

***

### 10. Cumplimiento regulatorio

**EU AI Act**: Databricks publica análisis detallados del EU AI Act y sus implicaciones para usuarios de plataformas de AI, posicionando la Data Intelligence Platform como un habilitador de compliance para los clientes. La plataforma incluye herramientas que facilitan el cumplimiento con las obligaciones del EU AI Act para sistemas de AI de alto riesgo (trazabilidad, auditoría, documentación, evaluación de conformidad). Databricks es consciente de que sus clientes desarrollan sistemas que caen bajo el EU AI Act, y la plataforma está diseñada para facilitar ese compliance — pero Databricks como desarrollador de modelos (DBRX) tiene sus propias obligaciones como GPAI provider bajo el EU AI Act, y la documentación sobre el cumplimiento de esas obligaciones específicas para DBRX es más delgada.

**NIST AI RMF**: El DASF mapea explícitamente sus controles al NIST AI Risk Management Framework, permitiendo a organizaciones alinear su implementación de governance de AI con el framework de referencia de EE.UU. para riesgo de AI. La participación de Databricks en el CAISI (US AI Safety Institute Consortium) también la vincula al ecosistema regulatorio de NIST.

**SOC 2 Type 2, ISO 27001, FedRAMP**: Databricks Cloud tiene las certificaciones estándar de seguridad cloud enterprise. No hay certificación ISO 42001 (AI Management System) documentada para Databricks — IBM Granite fue el primero en el comparativo en obtenerla entre proveedores open-source.

**HIPAA, GDPR, PCI DSS**: La plataforma Databricks soporta compliance con HIPAA (con Business Associate Agreement), GDPR (con herramientas de control de residencia de datos), y PCI DSS (con el compliance security profile de Databricks). Para sectores altamente regulados como salud y finanzas, estas certificaciones son el baseline de confianza mínimo.

**Sector financiero — SR 11-7**: Databricks tiene soluciones específicas para model risk management bancario bajo SR 11-7, con Unity Catalog y MLflow como habilitadores de la trazabilidad y documentación que requiere el framework de la Fed para gestión de riesgo de modelos. Sin embargo, la profundidad de la solución para SR 11-7 es menor que la de IBM watsonx.governance, que tiene plantillas y workflows específicamente diseñados para ese framework.

***

### 11. Monitoreo de regulaciones

Databricks tiene una postura proactiva de monitoreo y publicación sobre regulación de AI, aunque sin el aparato institucional de IBM Policy Lab o el Google AI Policy team:

**Blog y publicaciones de Databricks sobre regulación**: Databricks publica regularmente análisis de regulaciones emergentes de AI con implicaciones para sus clientes — incluyendo análisis del EU AI Act, el AI Executive Order de EE.UU., y regulaciones sectoriales de salud y finanzas. Jonathan Frankle participa como panelista en el FTC Tech Summit sobre AI, representando a Databricks en foros de política de AI. [Databricks](https://www.databricks.com/blog/ai-regulation-rolling-out-and-data-intelligence-platform-here-help)

**Postura de política pública**: Databricks tiene una postura documentada de apoyo a regulación de AI basada en riesgo y contextual — la misma postura que IBM y Microsoft. Esta alineación no es casual: los tres son proveedores enterprise que se benefician de regulación que requiere governance de AI (que su stack provee) y no les impone restricciones de capacidades que no tendrían.

**CAISI Consortium**: La membresía en el Consortium del US AI Safety Institute vincula a Databricks a los esfuerzos de evaluación de seguridad de AI del gobierno de EE.UU. y le da acceso a desarrollos regulatorios tempranos.

**Ausencia relativa**: No hay un equipo de Policy dedicado comparable al de IBM o Microsoft, ni presencia documentada en EU AI Act Code of Practice (como signatario de compromisos voluntarios específicos). La participación de Databricks en governance multilateral es más reactiva que proactiva comparada con los líderes del comparativo en este dominio.

***

### 12. Colaboración con organismos externos

| Organización / Iniciativa                     | Rol de Databricks                                                               |
| --------------------------------------------- | ------------------------------------------------------------------------------- |
| **CAISI / US AI Safety Institute Consortium** | Miembro fundador                                                                |
| **MITRE ATLAS**                               | Framework referenciado en DASF con mapeo de controles                           |
| **OWASP (Top 10 for LLMs)**                   | Framework referenciado en DASF con mapeo de controles                           |
| **NIST AI RMF**                               | Framework referenciado en DASF; Databricks participa en consultas               |
| **HITRUST**                                   | Framework referenciado en DASF; co-revisores del documento                      |
| **Carnegie Mellon University**                | Co-revisor del DASF v1.0                                                        |
| **Capital One**                               | Co-revisor del DASF v1.0                                                        |
| **FTC Tech Summit**                           | Participación de Jonathan Frankle como panelista (2024)                         |
| **OECD.AI**                                   | Jonathan Frankle listado como experto en OECD.AI                                |
| **Apache Software Foundation**                | Administrador de Apache Spark, principal contribución open-source de la empresa |
| **Linux Foundation (Delta Lake, MLflow)**     | Donador de proyectos Apache; MLflow bajo Linux Foundation AI & Data             |
| **Hugging Face**                              | Partner para distribución de modelos DBRX y MPT                                 |
| **GitHub**                                    | Publicación de repositorios open-source (LLM Foundry, Composer, MegaBlocks)     |

El perfil de colaboraciones de Databricks es el más técnico del comparativo — fuertemente centrado en co-creación de frameworks de seguridad y contribuciones open-source de infraestructura, con menor presencia en iniciativas de ética de AI, Seoul Commitments, Partnership on AI, o AI Alliance. Esta distribución refleja la identidad de Databricks como empresa de ingeniería de datos y ML, no como actor de governance ético o de frontier AI safety.

**Ausencias notables del comparativo**: No hay participación documentada en el Frontier Model Forum (aunque Databricks no tiene modelos de frontera), Partnership on AI, AI Alliance (co-fundada por IBM y Meta), Seoul AI Frontier Safety Commitments, Rome Call for AI Ethics, o EU GPAI Code of Practice. Para una empresa con $43B de valoración y 15,000+ clientes enterprise, la participación en governance multilateral de AI es proporcionalmente más baja que la de los actores equivalentes del comparativo.

***

### 13. Relación con Privacidad y Seguridad

**Data sovereignty como principio de seguridad y privacidad**: La proposición de valor central de Databricks en privacidad es la **soberanía de datos** — la arquitectura de la plataforma está diseñada para que los datos del cliente nunca necesiten salir de su entorno controlado (VPC del cliente, cloud del cliente, on-premises). Esta es una promesa arquitectónica de privacidad más profunda que la de proveedores que procesan datos en infraestructura compartida, y es especialmente relevante para sectores con regulaciones de residencia de datos (GDPR, regulaciones bancarias latinoamericanas, sector salud).

**Unity Catalog como pilar de privacidad**: Unity Catalog implementa data masking, column-level security, row-level security, dynamic views para PII, y audit logs completos para todas las accesiones a datos — capacidades que son la base técnica para cumplimiento con GDPR, CCPA, LGPD (Brasil), y regulaciones sectoriales. La integración de estas capacidades con el governance de modelos de AI (qué modelo accedió a qué datos) es la contribución más madura de Databricks al dominio de data privacy in AI.

**DASF como framework de seguridad de AI**: El DASF 2.0 cubre las dimensiones de seguridad de AI que son más relevantes para un CISO evaluando plataformas de ML enterprise: data poisoning, model theft, prompt injection, adversarial attacks, supply chain attacks de modelos de terceros, model sprawl y shadow AI. El DASF mapea 62 riesgos técnicos de seguridad a 64 controles recomendados, y el compendium organiza y aplica sus riesgos, amenazas, controles, y mapeos a estándares reconocidos de organizaciones como MITRE, OWASP, NIST, ISO, e HITRUST. [Techfabric](https://www.techfabric.com/blog/dasf---databricks-ai-security-framework)

**Mosaic AI Gateway como control de seguridad en runtime**: La capacidad de Mosaic AI Gateway para interceptar, inspeccionar, y filtrar requests a todos los modelos en la organización — incluyendo detección de PII en inputs, guardrails de seguridad configurables, logging completo para auditoría, y rate limiting por usuario/equipo — es una herramienta de seguridad de AI en producción comparable a la de AWS Bedrock Guardrails o IBM watsonx.governance en su función de control de runtime.

**Seguridad de infraestructura cloud**: Databricks tiene acuerdos de cloud con AWS, Azure, y GCP, heredando las posturas de seguridad de esos tres hiperescalares. Las certificaciones de compliance (SOC 2 Type 2, ISO 27001, FedRAMP Moderate, HIPAA, PCI DSS, GDPR) cubren el plano de control de Databricks. Los datos del cliente residen en las cuentas cloud de los propios clientes, reduciendo el radio de blast potencial de una brecha en la infraestructura de Databricks.

**Privacidad de AI Assistive Features**: Para sus propias funciones de AI asistidas (Genie, Assistant, AI/BI), Databricks tiene controles específicos de privacidad documentados: las respuestas de Genie y los comentarios aprobados generados por AI se almacenan en la base de datos del plano de control encriptada con AES-256. El historial del chat del Assistant se almacena en el mismo lugar que otro contenido de notebooks. [Databricks](https://docs.databricks.com/aws/en/databricks-ai/databricks-ai-trust)

***

### Recursos oficiales consolidados

| Recurso                                   | URL                                                                                                                                                                                                                                                            |
| ----------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Responsible AI (hub central)              | [https://www.databricks.com/trust/responsibleAI](https://www.databricks.com/trust/responsibleAI)                                                                                                                                                               |
| Databricks AI Governance Framework (DAGF) | [https://www.databricks.com/blog/introducing-databricks-ai-governance-framework](https://www.databricks.com/blog/introducing-databricks-ai-governance-framework)                                                                                               |
| DASF 2.0 (whitepaper)                     | [https://www.databricks.com/resources/whitepaper/databricks-ai-security-framework-dasf](https://www.databricks.com/resources/whitepaper/databricks-ai-security-framework-dasf)                                                                                 |
| DASF (architecture overview)              | [https://www.databricks.com/resources/architectures/databricks-ai-security-framework](https://www.databricks.com/resources/architectures/databricks-ai-security-framework)                                                                                     |
| DASF 2.0 announcement                     | [https://www.databricks.com/blog/announcing-databricks-ai-security-framework-20](https://www.databricks.com/blog/announcing-databricks-ai-security-framework-20)                                                                                               |
| Mosaic AI Gateway                         | [https://www.databricks.com/product/artificial-intelligence/ai-gateway](https://www.databricks.com/product/artificial-intelligence/ai-gateway)                                                                                                                 |
| Unity Catalog                             | [https://www.databricks.com/product/unity-catalog](https://www.databricks.com/product/unity-catalog)                                                                                                                                                           |
| MLflow (open-source)                      | [https://mlflow.org](https://mlflow.org)                                                                                                                                                                                                                       |
| AI regulation blog post                   | [https://www.databricks.com/blog/ai-regulation-rolling-out-and-data-intelligence-platform-here-help](https://www.databricks.com/blog/ai-regulation-rolling-out-and-data-intelligence-platform-here-help)                                                       |
| Responsible AI with Databricks Platform   | [https://www.databricks.com/blog/responsible-ai-databricks-data-intelligence-platform](https://www.databricks.com/blog/responsible-ai-databricks-data-intelligence-platform)                                                                                   |
| DBRX Open Model License                   | [https://www.databricks.com/legal/open-model-license](https://www.databricks.com/legal/open-model-license)                                                                                                                                                     |
| AI Assistive Features Trust & Safety      | [https://docs.databricks.com/aws/en/databricks-ai/databricks-ai-trust](https://docs.databricks.com/aws/en/databricks-ai/databricks-ai-trust)                                                                                                                   |
| AI governance glossary                    | [https://www.databricks.com/glossary/ai-governance](https://www.databricks.com/glossary/ai-governance)                                                                                                                                                         |
| DBRX launch                               | [https://www.databricks.com/company/newsroom/press-releases/databricks-launches-dbrx-new-standard-efficient-open-source-models](https://www.databricks.com/company/newsroom/press-releases/databricks-launches-dbrx-new-standard-efficient-open-source-models) |
| Jonathan Frankle (Chief AI Scientist)     | [https://www.jfrankle.com](https://www.jfrankle.com)                                                                                                                                                                                                           |

***

### Conclusión

Databricks es el proveedor más difícil de ubicar en el comparativo de doce actores porque no encaja en ninguna de las categorías establecidas: no es un desarrollador de modelos de frontera (como Anthropic, OpenAI, o Google), no es una plataforma de AI con principios éticos maduros (como IBM), no es un hiperescalar con governance de infraestructura y modelos integrada (como AWS, Azure, o GCP), y no es un actor chino con riesgos geopolíticos estructurales (como Huawei o Alibaba). Es, en cambio, **el proveedor de infraestructura de ML/datos sobre la que más AI enterprise del mundo se construye** — y esa posición genera una forma particular de responsabilidad de AI que es más sobre arquitectura habilitadora que sobre principios éticos propios.

Sus **tres diferenciadores positivos únicos** son: primero, MLflow como el mayor impacto de AI responsable por unidad de esfuerzo de cualquier proveedor del comparativo — con 20+ millones de descargas mensuales y adopción en miles de organizaciones que nunca usarán otra herramienta de Databricks, MLflow hace más por la trazabilidad y reproducibilidad de ML a escala global que cualquier otro recurso abierto del comparativo salvo posiblemente PyTorch (que es de Meta); segundo, el DASF como el framework de seguridad de AI end-to-end más operacionalizable del comparativo — con mapeos explícitos a MITRE ATLAS, OWASP, NIST, ISO, y HITRUST en un spreadsheet descargable con 62 riesgos y 64 controles, el DASF 2.0 es la herramienta más directamente útil para un equipo de seguridad implementando governance de AI que cualquier otro recurso equivalente del comparativo; y tercero, la arquitectura de data sovereignty como promesa de privacidad estructural — la decisión de diseño de mantener los datos del cliente en su propia infraestructura cloud, con Unity Catalog como capa de control y auditoría, es la base de privacidad más sólida del comparativo para organizaciones con requisitos estrictos de residencia de datos y segregación de entornos.

Sus **tres puntos de atención críticos** tienen naturaleza diferente a los de los otros once proveedores. Primero, la ausencia de gobernanza institucional de AI responsable es la brecha más llamativa para una empresa de su tamaño y posición: sin AI Ethics Board, sin Chief Ethics Officer, sin Responsible Scaling Policy, y con un Responsible AI Testing Framework más delgado que los Responsible Use Guides de IBM Granite o los System Cards de Anthropic, Databricks tiene el déficit de institucionalización de AI responsable más pronunciado del comparativo en el segmento de plataformas enterprise occidentales — comparable en esta dimensión específica a xAI (aunque por razones muy diferentes, ya que Databricks no tiene los riesgos de misión de un desarrollador de modelos de frontera). Segundo, la opacidad en datos de entrenamiento de DBRX es una brecha explícita de transparencia: mientras IBM Granite documenta el origen de sus datos de entrenamiento con detalle suficiente para obtener el rating más alto del Stanford Foundation Model Transparency Index, Databricks no reveló las fuentes exactas de datos de entrenamiento de DBRX — una omisión que limita la auditabilidad de su modelo y contradice el principio de transparencia que predica en el DAGF. Tercero, la sub-representación en governance multilateral de AI es desproporcionada con el peso de la empresa: con $43B de valoración, 15,000+ clientes enterprise, y una plataforma sobre la que corre gran parte del ML de Fortune 500, la ausencia de Databricks en el AI Alliance, Partnership on AI, Seoul Commitments, EU GPAI Code of Practice, y otras iniciativas multilaterales de AI governance es un gap de posicionamiento que puede convertirse en una vulnerabilidad reputacional si la regulación de AI se vuelve más exigente en cuanto a participación en estándares.

La recomendación de selección para Databricks es inequívoca en su dominio: **Databricks es la selección natural como plataforma de datos y ML para organizaciones con estrategias de AI enterprise complejas que requieren governance de datos de entrenamiento, trazabilidad de modelos, y operacionalización de ciclo de vida de AI a escala**. Para organizaciones en Argentina y LATAM con regulaciones del BCRA, CNV, o sectores de salud, la combinación de Unity Catalog (governance de datos), MLflow (trazabilidad de modelos), Lakehouse Monitoring (monitoreo en producción), y DASF (framework de seguridad) provee el stack más completo de tools de AI responsable del comparativo para el data engineering y ML operations layer. Databricks no reemplaza la necesidad de un proveedor de modelos (se integra con modelos de Anthropic, OpenAI, Meta, Mistral, y otros a través de Foundation Model APIs y Mosaic AI Gateway), y no reemplaza una solución de governance de AI negocio al estilo de IBM watsonx.governance para la capa de risk management y regulatory compliance — pero es el habilitador infraestructural de AI responsable más sólido del comparativo para el stack de datos y ML.
