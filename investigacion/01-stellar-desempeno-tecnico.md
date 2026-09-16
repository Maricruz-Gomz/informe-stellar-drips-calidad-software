# 01. Desempeño técnico — Stellar

## 1. Introducción

Stellar es una red blockchain pública y de código abierto orientada a
facilitar operaciones financieras digitales. Su funcionamiento utiliza
el Stellar Consensus Protocol (SCP), basado en el modelo Federated
Byzantine Agreement (FBA).

El análisis de Stellar desde la ingeniería de software permite estudiar
aspectos como seguridad, fiabilidad, rendimiento, mantenibilidad,
pruebas y gestión del código abierto.

## 2. Análisis técnico de Stellar

### 2.1 Arquitectura y consenso

El consenso de Stellar se realiza mediante el Stellar Consensus Protocol
(SCP). Los nodos participantes seleccionan los nodos en los que confían
para alcanzar acuerdos sobre el estado del libro mayor.

De acuerdo con la documentación oficial de Stellar, SCP busca propiedades
como:

- Tolerancia a fallos.
- Seguridad.
- Liveness o capacidad de continuar alcanzando acuerdos.

La tolerancia a fallos se relaciona con la capacidad del sistema para
continuar funcionando ante fallos de nodos. La seguridad busca evitar
que diferentes nodos acepten estados contradictorios y el liveness se
relaciona con la capacidad de alcanzar nuevos acuerdos.

### 2.2 Seguridad

La seguridad es un requisito fundamental porque Stellar procesa
operaciones financieras. El mecanismo de consenso debe permitir que
los participantes lleguen a un estado consistente del libro mayor y
evitar problemas como la aceptación de estados incompatibles.

Por ello, la seguridad debe analizarse junto con los mecanismos de
consenso, validación de transacciones, pruebas y revisión del software.

### 2.3 Fiabilidad

La fiabilidad puede analizarse mediante la capacidad de los componentes
de Stellar para mantener un funcionamiento consistente ante diferentes
condiciones y fallos.

La documentación de desarrollo de stellar-core indica que existen
pruebas automatizadas y herramientas para ejecutar la suite de pruebas.
También se recomienda comprobar que las pruebas pasen antes de enviar
cambios al proyecto.

### 2.4 Rendimiento

El rendimiento es importante en una red distribuida porque las
modificaciones realizadas en el software pueden afectar el procesamiento
de operaciones.

El repositorio de stellar-core establece que los cambios que puedan
afectar el rendimiento deben acompañarse de evidencia que permita
identificar mejoras o evitar regresiones.

## 3. Gestión de código abierto

Stellar mantiene repositorios públicos y proporciona mecanismos para
que la comunidad pueda contribuir al software.

Las instrucciones oficiales de contribución de stellar-core indican que
los cambios se realizan mediante forks y Pull Requests. También se
recomienda mantener los cambios enfocados en un solo problema y separar
los cambios lógicamente diferentes.

En el caso de Stellar Docs, su documentación de contribución también
indica que las Pull Requests deben ser revisadas y aprobadas antes de
fusionarse.

Esto permite relacionar la gestión de código abierto con prácticas de
calidad como:

- Revisión por pares.
- Control de versiones.
- Seguimiento de cambios.
- Pruebas.
- Revisión antes de integrar modificaciones.

## 4. "requerimientos/métricas aplicables al análisis

| Requerimiento | Aplicación en Stellar |
|---|---|
| Seguridad | Protección de la integridad del sistema y de las operaciones |
| Fiabilidad | Funcionamiento consistente ante fallos |
| Rendimiento | Evaluación de cambios que puedan producir regresiones |
| Mantenibilidad | Código organizado y cambios separados por objetivo |
| Trazabilidad | Historial de commits, Issues y Pull Requests |
| Verificación | Ejecución de pruebas antes de integrar cambios |
| Revisión | Revisión de Pull Requests antes de fusionar |

## 5. Seguridad y fiabilidad

La seguridad y la fiabilidad están relacionadas con la capacidad de
Stellar para mantener un estado consistente de la red y continuar
funcionando ante determinados fallos.

La documentación de stellar-core incluye pruebas automatizadas,
herramientas de diagnóstico y mecanismos como sanitizers y cobertura
de código para apoyar la detección de problemas durante el desarrollo.

Estas prácticas muestran que la calidad no depende únicamente del
funcionamiento de la blockchain, sino también del proceso utilizado
para desarrollar, probar y revisar el software.

## 6. Referencias

- Stellar. Stellar Consensus Protocol.
- Stellar Development Foundation / Stellar Docs. Stellar Consensus Protocol.
- Stellar. stellar-core — CONTRIBUTING.md.
- Stellar. stellar-docs — CONTRIBUTING.md.
