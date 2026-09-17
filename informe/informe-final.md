# Informe Final: Análisis de Calidad de Software en Stellar y Drips
## Aplicado al Proyecto Hub Mixteca — Costuras de Tijaltepec
## 1. Introducción General

El proyecto Hub Mixteca busca atender la falta de canales de comercialización y visibilidad de mercado de Costuras de Tijaltepec, un taller que actualmente realiza sus actividades de venta y gestión de pedidos principalmente de manera presencial. La solución propuesta contempla herramientas digitales para aumentar la visibilidad del taller, facilitar la consulta de productos y permitir el seguimiento de pedidos, complementando —no sustituyendo— la tienda física.

Para fundamentar los requisitos de calidad de esta solución, el presente informe analiza dos plataformas tecnológicas de código abierto del ecosistema blockchain: **Stellar**, una red orientada a operaciones con activos digitales y transferencias, y **Drips**, un protocolo descentralizado que financia proyectos de software libre mediante mecanismos de distribución continua de fondos (streaming).

El objetivo no es implementar la infraestructura de Stellar o Drips dentro de Hub Mixteca, sino utilizar el análisis de ambas plataformas como referencia técnica para identificar y adaptar requisitos de calidad —seguridad, fiabilidad, trazabilidad, transparencia y verificabilidad— a las necesidades reales del taller y de los usuarios de la región Mixteca.

El informe se organiza en cuatro bloques: (1) desempeño técnico de Stellar, (2) desempeño técnico de Drips, (3) adaptación al contexto de la Mixteca y pensamiento crítico sobre riesgos éticos y de seguridad, y (4) integración interdisciplinaria entre ingeniería de software y economía Web3.

---

## 2. Desempeño Técnico: Stellar

### 2.1 Análisis técnico de Stellar

**Stellar Consensus Protocol (SCP).** Stellar utiliza el Stellar Consensus Protocol para alcanzar consenso entre los participantes de la red, permitiendo que los nodos lleguen a un acuerdo sobre el estado de la información registrada. Desde la calidad de software, esto permite analizar características como consistencia de la información, fiabilidad, disponibilidad, integridad de los registros y tolerancia ante fallos de determinados participantes. Para Hub Mixteca, estos conceptos sirven como referencia para mantener información consistente sobre las operaciones que realmente requieran trazabilidad o verificación.

**Activos digitales.** Stellar permite representar diferentes tipos de activos digitales, incluyendo activos tradicionales y tokens, lo que permite estudiar cómo una infraestructura digital puede representar operaciones de manera verificable. En Hub Mixteca esta posibilidad se considera únicamente como referencia; no se propone convertir automáticamente los productos textiles o los pedidos de Costuras de Tijaltepec en activos digitales.

**Trazabilidad e integridad.** Las redes blockchain permiten mantener registros verificables de determinadas operaciones. Para Hub Mixteca esto se relaciona con la necesidad de mantener información confiable sobre los pedidos, por ejemplo mediante identificadores y estados de pedido que faciliten su seguimiento. El uso de blockchain debe limitarse a la información que realmente necesite integridad, trazabilidad o verificabilidad.

### 2.2 Gestión de código abierto en Stellar

Stellar se desarrolla mediante un ecosistema de código abierto donde el código y la documentación pública permiten que diferentes participantes estudien, revisen y contribuyan a la tecnología. Esto sirve como referencia para aplicar prácticas de ingeniería de software como control de versiones, registro de cambios, documentación, revisión del código, evidencias del desarrollo y seguimiento de modificaciones, mejorando la trazabilidad del propio desarrollo del proyecto Hub Mixteca.

### 2.3 Requerimientos de calidad identificados en Stellar

| Requerimiento | Referencia en Stellar | Aplicación en Hub Mixteca |
|---|---|---|
| Seguridad | Protección de operaciones y activos | Protección de información del taller y pedidos |
| Fiabilidad | Consenso entre participantes | Información consistente de los pedidos |
| Integridad | Registros verificables | Protección de información importante |
| Trazabilidad | Seguimiento de operaciones | Seguimiento mediante identificadores de pedido |
| Verificabilidad | Información registrada en la red | Verificación de datos seleccionados |
| Rendimiento | Procesamiento de operaciones | Sistema ligero y adecuado para dispositivos móviles |
| Mantenibilidad | Desarrollo y documentación pública | Código y documentación organizados |

### 2.4 Seguridad y fiabilidad

La seguridad es fundamental en una red blockchain porque las operaciones pueden involucrar activos digitales y registros que deben mantenerse íntegros. El análisis de Stellar permite considerar controles de calidad relacionados con validación de operaciones, integridad de los datos, consistencia de la información, control de acceso, registro de cambios y manejo de errores. Para Hub Mixteca, estos principios aplican a la gestión de información de Costuras de Tijaltepec, en particular a la información de pedidos, que debe mantenerse consistente para evitar errores en estados, fechas, anticipos y saldos.

### 2.5 Adaptación al proyecto

El problema principal identificado en Costuras de Tijaltepec es la **falta de canales de comercialización y visibilidad de mercado**. Entre las funciones consideradas para la solución se encuentran: perfil digital verificable del taller, información de productos, fotografías optimizadas, información de contacto, seguimiento de pedidos, identificación de los pedidos y consulta del estado del pedido. El análisis de Stellar permite relacionar estas funciones con los requisitos de seguridad, fiabilidad, trazabilidad y verificabilidad.

La solución también debe adaptarse a las condiciones reales de la región Mixteca: uso desde dispositivos móviles, interfaz sencilla, bajo consumo de recursos, fotografías optimizadas, facilidad de navegación y funcionamiento adecuado considerando las condiciones de conectividad. El uso de blockchain no debe aumentar innecesariamente la complejidad del sistema.

Para Hub Mixteca, blockchain se considera útil cuando proporcione un beneficio concreto de integridad, trazabilidad o verificabilidad. No se considera necesario almacenar fotografías, catálogos completos u otros archivos pesados directamente en blockchain; esta puede reservarse para los datos que realmente requieran verificación.

---

## 3. Desempeño Técnico: Drips

### 3.1 Análisis técnico de Drips

**Funcionamiento general.** Drips es un protocolo descentralizado construido sobre Ethereum que permite distribuir fondos hacia proyectos de software libre, repositorios de GitHub, direcciones de Ethereum y otras listas de distribución, utilizando estructuras denominadas *Drip Lists* para establecer los destinatarios. Esta característica permite analizar la importancia de mantener información organizada y trazable dentro de un sistema digital.

**Streaming de fondos.** Drips utiliza el concepto de streaming para realizar transferencias continuas de fondos durante un periodo determinado, mediante reglas que establecen la cantidad distribuida y el periodo de distribución. Para Hub Mixteca, este mecanismo se considera una referencia para analizar cómo un sistema puede manejar operaciones de manera programada y verificable, sin proponer utilizar streaming de fondos directamente para los pedidos de Costuras de Tijaltepec sin antes analizar requisitos, costos y riesgos.

**Contratos inteligentes.** Los contratos inteligentes contienen las reglas que administran las operaciones del protocolo. Dado que estas operaciones involucran activos digitales, la seguridad y fiabilidad de los contratos son requisitos importantes. Para Hub Mixteca, esto resalta la importancia de validar las reglas de negocio antes de incorporarlas a cualquier solución tecnológica.

### 3.2 Gestión de código abierto en Drips

Drips mantiene documentación y código de manera pública, lo que permite consultar los componentes del proyecto y revisar su evolución mediante control de versiones. Como referencia para Hub Mixteca, esto incluye prácticas como control de versiones, registro de commits, documentación, revisión de cambios, trazabilidad y evidencias del desarrollo.

### 3.3 Requerimientos de calidad identificados en Drips

| Requerimiento | Referencia en Drips | Aplicación en Hub Mixteca |
|---|---|---|
| Seguridad | Protección de contratos y operaciones | Protección de información y pedidos |
| Fiabilidad | Correcta ejecución de las reglas | Estados de pedidos consistentes |
| Trazabilidad | Registro de operaciones y cambios | Identificador y seguimiento de pedidos |
| Transparencia | Código y documentación públicos | Información clara para compradores |
| Verificabilidad | Operaciones basadas en reglas programadas | Verificación de información seleccionada |
| Mantenibilidad | Código organizado y versionado | Mantenimiento de la solución |
| Auditabilidad | Revisión y auditorías del protocolo | Revisión de cambios y evidencias |

*Estas características corresponden al análisis de calidad realizado para este informe y no deben interpretarse como una lista oficial de métricas publicada por Drips.*

### 3.4 Seguridad y fiabilidad

La seguridad es especialmente importante en Drips debido al uso de contratos inteligentes relacionados con la distribución de activos digitales. La documentación oficial describe el uso de pruebas, *fuzzing*, auditorías externas y otros mecanismos para analizar la seguridad del protocolo, permitiendo identificar posibles errores y vulnerabilidades. Para Hub Mixteca, estos principios aplican considerando integridad de los datos, protección de la información, control de modificaciones, validación de datos, registro de operaciones y manejo de errores.

### 3.5 Adaptación al proyecto y uso responsable de blockchain

Las características observadas en Drips —trazabilidad, transparencia, verificabilidad, seguridad y registro de operaciones— pueden tomarse como referencia para definir requisitos de calidad del sistema de Hub Mixteca. Sin embargo, no todas las funciones requieren blockchain: su uso debe justificarse únicamente cuando proporcione un beneficio concreto. No se considera conveniente almacenar fotografías u otros archivos pesados directamente en blockchain; estos pueden usar mecanismos de almacenamiento convencionales, reservando blockchain para la información que realmente necesite verificabilidad.

---

## 4. Adaptación a Contextos Complejos y Pensamiento Crítico

### 4.1 Contexto del proyecto

Costuras de Tijaltepec realiza actualmente sus actividades de venta y gestión de pedidos principalmente de manera presencial. La solución digital busca complementar la tienda física mediante un canal que muestre información del taller y facilite la interacción con compradores, reduciendo la dependencia de la atención presencial y facilitando la consulta de información.

### 4.2 Adaptación al contexto de la región Mixteca

La solución debe considerar las condiciones tecnológicas reales de los usuarios de la región: uso desde dispositivos móviles, conectividad limitada, interfaz ligera y fotografías optimizadas. Por ello, los requisitos de calidad deben incluir usabilidad, accesibilidad, rendimiento, optimización de imágenes, compatibilidad con dispositivos móviles y facilidad de navegación.

### 4.3 Relación con Stellar y Drips

Stellar utiliza un protocolo de consenso para mantener un estado consistente de la red; Drips utiliza contratos inteligentes para establecer reglas de distribución de fondos. El análisis de ambas plataformas resalta la importancia de establecer reglas claras, mecanismos de verificación y controles de seguridad. Sin embargo, Hub Mixteca no necesita incorporar toda la infraestructura de ninguna de las dos: la tecnología debe seleccionarse de acuerdo con las necesidades reales del proyecto.

### 4.4 Pensamiento crítico sobre blockchain

Blockchain no debe considerarse automáticamente como solución para todos los problemas tecnológicos; su incorporación debe estar justificada por un requisito concreto. En Hub Mixteca, los posibles beneficios identificados son integridad, trazabilidad y verificabilidad. Si una función no requiere estas características, puede utilizar tecnologías convencionales más sencillas, reduciendo complejidad y evitando el uso innecesario de blockchain.

### 4.5 Riesgos de seguridad

El sistema manejará información de talleres, productos, compradores y pedidos, incluyendo anticipos y saldos pendientes. Los riesgos identificados son:

| Riesgo | Posible consecuencia | Medida de calidad |
|---|---|---|
| Alteración de información | Pérdida de confianza | Control de cambios |
| Datos incompletos | Errores en pedidos | Validación de información |
| Modificación incorrecta de anticipos | Conflictos con compradores | Protección de registros |
| Información desactualizada | Confusión del comprador | Actualización de datos |
| Imágenes demasiado pesadas | Dificultad de acceso | Optimización |
| Problemas de conectividad | Dificultad para consultar | Interfaz ligera |

### 4.6 Consideraciones éticas

El sistema debe proporcionar información clara sobre las operaciones que realiza y los datos que registra, de modo que los usuarios comprendan qué información se utiliza y con qué finalidad. Debe evitarse presentar blockchain como una garantía absoluta de seguridad: la transparencia implica explicar claramente las características y limitaciones reales de la tecnología utilizada.

### 4.7 Auditoría y código abierto

El análisis de Stellar y Drips evidencia la importancia de las pruebas, revisiones y auditorías en proyectos de código abierto. En Hub Mixteca pueden aplicarse principios similares mediante control de versiones, commits identificables, documentación, revisión de cambios, pruebas, evidencias y registro de decisiones, manteniendo trazabilidad sobre la evolución de la solución.

### 4.8 Criterios de calidad adaptados al contexto

| Criterio | Aplicación en Hub Mixteca |
|---|---|
| Seguridad | Protección de información y registros |
| Usabilidad | Interfaz sencilla para compradores y taller |
| Accesibilidad | Uso desde dispositivos móviles |
| Rendimiento | Contenido ligero e imágenes optimizadas |
| Fiabilidad | Información correcta sobre pedidos |
| Trazabilidad | Identificadores y registros |
| Verificabilidad | Comprobación de información seleccionada |
| Transparencia | Información clara para los usuarios |

---

## 5. Integración Interdisciplinaria

### 5.1 Ingeniería de software y el problema del proyecto

La ingeniería de software permite transformar una problemática real en requisitos y funcionalidades concretas. En Costuras de Tijaltepec, la necesidad identificada es mejorar la visibilidad del taller y facilitar la gestión y consulta de pedidos, por lo que la solución debe partir de las necesidades del taller y de los compradores antes de seleccionar cualquier tecnología.

### 5.2 Calidad de software: síntesis general

| Característica | Aplicación en el proyecto |
|---|---|
| Usabilidad | Consulta sencilla de productos y pedidos |
| Seguridad | Protección de información y anticipos |
| Fiabilidad | Información correcta sobre los pedidos |
| Rendimiento | Interfaz ligera e imágenes optimizadas |
| Trazabilidad | Identificación y seguimiento de pedidos |
| Verificabilidad | Comprobación de información seleccionada |
| Mantenibilidad | Código y documentación organizados |

### 5.3 Financiamiento on-chain y streaming (economía Web3)

El financiamiento on-chain utiliza infraestructura blockchain para registrar y ejecutar determinadas operaciones relacionadas con activos digitales; en Drips, los contratos inteligentes participan en las reglas de distribución de fondos. Para Hub Mixteca, este concepto se analiza como referencia para operaciones que requieran trazabilidad o verificación, pero los anticipos de Costuras de Tijaltepec no deben convertirse automáticamente en operaciones blockchain sin antes analizar requisitos, costos, seguridad, facilidad de uso y beneficios reales.

De manera similar, el streaming de Drips —transferencias continuas de fondos mediante reglas programadas— demuestra cómo el software puede gestionar operaciones económicas mediante reglas de negocio, seguridad, estados, trazabilidad, manejo de errores y control de costos. En Hub Mixteca, el streaming se toma principalmente como referencia conceptual para estudiar nuevas formas de representar reglas de negocio mediante tecnología Web3, no como una funcionalidad a implementar de inmediato.

### 5.4 Relación interdisciplinaria (modelo conceptual)

\`\`\`
Ingeniería de software
        ↓
Requisitos de calidad
        ↓
Solución digital para Costuras de Tijaltepec
        ↓
Blockchain cuando sea necesario
        ↓
Integridad / trazabilidad / verificabilidad
        ↓
Stellar y Drips como referencias
        ↓
Economía Web3
        ↓
Financiamiento on-chain y streaming
\`\`\`

### 5.5 Aplicación al proyecto

La integración interdisciplinaria se mantiene subordinada a la problemática principal: **falta de canales de comercialización y visibilidad de mercado**. La solución contempla un perfil digital del taller, información de productos y seguimiento de pedidos, por lo que: las fotografías deben mantenerse optimizadas; la información del perfil debe ser clara; los pedidos deben contar con trazabilidad; los registros de anticipos deben mantenerse protegidos; la información que requiera verificación puede analizarse para usar blockchain; y la tienda física continúa formando parte del modelo de atención.

### 5.6 Integración con los criterios de la rúbrica

| Criterio de la rúbrica | Relación con el proyecto |
|---|---|
| Desempeño técnico | Análisis técnico de Stellar y Drips |
| Adaptación a situaciones complejas | Aplicación al contexto de la Mixteca |
| Pensamiento crítico | Análisis de riesgos, seguridad y ética |
| Actividades interdisciplinarias | Ingeniería de software, blockchain y economía Web3 |
| Calidad | Seguridad, fiabilidad, rendimiento, usabilidad y trazabilidad |

---

## 6. Conclusiones Generales

El análisis técnico de Stellar y Drips permitió identificar características de calidad transferibles al proyecto Hub Mixteca: consenso, seguridad, integridad, fiabilidad, trazabilidad, transparencia y verificabilidad. Stellar aportó una referencia sobre infraestructura blockchain, consenso distribuido y representación de activos digitales; Drips aportó una referencia sobre mecanismos de financiamiento de proyectos de software libre, distribución de fondos y streaming, además de evidenciar buenas prácticas de auditoría y gestión de código abierto.

La adaptación de estos conceptos al contexto de la región Mixteca mostró que los requisitos de calidad deben priorizar usabilidad, accesibilidad, rendimiento y trazabilidad por encima de la sofisticación tecnológica, y que el uso de blockchain solo se justifica cuando aporta un beneficio concreto de integridad, trazabilidad o verificabilidad — nunca como incorporación obligatoria por tratarse de una tecnología descentralizada.

Finalmente, la integración interdisciplinaria entre ingeniería de software y economía Web3 —representada en el modelo conceptual y en casos reales como el programa de financiamiento de Drips hacia proyectos de Stellar— confirma que la calidad del software y los mecanismos de financiamiento están relacionados, pero ambos deben mantenerse al servicio del objetivo central del proyecto: **resolver la falta de canales de comercialización y visibilidad de mercado de Costuras de Tijaltepec**.

---

## 7. Referencias

- Stellar Development Foundation. *Stellar Developer Documentation*.
- Stellar Development Foundation. *Stellar Consensus Protocol*.
- Stellar Development Foundation. *Stellar Assets and Tokenization*.
- Drips Documentation. *Introduction*.
- Drips Documentation. *Overview*.
- Drips Documentation. *Drips Inner Workings*.
- Drips Documentation. *Security*.
- Drips Documentation. *Drip Lists*.
- INEGI. *Encuesta Nacional sobre Disponibilidad y Uso de Tecnologías de la Información en los Hogares (ENDUTIH)*.
- Documentación y validación del proyecto Hub Mixteca.
