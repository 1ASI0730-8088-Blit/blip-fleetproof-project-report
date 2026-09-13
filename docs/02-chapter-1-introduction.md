# Capítulo I: Introducción

## 1.1. Startup Profile

BLIP es una startup tecnológica orientada al desarrollo de productos digitales que buscan simplificar procesos complejos y facilitar la gestión de información relevante para personas y organizaciones. La startup identifica necesidades presentes en procesos que requieren consultar, organizar y dar seguimiento a información proveniente de diferentes fuentes, y las transforma en soluciones digitales centradas en el usuario.

Dentro de este enfoque, BLIP desarrolla FleetProof, un producto digital orientado al seguimiento del estado documentario y administrativo de vehículos y flotas. La propuesta busca facilitar la transformación de consultas puntuales e información dispersa en una experiencia organizada que permita conocer, comparar y dar seguimiento al estado de las unidades.

### 1.1.1. Descripción de la Startup

**Propósito:**

El propósito de BLIP es desarrollar soluciones tecnológicas que simplifiquen procesos complejos y reduzcan el tiempo, esfuerzo e incertidumbre que enfrentan las personas y organizaciones en sus actividades cotidianas. Para ello, la startup busca identificar problemas concretos y transformarlos en experiencias digitales que faciliten la gestión de información y la toma de decisiones.

**Misión:**

La misión de BLIP es crear productos digitales innovadores, accesibles y confiables que permitan a personas y organizaciones gestionar información y procesos de manera más eficiente, contribuyendo a una toma de decisiones más informada y orientada a sus necesidades.

**Visión:**

La visión de BLIP es consolidarse como una startup tecnológica reconocida por desarrollar soluciones digitales innovadoras que transformen procesos tradicionales mediante experiencias centradas en las necesidades de sus usuarios y que generen valor sostenible.

**Propuesta de valor:**

La propuesta de valor de BLIP se basa en identificar necesidades reales y convertir procesos que actualmente pueden involucrar tareas manuales, información dispersa o consultas aisladas en experiencias digitales simples, organizadas y orientadas al usuario.

La startup busca generar valor mediante productos tecnológicos que reduzcan tareas innecesarias, centralicen información relevante y faciliten el seguimiento de procesos y situaciones que requieren atención. Su propuesta combina tecnología, innovación y comprensión de las necesidades de los usuarios para desarrollar productos útiles, escalables y capaces de evolucionar de acuerdo con las necesidades identificadas.

En este marco, FleetProof representa la aplicación de esta propuesta al ámbito de la gestión vehicular, buscando facilitar el seguimiento del estado documentario y administrativo de vehículos y flotas mediante información organizada, trazable y orientada a la toma de decisiones.

**Modelo de Negocio:**

BLIP plantea un modelo de negocio basado en el desarrollo y comercialización de productos digitales propios, buscando generar ingresos de manera independiente y sostenible sin depender exclusivamente de proyectos personalizados o de terceros.

La startup apuesta por modelos digitales escalables, en los que sus productos puedan atender progresivamente a un mayor número de usuarios sin que los costos de operación aumenten proporcionalmente. Asimismo, busca establecer fuentes de ingresos recurrentes, como suscripciones y otros servicios digitales, que permitan financiar el mantenimiento, evolución y expansión de sus productos.

Este enfoque permite que BLIP desarrolle productos propios con capacidad de crecimiento progresivo y que cada solución pueda evolucionar a partir de las necesidades y comportamiento de sus usuarios.

**Identidad visual de BLIP:**

La identidad visual de BLIP se representa mediante el logotipo oficial de la startup, el cual se incorpora como parte de la presentación de la organización.

![Logotipo oficial de BLIP](assets/chapter-1/logo-blip.png)

### 1.1.2 Perfiles de integrantes del equipo

| Integrante | Código | Carrera | Perfil técnico | Aporte al equipo |
|---|---|---|---|---|
| Reyes Limo Sebastian | u2022311656 | Ingeniería de Software | TODO | Technical Lead, SCM and Rubric Owner |
| Palomino Murga Daniel Stalin | U20201B253 | Ingeniería de Software | TODO | Lean UX Owner |
| Becerra Durand Sebastian Uriel | TODO | Ingeniería de Software | TODO | UX Research Owner |
| Gómez De La Torre Huertas Rodrigo Fernando | TODO | Ingeniería de Software | TODO | Requirements Owner |
| Payesa Torres Harrison Hubert | TODO | Ingeniería de Software | TODO | Product Design and Landing Page Owner |

## 1.2. Solution Profile

FleetProof es una plataforma web orientada al monitoreo documentario y administrativo de vehículos, diseñada para facilitar la consulta, consolidación, comparación y seguimiento de información proveniente de diferentes fuentes relacionadas con el estado de vehículos y flotas.

La solución está dirigida principalmente a empresas que administran flotas pequeñas y medianas, cuyos responsables necesitan conocer el estado de sus unidades, identificar observaciones y priorizar acciones de seguimiento. Como segmento complementario, FleetProof considera a propietarios, compradores y conductores independientes que requieren consultar y continuar monitoreando la información asociada a uno o pocos vehículos.

A diferencia de una consulta puntual orientada únicamente a obtener un reporte, FleetProof propone extender el proceso hacia un esquema de monitoreo recurrente. Para ello, la solución contempla el registro de resultados y evidencias por fuente, la comparación de diferentes estados de un vehículo, la generación de alertas y el seguimiento de observaciones mediante responsables y evidencias de resolución.

El alcance inicial se concentra en la gestión de información documentaria y administrativa relacionada con los vehículos. FleetProof no contempla convertirse en una plataforma de GPS o telemetría, ni administrar combustible, mantenimiento mecánico o sensores del vehículo. Asimismo, el MVP no busca automatizar todas las fuentes existentes, sino trabajar inicialmente con un número limitado de conectores o proveedores de prueba y mantener una arquitectura que permita incorporar nuevas fuentes posteriormente.

### 1.2.1. Antecedentes y problemática

| Técnica | Pregunta aplicada al problema | Sustento |
|---|---|---|
| Who | ¿Quién experimenta el problema? | Empresas que administran flotas de vehículos, en las que las actividades de consulta y seguimiento pueden involucrar a responsables de gestión de flota, control documentario o control operativo, dependiendo del tipo de servicio y de la organización interna. Asimismo, el problema puede involucrar a propietarios y conductores independientes que administran uno o pocos vehículos y necesitan verificar información relacionada con su documentación, habilitación, infracciones u otras condiciones asociadas al vehículo. |
| What | ¿Qué problema ocurre? | Los usuarios necesitan verificar diferentes tipos de información según las características y el servicio del vehículo. Entre los principales elementos se encuentran la vigencia del Seguro Obligatorio de Accidentes de Tránsito (SOAT), el Certificado de Inspección Técnica Vehicular (CITV), habilitaciones y autorizaciones correspondientes al servicio, así como infracciones y órdenes de captura. El MTC establece, por ejemplo, la necesidad de verificar el CITV y, según el procedimiento, documentación como SOAT y autorizaciones o permisos especiales; asimismo, existen procedimientos específicos de habilitación vehicular para servicios de transporte. (Ministerio de Transportes y Comunicaciones [MTC], 2024, 2022). |
| Where | ¿Dónde ocurre? | El problema se plantea inicialmente en el contexto peruano, particularmente en actividades relacionadas con el transporte terrestre de personas, mercancías y otros servicios sujetos a requisitos de habilitación, documentación y fiscalización. La información que debe verificarse se encuentra distribuida entre diferentes servicios digitales. Por ejemplo, el MTC dispone de un sistema de consulta del CITV, SUTRAN ofrece una plataforma para consultar el récord de infracciones y el SAT dispone de servicios para consultar papeletas y órdenes de captura vehicular. (MTC, 2026; Superintendencia de Transporte Terrestre de Personas, Carga y Mercancías [SUTRAN], 2026; Servicio de Administración Tributaria de Lima [SAT], s. f.). |
| When | ¿Cuándo y con qué frecuencia ocurre? | La necesidad de revisión se presenta en diferentes momentos según el tipo de vehículo, servicio y condición que se desea verificar. Puede producirse antes de iniciar determinadas operaciones o viajes y de manera periódica para comprobar la vigencia de documentos y autorizaciones. La periodicidad no es uniforme: por ejemplo, SUTRAN señala que los vehículos particulares deben realizar la inspección técnica una vez al año, mientras que los destinados al transporte de personas y materiales o residuos peligrosos deben hacerlo cada seis meses. (SUTRAN, 2026). |
| Why | ¿Por qué es relevante resolverlo? | La revisión permite identificar condiciones que pueden afectar la posibilidad de utilizar un vehículo para determinados servicios, así como detectar infracciones, documentos vencidos u otras observaciones que requieren atención. La relevancia de estas condiciones se evidencia en las actividades de fiscalización: durante el primer semestre de 2026, la ATU reportó 3003 vehículos enviados al depósito, incluyendo unidades sin SOAT y sin revisión técnica vigente. (Autoridad de Transporte Urbano para Lima y Callao [ATU], 2026). |
| How | ¿Cómo se resuelve actualmente? | De manera preliminar, la revisión se realiza mediante consultas en los diferentes portales y servicios digitales disponibles para cada fuente. Estos servicios pueden requerir consultas independientes utilizando datos como la placa del vehículo. Actualmente existen, por ejemplo, sistemas separados para consultar el CITV, el récord de infracciones y las órdenes de captura vehicular. La forma en que los usuarios consolidan, registran y realizan seguimiento de los resultados obtenidos será validada mediante la investigación con usuarios. |
| How Much | ¿Cuánto tiempo, costo o impacto implica? | El esfuerzo asociado a este proceso aún requiere ser cuantificado. De manera preliminar, la necesidad de consultar diferentes fuentes podría generar trabajo repetitivo, especialmente cuando se administran múltiples vehículos. Sin embargo, el tiempo empleado por consulta, la frecuencia de revisión, el número de fuentes consultadas y el impacto económico u operativo serán variables a medir durante la investigación con usuarios. |

**Objetivos y límites del proyecto**

El objetivo de FleetProof es facilitar la investigación y el monitoreo del estado documentario y administrativo de vehículos, mediante mecanismos que permitan consolidar resultados provenientes de diferentes fuentes, comparar cambios y realizar seguimiento de observaciones.

Como objetivos específicos, la solución busca:

- centralizar los resultados obtenidos a partir de diferentes fuentes de consulta;
- registrar la fuente, fecha y evidencia asociada a cada resultado;
- permitir la comparación entre diferentes estados registrados de un vehículo;
- facilitar la identificación y priorización de observaciones;
- proporcionar mecanismos para asignar responsables y registrar evidencias de resolución;
- ofrecer una visualización consolidada para la gestión de vehículos individuales y flotas.

El alcance inicial se limita a la gestión de información documentaria y administrativa relacionada con los vehículos. El MVP no contempla funcionalidades de GPS, telemetría, sensores, combustible o mantenimiento mecánico, ni el desarrollo de una aplicación móvil nativa. Tampoco se plantea automatizar todas las fuentes disponibles; inicialmente se trabajará con un número limitado de conectores o proveedores de prueba, manteniendo una arquitectura que permita incorporar nuevas fuentes posteriormente.

Asimismo, FleetProof no se presentará como una fuente oficial ni reemplazará los certificados o consultas de las entidades públicas correspondientes.

### 1.2.2 Lean UX Process

#### 1.2.2.1 Lean UX Problem Statement

El estado actual de la verificación documentaria vehicular en Perú se concentra en consultas aisladas realizadas sobre múltiples portales y reportes individuales orientados principalmente a compraventa. Los productos existentes no cubren suficientemente el monitoreo continuo, la comparación histórica, la gestión colaborativa de observaciones y la consolidación del riesgo de una flota. FleetProof cubrirá esta brecha mediante una plataforma que registra vehículos, organiza consultas por fuente, genera reportes trazables y alerta cambios que puedan afectar la operación. El foco inicial serán empresas con flotas pequeñas y medianas; el segundo segmento serán propietarios y compradores particulares. El éxito se evidenciará mediante menor tiempo de preparación, detección temprana y uso recurrente.

#### 1.2.2.2 Lean UX Assumptions

##### Business Assumptions

- Las empresas pagarán por reducir trabajo manual y riesgo operativo.
- El monitoreo recurrente generará mayor retención que el reporte unitario.
- Los planes por volumen de vehículos y reportes permitirán escalar el modelo de negocio.

##### Business Outcome Assumptions

- Aumentará el porcentaje de clientes que genera un segundo reporte.
- Disminuirá el tiempo promedio de preparación y revisión.
- Aumentará el porcentaje de observaciones con responsable y evidencia.

##### User Assumptions

- Los administradores de flota combinan portales, hojas de cálculo y mensajería.
- Los supervisores necesitan resumen de riesgo y trazabilidad.
- Los particulares tienen dificultad para interpretar resultados registrales.

##### User Outcome and Benefit Assumptions

- Los usuarios identificarán unidades críticas rápidamente.
- Los usuarios evitaran repetir consultas y perder evidencias.
- Los usuarios comprenderán cambios y regularizaran observaciones.

##### Feature Assumptions

- La carga CSV reducirá esfuerzo de adopción empresarial.
- El checklist por fuente reducirá omisiones.
- La comparación de snapshots hará visible información nueva.
- El semáforo con explicación facilitará la priorización.
- Los casos con responsable y evidencia mejorarán seguimiento.
- Los planes con límites reales sostendrán monetización.

#### 1.2.2.3 Lean UX Hypothesis Statements

TODO: Redactar un hypothesis statement por cada Feature Assumption usando:

```text
We believe we will achieve [this business outcome]
If [these personas]
Attain [this benefit/user outcome]
With [this feature or solution]
```

#### 1.2.2.4 Lean UX Canvas

TODO: Insertar captura del Lean UX Canvas y explicar aprendizajes.

## 1.3 Segmentos objetivo

### Empresas con flotas

Empresas de taxi, buses, turismo, reparto, logística, alquiler y servicios con aproximadamente 5 a 100 unidades.

### Propietarios y compradores particulares

Personas que compran, venden o administran uno o pocos vehículos, incluidos conductores independientes y taxistas propietarios.
