# Informe THD: NVIDIA Corporation

**Práctica T03 · Digitalización aplicada a los sectores productivos · Criterio 2.7**

**Autores:** Kyle Cardano  
**Fecha:** 24/11/2026  
**Módulo:** 1º DAW - DIGI  
**Repositorio de GitHub:** [PENDIENTE: enlace al repositorio]

## 1. Datos de la empresa

| Información      | Descripción                                                                                        |
| ---------------- | -------------------------------------------------------------------------------------------------- |
| Nombre           | NVIDIA Corporation                                                                                 |
| Web corporativa  | [NVIDIA España](https://www.nvidia.com/es-es/)                                                     |
| Sector           | TIC. Diseño de semiconductores, software e infraestructura de computación acelerada.               |
| Tamaño           | Gran empresa multinacional.                                                                        |
| Oferta principal | GPU, sistemas de computación y redes para centros de datos, y plataformas de software para IA [1]. |

He elegido NVIDIA porque diseña hardware y software para procesar información y ofrece plataformas que también se utilizan en entornos industriales. Esto permite comparar proyectos propios con aplicaciones en instalaciones de sus clientes.

## 2. Resumen ejecutivo

El informe analiza cuatro tecnologías habilitadoras digitales (THD) en NVIDIA: inteligencia artificial, internet de las cosas, ciberseguridad y computación en la nube. Los casos abarcan la asistencia al diseño de chips, la supervisión de líneas de montaje, el análisis de vulnerabilidades de software y el entrenamiento de modelos en la nube.

En el informe, **IT** se refiere a las aplicaciones, los datos y la infraestructura informática. **OT** se refiere a los equipos y sistemas que supervisan o controlan procesos físicos. El vínculo más directo aparece en Deltia AI: las imágenes de la línea de montaje se convierten en indicadores que el personal consulta en un panel.

## 3. Análisis de las tecnologías habilitadoras digitales

### 3.1. Inteligencia artificial (IA)

**Definición.** Conjunto de técnicas que permiten a un sistema realizar tareas como reconocer patrones, generar texto o interpretar imágenes.

**Características.** Los modelos de aprendizaje automático se entrenan con datos, se pueden adaptar a un dominio y, durante la inferencia, producen resultados a partir de entradas nuevas.

**Aplicación y objetivo de negocio.** NVIDIA Research evaluó ChipNeMo, un modelo de lenguaje adaptado al diseño de chips. Una de las pruebas fue un asistente que respondía a preguntas de ingeniería a partir de documentación especializada. También se evaluó la generación de scripts para herramientas de automatización del diseño electrónico. El proyecto explora cómo reducir el tiempo que el personal dedica a buscar información y preparar tareas de diseño, una actividad central para NVIDIA [2, 3].

**Mejora IT-OT y evidencia.** ChipNeMo es una aplicación de IT confirmada en un proyecto de investigación sobre diseño de hardware. Las fuentes describen pruebas en herramientas de ingeniería. La conexión operativa de la IA se confirma en el caso de Deltia: un modelo de visión interpreta imágenes de la línea y genera marcas temporales que el personal utiliza para localizar cuellos de botella [4].

### 3.2. Internet de las cosas (IoT)

**Definición.** Conexión de dispositivos físicos a una red para recoger, intercambiar o procesar datos sobre su entorno o funcionamiento.

**Características.** Los sensores capturan datos del entorno, los dispositivos conectados transmiten datos y la computación en el borde permite procesarlos cerca de su origen.

**Aplicación y objetivo de negocio.** NVIDIA ofrece módulos Jetson y servicios de software para desplegar aplicaciones en el borde. Deltia AI integra Jetson AGX Orin y NVIDIA Metropolis para procesar vídeo de cámaras instaladas en líneas de montaje. El caso muestra cómo NVIDIA amplía su mercado al suministrar hardware y software a empresas de automatización industrial [4, 5].

**Mejora IT-OT y evidencia.** En el despliegue documentado, las cámaras observan la línea de montaje (OT). Jetson procesa el vídeo junto a la línea y extrae marcas de llegada, trabajo y salida de cada puesto. El panel de Deltia (IT) muestra esa información al personal para comparar tiempos de ciclo y localizar cuellos de botella. El caso confirma la integración para supervisión de la producción [4].

### 3.3. Ciberseguridad

**Definición.** Conjunto de medidas destinadas a proteger sistemas, redes y datos y a preservar su confidencialidad, integridad y disponibilidad.

**Características.** Incluye el control de acceso, la monitorización de eventos y la gestión de vulnerabilidades para priorizar correcciones.

**Aplicación y objetivo de negocio.** NVIDIA documentó Agent Morpheus como ejemplo de IA aplicada al análisis defensivo de vulnerabilidades en software. El sistema ayuda a los analistas a determinar si una vulnerabilidad publicada afecta a un componente y a priorizar su revisión. Esto apoya el mantenimiento seguro del software. La documentación confirma el desarrollo del ejemplo. NVIDIA indica que el soporte de los contenedores de Morpheus dentro de AI Enterprise terminó en enero de 2026 [6, 7, 8].

**Mejora IT-OT y evidencia.** El caso documenta un uso de IT. Como aplicación potencial, el inventario informático podría incorporar versiones del software de las pasarelas industriales (OT). El equipo de seguridad podría revisar qué pasarelas están afectadas y coordinar las actualizaciones con planta en una ventana de mantenimiento. Las fuentes citadas dejan este despliegue industrial sin confirmar [6–8].

### 3.4. Computación en la nube

**Definición.** Modelo que permite acceder por red y bajo demanda a recursos informáticos compartidos, como servidores, almacenamiento y capacidad de cálculo.

**Características.** Los recursos se aprovisionan bajo demanda, la capacidad se ajusta a la carga y el acceso se realiza de forma remota.

**Aplicación y objetivo de negocio.** El caso de Deloitte confirma que Quartz Atlas AI utiliza NVIDIA DGX Cloud en Oracle Cloud Infrastructure para entrenar modelos que trabajan con secuencias químicas y de proteínas. NVIDIA ofrece así acceso remoto a infraestructura de cálculo acelerado para clientes que necesitan entrenar modelos especializados [9, 10].

**Mejora IT-OT y evidencia.** En Deloitte, la mejora documentada se sitúa en IT: el cliente accede a capacidad de cálculo para entrenar modelos. Un uso industrial potencial sería enviar históricos de vibración de una máquina (OT) a la nube (IT) para estudiar patrones de desgaste y devolver alertas al equipo de mantenimiento. El control inmediato de la máquina seguiría en planta. Las fuentes del caso dejan esa integración industrial sin confirmar [9, 10].

## 4. Tabla comparativa de las THD

| THD            | Aplicación documentada                                                 | Mejora y alcance IT-OT                                                                                   |
| -------------- | ---------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| IA             | ChipNeMo en investigación de NVIDIA [2, 3]. Visión en Deltia [4].      | Asistencia al personal de diseño (IT). En Deltia, convierte imágenes de planta en indicadores (OT → IT). |
| IoT            | Jetson y Metropolis en líneas de montaje de clientes de Deltia [4, 5]. | Conecta cámaras de planta con el panel de supervisión (OT → IT).                                         |
| Ciberseguridad | Análisis defensivo de vulnerabilidades con Agent Morpheus [6–8].       | Apoya la priorización de revisiones (IT). Aplicación a pasarelas industriales potencial.                 |
| Nube           | Entrenamiento de modelos en DGX Cloud por Deloitte [9, 10].            | Aporta capacidad de cálculo remota (IT). Análisis de históricos de planta en la nube como uso potencial. |

## 5. Conclusiones

Considero que la **inteligencia artificial** es la THD más determinante para NVIDIA. La IA impulsa la demanda de sus sistemas acelerados y da valor al software y a servicios como DGX Cloud. En el ejercicio fiscal 2026, el mercado de centros de datos aportó unos 193.700 millones de dólares de un total de 215.938 millones, cerca del 90 %. Esa cifra corresponde al conjunto del negocio de centros de datos. NVIDIA atribuye su crecimiento a la computación acelerada y a la IA [1]. Sin la demanda de entrenamiento e inferencia, perderían peso dos usos centrales de su oferta de centros de datos [1, 9].

El caso de Deltia muestra la mejora IT-OT más clara del informe. El personal puede usar datos extraídos de las cámaras para localizar retrasos en la línea. La ciberseguridad y la nube aportan mejoras informáticas demostradas, con aplicaciones industriales potenciales descritas en sus apartados.

## 6. Fuentes

**Fecha de consulta de todas las fuentes:** 24/11/2026.

- [1] NVIDIA. [Informe anual del ejercicio fiscal 2026, resumen de resultados y mercados](https://s201.q4cdn.com/141608511/files/doc_financials/2026/ar/2026-annual-report-web-Hyperlinks.pdf).
- [2] Mingjie Liu y otros, NVIDIA Research. [ChipNeMo: Domain-Adapted LLMs for Chip Design](https://research.nvidia.com/publication/2023-10_chipnemo-domain-adapted-llms-chip-design).
- [3] NVIDIA Blog. [Silicon Volley: Designers Tap Generative AI for a Chip Assist](https://blogs.nvidia.com/blog/llm-semiconductors-chip-nemo/).
- [4] Scott Martin, NVIDIA Blog. [Manufacturing Intelligence: Deltia AI Delivers Assembly Line Gains With NVIDIA Metropolis and Jetson](https://blogs.nvidia.com/blog/deltia-ai-metropolis-jetson/).
- [5] NVIDIA Docs. [Jetson Platform Services](https://docs.nvidia.com/moj/moj-overview.html).
- [6] NVIDIA Technical Blog. [Applying Generative AI for CVE Analysis at an Enterprise Scale](https://developer.nvidia.com/blog/applying-generative-ai-for-cve-analysis-at-an-enterprise-scale).
- [7] NVIDIA Docs. [Morpheus Documentation, versión 25.06](https://docs.nvidia.com/morpheus/).
- [8] NVIDIA Docs. [NVIDIA AI Enterprise Lifecycle Policy: End of Life Notices](https://docs.nvidia.com/ai-enterprise/lifecycle/latest/eol-notices.html).
- [9] NVIDIA. [Construcción de canales de descubrimiento de fármacos con IA generativa: Deloitte](https://www.nvidia.com/es-es/case-studies/generative-ai-in-drug-discovery/).
- [10] Deloitte, sesión de GTC 2024. [Atlas AI: Drug Discovery at the Speed of AI](https://www.nvidia.com/en-us/on-demand/session/gtc24-s62981/).
