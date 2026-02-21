# Meta AI



## Análisis de la Estrategia de AI Responsable de Meta AI

***

### 1. Principios fundamentales y evolución

Meta tiene el perfil de AI responsable más complejo y contradictorio del comparativo de siete proveedores: es simultáneamente el laboratorio con la apuesta más radical por la democratización del AI (a través del open-source con Llama) y el que presenta los indicadores más preocupantes de debilitamiento institucional de la gobernanza de AI responsable.

La evolución de principios tiene tres momentos. Primero, **2018**: Mark Zuckerberg publicó el blog "Facebook's Five Pillars of Responsible AI", articulando los cinco ejes fundacionales. Este documento no tenía el peso formal de los principios de Google (2018) ni del "Future Computed" de Microsoft, pero estableció el vocabulario que definiría el programa durante años.

Segundo, **2021**: Los cinco principios se formalizaron como el framework oficial del equipo de Responsible AI (RAI), recién creado como unidad centralizada. Los cinco principios de core son: Privacy & Security, Fairness & Inclusion, Robustness & Safety, Transparency & Control, y Accountability & Governance. [Meta](https://ai.meta.com/about/) También en 2021 Meta publicó el primer update formal de AI fairness y transparency, estableciendo un precedente de reporte anual que luego no mantuvo con consistencia.

Tercero, **noviembre 2023**: El evento que define el perfil actual de Meta en el comparativo. El equipo de Responsible AI fue disuelto: la mayoría de los empleados fue reasignada al brazo de Generative AI de Meta, y algunos a la unidad de infraestructura de machine learning. Esto siguió a que el grupo fuera integrado en la unidad de Social Impact un año antes. Un portavoz de Meta confirmó la decisión indicando que los cambios permitirían escalar mejor para satisfacer las necesidades futuras, y que el equipo remanente continuaría apoyando esfuerzos transversales de desarrollo responsable. [The Register](https://www.theregister.com/2023/11/20/meta_responsible_ai/)

**El evento regulatorio más crítico de 2025**: A diferencia de todos los otros proveedores del comparativo (Microsoft, Google, Anthropic, OpenAI, AWS, Oracle), Meta **rechazó firmar** el EU General-Purpose AI Code of Practice. La decisión de Meta de rechazar el GPAI Code creó incertidumbre regulatoria significativa para empresas que despliegan sistemas AI de propósito general, ya que las nuevas disposiciones del EU AI Act entraron en vigor en agosto de 2025. Meta argumentó que el Código introduce requisitos ambiguos y se extiende más allá del alcance del EU AI Act, complicando el cumplimiento y potencialmente obstaculizando la innovación. Meta percibió a la UE como yendo en la dirección equivocada con una supervisión regulatoria excesiva. [Nemko Group AS](https://digital.nemko.com/news/meta-refuses-gpai-code)

**URL oficial principal**: [https://ai.meta.com/responsible-ai/](https://ai.meta.com/responsible-ai/)

***

### 2. Componentes de la declaración de AI Responsable

La arquitectura documental de Meta es la más fragmentada de los siete proveedores, distribuida entre múltiples equipos, plataformas y líneas de productos sin un documento integrador equivalente al RSP de Anthropic, el Responsible AI Standard v2 de Microsoft, o incluso los AI Principles de Google.

**Documento de principios**: Los cinco pilares de 2021 (Privacy & Security, Fairness & Inclusion, Robustness & Safety, Transparency & Control, Accountability & Governance) publicados en ai.meta.com/about. Más aspiracionales que operativos, sin versiones actualizadas publicadas.

**Políticas de uso**: Llama Acceptable Use Policy (AUP), Llama Community License Agreement, y Meta AI Terms of Service. Documentos separados para modelos open-source y productos consumer.

**Guías técnicas para desarrolladores**: Responsible Use Guide (actualizado con cada versión de Llama), Developer Use Guide: AI Protections, System Cards por modelo (más de 22 publicados). Estos son los documentos más detallados y técnicamente sustanciosos del corpus documental de Meta.

**Herramientas open-source**: Purple Llama ecosystem con Llama Guard 4, Prompt Guard 2, LlamaFirewall, CyberSecEval 4, entre otros. Publicados en GitHub y Hugging Face con licencias permisivas que permiten uso comercial.

**Diferencia crítica respecto a otros proveedores**: Meta no publica reports anuales de AI responsable equivalentes a los de Google (6 desde 2019) o Microsoft. El último update significativo de progreso documentado data de 2022. Esto genera un vacío de transparencia estructural que ningún otro proveedor del comparativo presenta en la misma magnitud.

***

### 3. Procesos y estructura de gobernanza

Meta tiene la estructura de gobernanza de AI responsable más debilitada institucionalmente de los siete proveedores, resultado directo de la disolución del equipo RAI en noviembre 2023 y de la ausencia de un equivalente al Chief Responsible AI Officer de Microsoft (Natasha Crampton), al RSO de Anthropic (Jared Kaplan), o al Safety and Security Committee de OpenAI.

**Estado post-noviembre 2023**: Los principios de los cinco pilares se mantienen formalmente, pero la estructura organizacional que los operacionalizaba fue desmantelada. Las evaluaciones de analistas señalan que la disolución puede reflejar la anticipación de Meta de que la regulación gubernamental hará que el cumplimiento legal sea una preocupación más urgente que la orientación ética interna de un equipo de responsible AI, aunque persiste la necesidad de una capa separada de gobernanza de AI para supervisión de riesgos, legal y compliance. [TechTarget](https://www.techtarget.com/searchenterpriseai/news/366560695/Possible-reasons-for-Meta-disbanding-its-responsible-AI-team)

**Estructura actual documentada**: FAIR (Fundamental AI Research), el laboratorio de investigación fundacional de Meta activo desde 2013, tiene como misión declarada desarrollar AI más segura y continúa activo. El equipo FAIR ha pasado la última década trabajando para desarrollar sistemas AI más seguros, y Meta continúa invirtiendo en su equipo de Responsible AI para apoyar trabajo líder en la industria en temas como privacidad, equidad, accountability y transparencia. [Meta](https://transparency.meta.com/es-la/policies/ai-safety-policies-for-safety-summit/) Sin embargo, la relación entre FAIR y las decisiones de gobernanza de productos es opaca en la documentación pública.

**Ausencia de un rol equivalente al Chief RAI Officer**: Meta no tiene ningún ejecutivo con designación pública equivalente. Mark Zuckerberg como CEO y Nick Clegg como President of Global Affairs son las voces más visibles en política de AI, pero sin el mandato específico de gobernanza responsable que tienen sus equivalentes en Microsoft o Anthropic.

**Comparación directa con el comparativo**: Microsoft tiene AETHER + ORA + Chief RAI Officer (Natasha Crampton, desde 2019). Google tiene ATRC + Responsible Innovation Team + RSC en DeepMind. OpenAI tiene Board SSC + SAG. Anthropic tiene LTBT + RSO formal. AWS tiene Responsible AI Champions. Oracle tiene governance committee de EU Sovereign Cloud. Meta tenía un equipo RAI centralizado y lo disolvió.

***

### 4. Alcance en el ciclo de vida de AI

La cobertura del ciclo de vida en Meta opera con diferente énfasis según el tipo de producto: los modelos Llama (open-source) tienen el proceso más documentado públicamente, mientras que los productos consumer (Meta AI en WhatsApp, Facebook, Instagram) tienen documentación pública más limitada.

**Pre-entrenamiento**: Mitigaciones de datos de pre-entrenamiento aplicadas a todos los modelos para establecer un nivel base de seguridad. Exclusión de fuentes conocidas por contener alto volumen de información personal sobre individuos privados. Para Llama 3.2, se extendió el trabajo de evaluación de riesgos a capacidades visuales.

**Evaluación pre-despliegue**: Durante y después del entrenamiento se realizan evaluaciones automatizadas y manuales para entender el rendimiento de los modelos en áreas de riesgo como armas, ataques cibernéticos y explotación infantil, además de extensivos ejercicios de red teaming con expertos externos e internos para encontrar formas inesperadas en que los modelos podrían ser usados. [Meta](https://ai.meta.com/blog/meta-llama-3-meta-ai-responsibility/) Para Llama 3.1, se evaluó cada modelo fine-tuned contra un rango de riesgos incluyendo crimen violento, explotación sexual infantil, CBRNE y privacidad.

**Capacidades CBRN**: Meta realiza uplift testing para determinar si los modelos podrían aumentar significativamente las capacidades de actores maliciosos para planificar o ejecutar ataques con armas químicas y biológicas, en colaboración con expertos externos. Las evaluaciones se realizan con asistencia de expertos externos e incluyen modelos de amenaza que creen que aumentan significativamente el riesgo del ecosistema para actores de baja y moderada habilidad. [Meta](https://ai.meta.com/blog/meta-llama-3-1-ai-responsibility/)

**Post-despliegue**: Proceso de reporte de vulnerabilidades después del lanzamiento. System Cards actualizados con información sobre capacidades, limitaciones y evaluaciones. Para productos consumer: marcadores visibles en imágenes generadas por AI, etiquetado "Made with AI" para contenido detectado, y watermarks invisibles.

**Diferencia clave respecto al comparativo**: Meta no tiene un framework de evaluación por niveles de capacidad equivalente al RSP/ASL de Anthropic ni al Preparedness Framework v2 de OpenAI. Sus evaluaciones son específicas por modelo pero no se rigen por una arquitectura de umbrales y salvaguardas requeridas publicada y verificable.

***

### 5. Alcance interno

Meta usa Meta AI integrado en todos sus productos consumer (WhatsApp, Facebook, Instagram, Messenger, Ray-Ban AI glasses, Meta Quest VR), convirtiendo a sus más de 3 billones de usuarios activos diarios en el banco de pruebas de uso más grande del comparativo. Esta escala de deployment interno es una ventaja para detectar comportamientos emergentes en uso real, pero también representa la exposición de riesgo más grande del grupo al operar AI a escala masiva sin la estructura de gobernanza centralizada que los otros proveedores mantienen.

FAIR usa los modelos Llama y las herramientas de evaluación Purple Llama internamente para investigación de seguridad. El equipo de Fundamental AI Research también desarrolla investigación de interpretabilidad y robustez que se publica académicamente, contribuyendo a la base de conocimiento pública sobre seguridad de AI.

Meta usa AI extensivamente en sus sistemas de moderación de contenido en plataformas sociales, sistema de publicidad (Ad Fairness), y recomendaciones de contenido. Esta experiencia operativa de una década en AI a escala para moderación de contenido en miles de millones de usuarios es un activo técnico relevante para su programa de responsible AI que no tienen los laboratorios de AI puros como Anthropic u OpenAI.

***

### 6. Políticas de uso y terceros

Meta opera una estructura de políticas de uso con dos pilares distintos según el canal de distribución.

**Llama Acceptable Use Policy (open-source)**: Define usos prohibidos para modelos descargados y desplegados por terceros. Prohibiciones absolutas: apoyo a armas de destrucción masiva (biológicas, químicas, nucleares, radiológicas), CSAM, ataques a infraestructura crítica, vigilancia masiva no consentida. La AUP aplica como condición de la licencia de uso, pero su enforcement sobre usuarios que descargan modelos open-source es estructuralmente limitado: una vez descargado el modelo, Meta pierde control operativo sobre su uso.

**Meta AI Terms of Service (productos consumer)**: Restricciones adicionales aplicables a Meta AI en productos propios, incluyendo prohibición de generación de deepfakes de individuos reales sin consentimiento, identificación de personas en imágenes, y contenido que viole derechos de propiedad intelectual. En regiones donde las personas pueden subir imágenes a Meta AI, Meta tomó pasos para prevenir que Meta AI sea usado para identificar personas en esas imágenes, incluyendo safety-tuning para detectar prompts que piden identificar quién está en una imagen y filtrado de outputs para prevenir respuestas. [Meta](https://ai.meta.com/responsible-ai/)

**Postura sobre decisiones de alto riesgo**: Meta no tiene restricciones explícitas equivalentes a las de OpenAI (que prohíbe automatización sin revisión humana) o a la revisión de Sensitive Uses de Microsoft. Es el proveedor con la postura más permisiva en decisiones de alto impacto (empleo, salud, finanzas), transfiriendo máxima responsabilidad al desarrollador/deployer downstream, especialmente relevante dado el modelo open-source donde Meta no puede monitorear ni controlar el uso post-descarga.

**Tensión estructural única**: El modelo de distribución open-source crea una paradoja de gobernanza sin equivalente en el comparativo: Meta publica la política de uso, pero no puede hacer cumplir sus términos técnicamente una vez que los pesos del modelo son descargados. Esta es la brecha de gobernanza más difícil de cerrar del grupo.

***

### 7. Alcance en ecosistema externo

El ecosistema externo de Meta es su diferenciador más técnicamente innovador y también el más debatido en términos de responsible AI: el **Purple Llama ecosystem**, el conjunto de herramientas de safety open-source más completo del comparativo.

**Purple Llama (umbrella project)**: Proyecto paraguas que integra evaluaciones y herramientas de seguridad para AI generativo con un enfoque de "purple teaming" (combinando perspectivas de ataque y defensa). Todos los componentes tienen licencias permisivas que permiten uso comercial y de investigación.

**Llama Guard 4**: La nueva Llama Guard 4 es una actualización de la herramienta Llama Guard, actuando como una salvaguarda unificada a través de modalidades, con soporte de protecciones para comprensión de texto e imágenes. [Meta](https://ai.meta.com/blog/ai-defenders-program-llama-protection-tools/) Soporta clasificación de contenido en ocho idiomas alineada con la taxonomía de riesgos estándar de MLCommons (13 categorías).

**Prompt Guard 2**: Clasificador de detección de prompt injection y jailbreaks. Prompt Guard 2 22M es una versión más pequeña y rápida que puede reducir latencia y costos de cómputo con mínimas penalizaciones de rendimiento de hasta 75% comparado con el modelo de 86M. [Meta](https://ai.meta.com/blog/ai-defenders-program-llama-protection-tools/)

**LlamaFirewall**: Nueva herramienta de seguridad para orquestar modelos guard y detectar riesgos como prompt injection, código inseguro e interacciones riesgosas de plugins LLM.

**CyberSecEval 4**: La actualización a la suite de benchmarks de ciberseguridad open-source de la industria, CyberSecEval 4, expande su predecesor aumentando los benchmarks para medir no solo los riesgos sino también las capacidades defensivas de ciberseguridad de los sistemas AI, con nuevas herramientas CyberSOC Eval y AutoPatchBench. [Llama](https://www.llama.com/llama-protections/)

**Llama Defenders Program**: Programa selecto de socios para integración de herramientas de detección de contenido AI-generado (audio, imágenes) en sus sistemas. En el lanzamiento: Zendesk, Bell Canada y AT\&T.

**Private Processing (WhatsApp)**: Nueva tecnología para que usuarios de WhatsApp usen capacidades AI para resumir mensajes o refinarlos con garantías de privacidad de que Meta/WhatsApp no puede acceder al contenido.

**System Cards**: Más de 22 system cards publicados para productos generativos con información sobre cómo funciona el sistema, limitaciones, uso de datos y consideraciones de uso.

**Responsible Use Guide**: Guía actualizada con cada versión de Llama, con orientación detallada sobre mejores prácticas de responsabilidad para desarrolladores que construyen sobre los modelos.

***

### 8. Recomendaciones para Centro de Excelencia de AI

Meta no publica un framework explícito de COE comparable al Responsible AI Lens de AWS o las guías de Google Cloud, pero el Responsible Use Guide para Llama y la documentación del Purple Llama ecosystem son los recursos más sustanciosos para organizaciones construyendo sobre modelos Meta.

El framework implícito que emerge de la documentación de Meta para COEs tiene tres componentes. En cuanto a gobernanza del modelo: las organizaciones que adoptan Llama son responsables de implementar sus propias capas de gobernanza, ya que Meta establece las condiciones de uso pero no puede monitorear el deployment post-descarga. La recomendación de Meta es usar Llama Guard como punto de partida y personalizar la taxonomía de riesgos para el caso de uso específico.

En evaluación continua: CyberSecEval 4 y las herramientas del ecosystem Purple Llama proveen un conjunto de benchmarks técnicos que los COEs pueden incorporar en sus pipelines de CI/CD para evaluación continua de riesgos.

En respuesta a incidentes: Meta tiene un proceso de reporte de vulnerabilidades post-lanzamiento y recomienda a los desarrolladores combinar las herramientas del ecosystem con otras salvaguardas específicas para sus casos de uso, reconociendo explícitamente que no existe una solución universal.

***

### 9. Nuevos roles organizacionales

La ausencia de roles dedicados de gobernanza de AI responsable con visibilidad pública equivalente a los de otros proveedores es el indicador más elocuente del estado actual del programa de Meta.

**Roles ausentes (comparado con pares)**: No hay Chief Responsible AI Officer (Microsoft tiene Natasha Crampton desde 2019). No hay Responsible Scaling Officer (Anthropic tiene Jared Kaplan). No hay Safety and Security Committee del Board (OpenAI). No hay equivalente del AETHER Committee (Microsoft) o del ATRC (Google).

**Roles existentes documentados**: FAIR continúa bajo el liderazgo de investigadores académicos de renombre. Nick Clegg como President of Global Affairs es la voz más visible en política de AI, aunque su rol es de advocacy y política pública, no de gobernanza técnica interna. Los equipos de Trust & Safety de las plataformas consumer (Facebook, Instagram, WhatsApp) tienen larga historia operativa en moderación de contenido a escala, con experiencia que supera a la mayoría de los laboratorios de AI del comparativo.

**Implicación práctica**: Para organizaciones enterprise que requieren un interlocutor específico de gobernanza de AI responsable en Meta equivalente al que tendrían con Microsoft (ORA), Google (Responsible Innovation Team) o Anthropic (Responsible Scaling Officer), la estructura actual de Meta no provee ese interlocutor de forma transparente.

***

### 10. Cumplimiento regulatorio

El perfil regulatorio de Meta es el más conflictivo del comparativo, con compromisos voluntarios en algunos espacios y rechazo explícito en otros.

**Compromisos firmados**: White House Voluntary Commitments (2023), Frontier AI Safety Commitments del AI Seoul Summit (2024). En ambos casos Meta es signataria junto al resto del grupo del comparativo.

**Rechazo del EU GPAI Code of Practice**: Meta se convirtió en el único laboratorio de AI de primer nivel en rechazar el GPAI Code, argumentando que las obligaciones son ambiguas y van más allá del alcance del EU AI Act. Mientras competidores como Microsoft abrazan los frameworks de cumplimiento, Meta percibe a la UE como yendo en la dirección equivocada con supervisión regulatoria excesiva, señalando que sus compromisos públicos de Anthropic y OpenAI con las regulaciones EU enfatizan la transparencia, seguridad y accountability. [Nemko Group AS](https://digital.nemko.com/news/meta-refuses-gpai-code) Este rechazo tiene implicaciones prácticas concretas: Meta deberá demostrar cumplimiento con el EU AI Act por otras vías, y los clientes enterprise en Europa que dependen de Llama o Meta AI deberán evaluar sus propias obligaciones bajo el Act independientemente de la postura de Meta.

**ISO 42001**: No se documenta certificación ISO/IEC 42001 para Meta (a diferencia de Microsoft - certificación corporativa, AWS - certificación por servicios, Anthropic - certificación corporativa).

**GDPR / regulación de plataformas**: Meta tiene un historial significativo de enforcement regulatorio europeo en privacidad (multas GDPR multimillonarias) que crea un contexto de riesgo regulatorio elevado que diferencia su perfil del resto del comparativo.

**Frontier AI Safety Commitments (Seoul Summit 2024)**: Meta firmó los compromisos junto a 15 otras compañías, incluyendo compromiso de evaluaciones de capacidades peligrosas antes del despliegue. Sin embargo, Meta no ha publicado un framework de escalada de salvaguardas por niveles de riesgo equivalente al RSP de Anthropic.

***

### 11. Monitoreo de regulaciones

Meta tiene el equipo de Global Affairs más grande del comparativo (heredado de la experiencia de décadas en regulación de plataformas sociales), con Nick Clegg como su líder más visible en el espacio de política de AI. Esta capacidad institucional de engagement regulatorio es superior a la de Anthropic o OpenAI en términos de escala, aunque su ejercicio reciente en AI ha sido más de resistencia que de cooperación activa (particularmente en el rechazo del GPAI Code).

Meta colabora con NIST y MLCommons en el desarrollo de estándares de evaluación, contribuyendo su taxonomía de riesgos como base para la taxonomía estándar de MLCommons que Llama Guard implementa. Esta contribución al establecimiento de estándares de evaluación de la industria es una forma de influencia regulatoria técnica que complementa su postura de advocacy político.

Meta también participa en discusiones con safety institutes de EE.UU. y UK, aunque con menos compromiso público que OpenAI o Anthropic. Meta espera el progreso en evaluación de seguridad e investigación de los institutos nacionales de seguridad, particularmente en el establecimiento de modelos de amenaza estandarizados y evaluaciones a lo largo del proceso de desarrollo de AI. [Meta](https://ai.meta.com/blog/meta-llama-3-meta-ai-responsibility/)

***

### 12. Colaboración con organismos externos

| Organización / Iniciativa                                    | Rol de Meta                                                                                         |
| ------------------------------------------------------------ | --------------------------------------------------------------------------------------------------- |
| **Frontier Model Forum**                                     | Miembro (se unió 2024, no co-fundador como Microsoft/Google/OpenAI/Anthropic)                       |
| **White House Voluntary Commitments**                        | Signatario (2023)                                                                                   |
| **Frontier AI Safety Commitments (AI Seoul Summit)**         | Signatario (2024)                                                                                   |
| **MLCommons AI Safety**                                      | Colaboración activa; taxonomía de riesgos de Llama Guard alineada con estándar MLCommons            |
| **C2PA (Coalition for Content Provenance and Authenticity)** | Miembro del Steering Committee (2024) para watermarking y proveniencia de contenido AI              |
| **NIST**                                                     | Colaboración en desarrollo de estándares de evaluación de AI                                        |
| **Partnership on AI**                                        | Miembro fundador (desde 2016, como Facebook)                                                        |
| **EU GPAI Code of Practice**                                 | **NO signatario** (rechazo explícito, 2025)                                                         |
| **US AI Safety Institute**                                   | Colaboración limitada en evaluaciones (sin partnership formal documentado)                          |
| **Llama Defenders Program**                                  | Partnerships selectos con Zendesk, Bell Canada, AT\&T para integración de herramientas de detección |
| **Academia**                                                 | Donaciones de investigación, colaboraciones con universidades en fairness y robustez                |

**Comparación crítica**: Meta es el único del comparativo que rechazó el GPAI Code. Además, fue el último del grupo en unirse al Frontier Model Forum (2024 vs. 2023 de los co-fundadores). Esta postura de menor integración con mecanismos de gobernanza multilateral contrasta con su participación temprana en Partnership on AI (2016).

***

### 13. Relación con Privacidad y Seguridad

La relación de Meta con privacidad y seguridad en AI es la más compleja del comparativo, moldeada por su historia como plataforma social con el mayor dataset de comportamiento humano del planeta y un historial de tensiones regulatorias en privacidad que no tiene equivalente en el grupo.

**Privacidad como principio del modelo**: Meta no usa posts con audiencia no pública para entrenar modelos Llama. Meta especifica que no entrenó sus modelos Llama 3.2 usando posts o comentarios con audiencia distinta a pública. [Meta](https://ai.meta.com/responsible-ai/) Sin embargo, sí usa posts públicos de Facebook e Instagram, lo que ha generado debate regulatorio y litigación en múltiples jurisdicciones.

**Tecnologías de privacidad avanzadas**: Meta usa computación multiparte segura (SMPC) para investigación de fairness en publicidad, permitiendo medir disparidades raciales sin que Meta acceda a los datos individuales de raza auto-reportada. Esta técnica de privacy-enhancing tiene sofisticación técnica superior al promedio del comparativo.

**Private Processing para WhatsApp**: La nueva tecnología anunciada en 2025 permite que usuarios de WhatsApp usen AI para resumir mensajes con garantías técnicas de que ni Meta ni WhatsApp pueden acceder al contenido. Si se implementa correctamente, sería una de las arquitecturas de privacidad para AI más avanzadas a nivel consumer del comparativo.

**Watermarking y C2PA**: Meta implementa watermarks invisibles y metadatos en imágenes generadas por Meta AI, e integra marcadores visibles en contenido generado. Watermarks invisibles y metadatos se incrustan en archivos de imagen como capas adicionales de transparencia, y Meta recientemente se unió al C2PA Steering Committee para continuar este trabajo. [Meta](https://ai.meta.com/responsible-ai/)

**Herramientas de detección de contenido AI-generado**: Llama Generated Audio Detector, Llama Audio Watermark Detector para detectar amenazas de audio AI-generado como estafas, fraude y phishing.

**Tensión estructural**: La combinación de ser la plataforma social más grande del mundo (con acceso a datos de comportamiento de más de 3 billones de personas) + laboratorio de AI open-source + empresa de publicidad digital crea una tensión estructural de privacidad sin equivalente en el comparativo. Los modelos se entrenan sobre datos de usuarios que, aunque "públicos", fueron generados en un contexto de plataforma social, y el consent landscape para ese uso es ambiguo en múltiples jurisdicciones.

***

### Recursos oficiales consolidados

| Recurso                                  | URL                                                                                                                                                          |
| ---------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Responsible AI hub                       | [https://ai.meta.com/responsible-ai/](https://ai.meta.com/responsible-ai/)                                                                                   |
| Cinco principios (About AI at Meta)      | [https://ai.meta.com/about/](https://ai.meta.com/about/)                                                                                                     |
| Responsible Use Guide (Llama)            | [https://ai.meta.com/static-resource/responsible-use-guide/](https://ai.meta.com/static-resource/responsible-use-guide/)                                     |
| Purple Llama (safety tools)              | [https://github.com/meta-llama/PurpleLlama](https://github.com/meta-llama/PurpleLlama)                                                                       |
| Llama Protections / Trust & Safety       | [https://www.llama.com/llama-protections/](https://www.llama.com/llama-protections/)                                                                         |
| Llama Defenders Program                  | [https://ai.meta.com/blog/ai-defenders-program-llama-protection-tools/](https://ai.meta.com/blog/ai-defenders-program-llama-protection-tools/)               |
| CyberSecEval (GitHub)                    | [https://github.com/meta-llama/PurpleLlama](https://github.com/meta-llama/PurpleLlama) (sub-proyecto)                                                        |
| UK AI Safety Summit - AI Safety Policies | [https://transparency.meta.com/policies/ai-safety-policies-for-safety-summit/](https://transparency.meta.com/policies/ai-safety-policies-for-safety-summit/) |
| Connect 2024: AI responsibility          | [https://ai.meta.com/responsible-ai/](https://ai.meta.com/responsible-ai/)                                                                                   |
| Fairness & Transparency update 2022      | [https://ai.meta.com/blog/responsible-ai-progress-meta-2022/](https://ai.meta.com/blog/responsible-ai-progress-meta-2022/)                                   |
| Llama 3.1 responsibility                 | [https://ai.meta.com/blog/meta-llama-3-1-ai-responsibility/](https://ai.meta.com/blog/meta-llama-3-1-ai-responsibility/)                                     |
| Llama 3 responsibility                   | [https://ai.meta.com/blog/meta-llama-3-meta-ai-responsibility/](https://ai.meta.com/blog/meta-llama-3-meta-ai-responsibility/)                               |
| Meta Transparency Center                 | [https://transparency.meta.com/](https://transparency.meta.com/)                                                                                             |

***

### Conclusión

Meta representa el perfil de AI responsable más heterodoxo del comparativo de siete proveedores, con diferenciadores técnicos genuinamente únicos coexistiendo con los déficits de gobernanza institucional más pronunciados del grupo.

Sus **tres diferenciadores positivos únicos** no tienen equivalente completo en los otros seis. Primero, el **ecosistema Purple Llama open-source**: la única suite de herramientas de safety para AI que es completamente open-source, personalizable y usable con cualquier modelo, no solo los propios. Llama Guard 4, Prompt Guard 2, LlamaFirewall y CyberSecEval 4 representan una contribución a la infraestructura de safety de la industria sin precedente en el comparativo, incluyendo la alineación con la taxonomía estándar de MLCommons que ayuda a establecer un lenguaje común para evaluación de riesgos. Segundo, la **democratización del AI de frontera**: Llama es el único modelo de frontera abierto del comparativo, con implicaciones de responsible AI tanto positivas (acceso, transparencia, investigación independiente de safety) como negativas (pérdida de control post-distribución). Este debate filosófico sobre qué es más responsable —open o closed— es el más genuino y sin resolver del campo. Tercero, la **escala de experiencia operativa en moderación de contenido**: con más de una década moderando contenido de 3+ billones de usuarios en múltiples idiomas y culturas, Meta tiene la experiencia operativa más profunda del comparativo en los desafíos prácticos de aplicar AI responsable a escala masiva, especialmente en contextos de desinformación, odio, y manipulación política.

Sin embargo, tres **puntos de atención críticos** son los más severos del comparativo para organizaciones enterprise en sectores regulados. Primero, la **disolución del equipo RAI y ausencia de accountability ejecutiva**: la eliminación del equipo de Responsible AI en noviembre 2023 y la ausencia de cualquier rol ejecutivo equivalente al Chief RAI Officer de Microsoft o el RSO de Anthropic significa que no hay un interlocutor claro de gobernanza responsable en Meta, y que no hay mecanismo institucional transparente que asegure que los principios de los cinco pilares se operacionalizan en las decisiones de producto. Para un CISO evaluando el riesgo reputacional y de gobernanza de adoptar tecnología de Meta, esta brecha es la más difícil de mitigar externamente. Segundo, el **rechazo del EU GPAI Code of Practice**: Meta es el único proveedor del comparativo que rechazó firmar el marco regulatorio europeo voluntario más importante para modelos de AI de propósito general. Para clientes en Europa, en LATAM con vínculos regulatorios europeos, o en organizaciones con políticas de cumplimiento alineadas al estándar europeo (como muchas instituciones financieras y de salud en Argentina y Chile), esto crea incertidumbre regulatoria directa y un posible conflicto con sus propias obligaciones de due diligence de proveedores. Tercero, la **brecha de gobernanza inherente al modelo open-source**: ningún otro proveedor del comparativo enfrenta el desafío estructural de Meta de distribuir modelos poderosos sin control técnico post-distribución. La AUP establece condiciones de uso, pero la arquitectura open-source hace que su enforcement sea conceptualmente imposible a escala. Para organizaciones en sectores regulados que adoptan Llama, esto significa que son ellas mismas las que deben asumir la responsabilidad de gobernanza que en otros proveedores está distribuida entre el proveedor y el cliente.

En síntesis: Meta es la opción más apropiada para organizaciones que priorizan flexibilidad de despliegue, control sobre infraestructura (on-premise, air-gapped), acceso a herramientas de safety open-source y personalizables, y coste de modelos sin licencia. Pero requiere que el cliente construya la capa de gobernanza empresarial completa que otros proveedores proveen como servicio gestionado, y presenta el mayor riesgo regulatorio europeo del comparativo por el rechazo al GPAI Code, con enforcement de la EU AI Act iniciando en agosto de 2026. Para organizaciones en sectores regulados con fuertes compromisos ESG o bajo escrutinio de terceros en gobernanza de AI, el perfil actual de Meta es el más difícil de justificar en un proceso de due diligence formal.

