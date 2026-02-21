# Microsoft



Aquí está el análisis completo:

***

## Análisis de la Estrategia de AI Responsable de Microsoft

***

### 1. Principios fundamentales y evolución

Los principios de AI de Microsoft tienen raíces en 2016, cuando el CEO Satya Nadella articuló seis objetivos para el desarrollo seguro de AI. En 2017, Microsoft creó el AETHER Committee (AI and Ethics in Engineering and Research), co-fundado por el Technical Fellow Eric Horvitz y el presidente Brad Smith, como cuerpo asesor cross-company. En 2018, AETHER sentó las bases para los seis principios publicados en el libro "The Future Computed": fairness, inclusiveness, reliability and safety, transparency, privacy and security y accountability.

La evolución más significativa ocurrió en 2022: en junio de ese año, Microsoft publicó su Responsible AI Standard v2, co-autorada por más de 30 expertos entre científicos, abogados, diseñadores e ingenieros. En 2025, el segundo Responsible AI Transparency Report introdujo el **Frontier Governance Framework**, una respuesta directa a la complejidad de los modelos de AI de frontera que podrían representar riesgos de seguridad nacional o pública, surgido de compromisos voluntarios de seguridad en mayo de 2024 junto con otras quince organizaciones.

A diferencia de Google, Microsoft **mantuvo sus prohibiciones específicas** en el tiempo, incluso expandiéndolas (ej. facial recognition, emotional inference), sin flexibilizarlas.

**URLs oficiales verificadas:**

* Principios y enfoque: https://www.microsoft.com/en-us/ai/principles-and-approach
* Transparency Report 2025: https://www.microsoft.com/en-us/corporate-responsibility/responsible-ai-transparency-report/
* Responsible AI Standard v2 (PDF): https://msblogs.thesourcemediaassets.com/sites/5/2022/06/Microsoft-Responsible-AI-Standard-v2-General-Requirements-3.pdf

***

### 2. Componentes de la declaración de AI Responsable

La estructura jerárquica opera en tres capas. En la cima están los **seis principios**: fairness, reliability and safety, privacy and security, inclusiveness, transparency y accountability. Estos se operacionalizan a través del **Responsible AI Standard v2** (políticas internas concretas) y se complementan con el **Frontier Governance Framework** para modelos avanzados.

Los frameworks de soporte incluyen el **NIST AI Risk Management Framework** como referencia externa, con sus cuatro funciones: govern, map, measure y manage. Para seguridad específica de AI, se aplica el **Secure Development Lifecycle (SDL)** adaptado, y para evaluación de contenido, el stack de **Azure AI Content Safety** con clasificadores para contenido sexual, violento, hate speech y auto-daño.

**URL oficial:** https://www.microsoft.com/en-us/ai/responsible-ai

***

### 3. Procesos y estructura de gobernanza

La gobernanza de AI de Microsoft adopta un modelo hub-and-spoke, con tres cuerpos centrales en el "hub": el AETHER Committee (expertise técnico y científico), la Office of Responsible AI (ORA, que define políticas y gobernanza), y el RAISE group (Responsible AI Strategy in Engineering, que implementa procesos en los equipos de ingeniería).

**Roles clave identificados:**

Natasha Crampton es la primera Chief Responsible AI Officer de Microsoft y lidera la Office of Responsible AI (ORA), que pone en práctica los principios de AI definiendo, habilitando y gobernando el enfoque de la compañía. El Responsible AI Council es supervisado por Brad Smith (President) y Kevin Scott (CTO). Teresa Hutson ocupa el rol de Corporate Vice President del Trusted Technology Group.

El proceso de escalación funciona de abajo hacia arriba: los **Responsible AI Champs** (red distribuida de champions por área de negocio) identifican casos sensibles, los elevan al **Sensitive Uses Working Group** del AETHER Committee, y casos de alta complejidad ascienden al AETHER Committee completo, que asesora directamente a la Senior Leadership Team.

***

### 4. Alcance en el ciclo de vida de AI

Microsoft aplica el framework NIST AI RMF con cuatro funciones a lo largo del ciclo de vida: govern (políticas, procesos, roles), map (priorización de riesgos), measure (evaluación cuantitativa), y manage (mitigaciones en el stack tecnológico).

Antes de cualquier despliegue, los equipos deben completar un **Impact Assessment** documentado. En 2024, Microsoft refinó sus procesos de supervisión pre-despliegue incluyendo el deployment safety process para sistemas generativos y el programa Sensitive Uses and Emerging Technology. El 77% de los casos consultados a ese equipo en 2024 fueron relacionados con AI generativa.

El stack de seguridad en capas cubre: User Experience → System Messages & Grounding → Safety System → Model, con mejoras en clasificadores, Prompt Shields contra jailbreak e indirect prompt injection, y detección de materiales protegidos por copyright en texto y código. En 2024, el AI Red Team condujo 67 operaciones sobre modelos Phi y herramientas Copilot.

***

### 5. Alcance interno

Microsoft aplica dogfooding sistemático: todos sus productos Copilot se prueban internamente antes del lanzamiento público. El programa Responsible AI Champs distribuye expertise de AI responsable a través de líderes senior en cada grupo de negocio, complementado con entrenamiento continuo.

Internamente, Microsoft usa Copilot para M365 en HR, desarrollo de software y gestión de contenidos. El AI Business School incluye módulos de Responsible AI como uno de sus contenidos más populares, compartiendo aprendizajes del AETHER Committee y la ORA con clientes corporativos.

***

### 6. Políticas de uso y terceros

El **Code of Conduct for Microsoft AI Services** establece prohibiciones específicas. Entre ellas, el sistema no puede usarse para: categorizar personas por datos biométricos para inferir raza, opiniones políticas, afiliación sindical, creencias religiosas u orientación sexual; ni para inferir atributos sensibles sin consentimiento explícito.

Microsoft adoptó prohibiciones concretas en casos de alto riesgo. Decidió no proporcionar acceso abierto a API de tecnología que pueda escanear rostros e inferir estados emocionales, dado el falta de consenso científico sobre la definición de "emociones" y las preocupaciones de privacidad asociadas.

Para decisiones de alto impacto (crédito, empleo, salud), Microsoft requiere supervisión humana activa, no la prohíbe, pero somete estos casos al proceso de Sensitive Uses con controles adicionales.

**URL oficial:** https://learn.microsoft.com/en-us/legal/ai-code-of-conduct

***

### 7. Alcance en ecosistema externo

Para clientes B2B, Microsoft ofrece un ecosistema robusto en Azure: **Responsible AI Dashboard** (integra Fairness Assessment, Error Analysis, Model Interpretability, Counterfactual Analysis y Causal Inference), **Transparency Notes** para todos los servicios cognitivos, y **Azure AI Content Safety** como API standalone. En 2024, Microsoft extendió sus Customer Copyright Commitments para incluir a socios revendedores.

Para consumidores finales, Microsoft implementó **Content Credentials (C2PA)** en herramientas de generación de imágenes y adoptó políticas de no generación de imágenes de candidatos electorales con enrutamiento a fuentes autorizadas para información electoral crítica.

***

### 8. Recomendaciones para Centro de Excelencia de AI

Microsoft publica guías específicas para organizaciones. La estructura recomendada replica su modelo hub-and-spoke: un AI Governance Lead con autoridad real, champions distribuidos por área, y comités de revisión para casos sensibles. El **AI Impact Assessment Template** (disponible públicamente) es la herramienta base para documentar riesgos antes del despliegue.

Para agentes AI, Microsoft recomienda implementar Prompt Shields contra agent-hijack patterns, logging comprehensivo de acciones del agente, y human-in-the-loop para decisiones de alto impacto.

**URLs útiles:**

* RAI Dashboard: https://learn.microsoft.com/en-us/azure/machine-learning/concept-responsible-ai-dashboard
* AI Learning (Microsoft Learn): https://learn.microsoft.com/en-us/training/paths/responsible-ai-business-principles/

***

### 9. Nuevos roles organizacionales

Natasha Crampton lidera la Office of Responsible AI como primera Chief Responsible AI Officer de Microsoft desde 2019, siendo miembro del UN AI Advisory Body para gobernanza global de AI.

La estructura de accountability reconoce tres capas: la Senior Leadership Team (dirección estratégica), la ORA + AETHER + RAISE (hub de gobernanza), y los Responsible AI Champs (implementación distribuida en los spokes). Este rol de Chief Responsible AI Officer es el equivalente más directo a un DPO pero para AI, con autoridad formal para bloquear o condicionar lanzamientos.

***

### 10. Cumplimiento regulatorio

El Transparency Report 2025 dedica sección específica a preparaciones para el EU AI Act, cubriendo prácticas prohibidas, políticas a nivel de modelo y documentación para clientes. Microsoft fue certificada con **ISO/IEC 42001** (primera certificación de AI Management Systems), mantiene FedRAMP High para sector público en EE.UU., y es signataria del EU AI Code of Practice junto con Google, OpenAI y Anthropic.

***

### 11. Monitoreo de regulaciones

Microsoft ha renovado su estrategia de política-a-implementación, integrando compliance checks dentro de workflows de desarrollo de producto mediante colaboración entre equipos de policy, ingeniería y herramientas automatizadas, alineando la gobernanza interna con regulaciones externas como el EU AI Act. El equipo de Natasha Crampton mantiene interlocución activa con la European Commission AI Office y reguladores estatales en EE.UU.

***

### 12. Colaboración con organismos externos

| Organización                            | Rol de Microsoft                            |
| --------------------------------------- | ------------------------------------------- |
| **Frontier Model Forum**                | Co-fundador (con Google, Anthropic, OpenAI) |
| **Partnership on AI**                   | Miembro; Crampton en Board of Directors     |
| **NIST AI Safety Institute Consortium** | Miembro activo                              |
| **MLCommons**                           | Contribuidor a benchmarks AILuminate        |
| **C2PA**                                | Implementador de Content Credentials        |
| **UN AI Advisory Body**                 | Crampton como miembro                       |
| **EU AI Code of Practice**              | Signatario (enero 2025)                     |

***

### 13. Relación con Privacidad y Seguridad

El enfoque de Microsoft hacia privacidad y protección de datos parte de la premisa de que los clientes son dueños de sus propios datos, y cualquier producto o servicio se construye con privacy by design desde el inicio. Los tres dominios (AI Responsable, Privacidad, Seguridad) comparten el mismo modelo hub-and-spoke y el mismo proceso de Sensitive Uses, con revisores especializados en cada dominio participando en evaluaciones conjuntas. PyRIT (Python Risk Identification Toolkit) es la herramienta open source del AI Red Team para automatizar evaluaciones de seguridad en sistemas AI.

***

### Recursos oficiales consolidados

| Recurso                     | URL                                                                                                                      |
| --------------------------- | ------------------------------------------------------------------------------------------------------------------------ |
| Responsible AI Hub          | https://www.microsoft.com/en-us/ai/responsible-ai                                                                        |
| Principios y Enfoque        | https://www.microsoft.com/en-us/ai/principles-and-approach                                                               |
| Transparency Report 2025    | https://www.microsoft.com/en-us/corporate-responsibility/responsible-ai-transparency-report/                             |
| RAI Standard v2 (PDF)       | https://msblogs.thesourcemediaassets.com/sites/5/2022/06/Microsoft-Responsible-AI-Standard-v2-General-Requirements-3.pdf |
| Code of Conduct AI Services | https://learn.microsoft.com/en-us/legal/ai-code-of-conduct                                                               |
| RAI Dashboard (Azure ML)    | https://learn.microsoft.com/en-us/azure/machine-learning/concept-responsible-ai-dashboard                                |
| AETHER Committee (Horvitz)  | https://erichorvitz.com/Aether\_Committee\_Microsoft.htm                                                                 |
| Building Blocks blog (2021) | https://blogs.microsoft.com/on-the-issues/2021/01/19/microsoft-responsible-ai-program/                                   |

***

### Conclusión

El programa de AI Responsable de Microsoft es probablemente el más maduro institucional y operacionalmente de la industria, con tres diferenciadores clave frente a competidores como Google. Primero, el **Chief Responsible AI Officer existe desde 2019**, lo que le da casi una década de rodaje. Segundo, la **jerarquía AETHER → ORA → RAISE** es un modelo hub-and-spoke probado, no un comité ad-hoc. Tercero, a diferencia de la actualización de Google en 2025 que eliminó prohibiciones explícitas, Microsoft **mantiene y amplía sus restricciones concretas** (facial recognition, emotional inference).

Para organizaciones que evalúan adopción, los puntos de atención son: la complejidad del proceso de Sensitive Uses puede generar fricción en proyectos de rápida iteración; la distinción entre "Restricted Use" y "Sensitive Use" requiere capacitación interna para aplicarse correctamente; y el modelo de responsabilidad compartida en Azure implica que los clientes deben replicar parte de la gobernanza en su propio entorno, no asumir que Microsoft la cubre completamente.
