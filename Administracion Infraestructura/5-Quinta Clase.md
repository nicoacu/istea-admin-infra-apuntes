#cmdb #gobierno_it

## Qué es un CMDB y para qué sirve?

El CMDB (configuration management database) es una base de datos que contiene toda la información relevante acerca de los activos de hardware y software (llamados configuration items - "CI") utilizados dentro de la organización.

El CMDB provee una vista organizada y detallada de cada activo de IT y la relación entre este y los demás. Nos permite entender e identificar activos que son críticos para la organización y sus características e interrelaciones.

El sistema permite registrar información como: ubicación, responsable, criticidad, tipo de elemento, modelo, etc... también nos permite cargar detalles técnicos como: versión de SO/Firmware, direcciones IP, fecha de EoL/EoS, etc...

> "Hay CIs que tienen como característica tener direcciones IP." 

## Por qué un CMDB es importante?

Cada vez mas la infraestructura de IT se vuelve más compleja por lo que se vuelve necesario identificar y entender cada vez mas información de estos dispositivos.

Permite inventariar los activos, no solo a nivel técnico, sino a nivel de servicio, dentro de la organización (responsable, ubicación, servicio afectado, criticidad, nivel de SLA, etc).

Ejemplos de CIs:

- **Hardware**: PCs, impresoras, routers, switches, notebooks, teclados, librerías, storages, servidores.
- **Software**: Sistemas Operativos, aplicaciones, etc.
- **Documentación**: Procedimientos, manuales, licencias, acuerdos de SLAs.

#### Beneficios de un CMDB

- Optimización de costos para: recambio tecnologico, incremento de capacidades, adquisicion de licencias, etc.
- Responder antes a un evento de troubleshooting
- Mejorar la calidad del servicio.
- Mejorar la experiencia y satisfacción del cliente.
- Administración eficaz de los activos y las configuraciones.
- Administración efectiva y eficiente de los cambios y las versiones.
- Mejora la planificación de tareas de mantenimiento.
- Identifica los responsables de cada activo.
- Disponibilidad de consulta sobre la infraestructura tecnológica de la organización.



![](https://i.imgur.com/dy7CI0e.png)

>Explicación: el servicio tiene 2 patas. Una de network y otra de Hosting. la de hosting esta administrado por john mark y tiene un servidor linux. Ese servidor linux corre un "Application1" que depende del servidor web, que es `Microsoft web IIS` y la parte de datos `Mycrosoft SQL`. Basicamente el CMDB muestra ramificaciones de este tipo de integraciones/arquitecturas.

> Los CMDB tienen "agentes" que van a estar monitoreando distintos dispositivos (ej: routers, switchs, librerias, storages, servers). Necesitan ciertas credenciales de acceso para correr comandos basicos (de solo lectura) para traer informacion de los equipos. nota personal @nia: suena parecido al `node-exporter` o a cualquier agente para capturar/monitorear y enviar metricas.  



---
# UNIDAD 2

## Agenda: Gobierno de IT (IT Governance)

```
- Definición
- Estadios de madurez.
- Competencias básicas del gobierno de IT.
- Areas de enfoque.
- Factores inductores y críticos.
- Organización del área de IT.
- Pasos para implementar el gobierno de IT.
- Matriz RACI
```


## Gobierno de IT

### Qué es Gobierno de IT?

Son las acciones que realiza el área de IT en coordinacion con la Organización para gestionar recursos fisicos y tecnologicos de la manera más eficiente en respuesta a requisitos regulatorios, operativos, estrategicos y del negocio.

El gobierno de IT busca que el área de IT contribuya al éxito de las empresas en las que se encuadran mediante una gestión eficiente de los recursos, minimizando los riesgos y alineando las decisiones con los objetivos del negocio.

Un buen gobierno de IT asegura que la inversión sea óptima, alineada con la estrategia del negocio y entrega valor bajo límites de riesgos aceptables teniendo en cuenta la cultura, estructura organizacional, madurez y estratégia.

#### Provee: 

- Un marco de estructuras y procesos mediante el cual las Organizaciones pueden alinear la estrategia del área de IT con la estratégia del negocio.

- Un conjunto de métodos y prácticas que permiten establecer:
	- Criterios de información requeridos por el negocio.
	- Procesos de negocio.
	- Recursos a utilizar.
- Procesos para conocer y gestionar todos los riesgos relacionados 

#### Por qué es importante?

- Cumple con las regulaciones vigentes
- Provee una ventaja competitiva.
- Soporta los objetivos de la Organización.
- Facilita el crecimiento y la innovación.
- Incrementa el valor intangible de la Organización.
- Reduce los riesgos.

## Madurez del Gobierno de IT

### Etapa 1: Ad Hoc

No hay procesos formales del Gobierno de IT y no es reconocido por el management como necesario. La inversión en IT es realizada completamente bajo la premisa "ad hoc".

### Etapa 2: Fragmentado

Hay un intento de formalizar los procesos del gobierno de IT pero se realiza de manera fragmentada, en una o varias unidades de negocio. Se optimizan las decisiones de IT dentro de cada unidad de negocio pero sin coordinación con el resto de la Organización.

> El profesor hace una mencion en clase de que el gobierno de IT utiliza el ciclo de demin para actualizar y perfeccionar los procesos

![](https://i.imgur.com/wSSURkS.png)

### Etapa 3: Consistencia

En esta etapa de madurez los procesos del Gobierno de IT han sido aplicados a traves de la Organizacin. Todas las unidades de negocio o entidades conforman las mismas politicas y procesos de IT. Las decisiones de inversión se basan en una visión general de la Organización.

### Etapa 4: Mejores Prácticas

Los procesos del Gobierno IT están totalmente optimizados a través de la Organización, un fuerte portfolio de procesos asegura que las decisiones de inversión de IT son tomadas de manera óptima. El CEO y el grupo ejecutivo son participantes activos en los procesos de gobernanza, la estrategia de IT es parte de la estrategia de la Organización.


## Competencias Básicas del Gobierno de IT

![](https://i.imgur.com/AFzjjFD.png)

# Areas de Enfoque

![](https://i.imgur.com/fnqRxES.png)

#### Alineacion Estrategica:

- Asegura que tanto los procesos de negocio como los de IT trabajen en conjunto.

#### Entrega de Valor:

- Asegura que el área de IT sea tan eficiente y eficaz como sea posible
- Generalmetne asociado a los costos.

#### Gestión de Recursos:

- Gestiona, controla y monitorea los recursos humanos y tecnológicos del área (propios y de terceros) para que sean lo más óptima posible.

#### Gestión de Riesgo:

- Permite que la empresa visualice los posibles riesgos para el negocio y suministra formas de minimizarlo. Determinar y mitigar los riesgos.

> Nota de @nia: relacionado con planes de disaster recovery.
#### Medición de desempeño:

- Usa indicadores que van mucho más allá de los criterios financieros, el Gobierno de IT asegura la medición y la evaluación precisa de los resultados del negocio.
- Visualiza el aporte del área de IT al negocio.

> **Nota: Sin una efectiva medición de desempeño, los otros cuatro aspectos del Gobierno de IT es muy probable que fallen.**

## Factores Inductores y Críticos:

### Factores Inductores

#### Regulaciones y Normativas:

- Legales (SOX, Ley de protección de datos personales)
- Estándares (ISO 27001, ISO 20000)

#### Optimización de Recursos:

- Reingeniería de procesos de IT
- Consolidación de recursos
- Estrategias de externalización (tercerización)

#### Peticiones del Negocio:

- Alineamiento de IT con la estrategia del negocio
- Ciclo de vida de productos
- Servicios
- Gestión de la demanda.

### Factores Críticos

- Conocer a donde se desea ir, evitando la improvisación.
- Dotar a la Organización de las herramientas adecuadas.
- Establecer mecanismos de medición y control claros.
- Cada situación requiere de soluciones a medida.
- Alinearse con iniciativas que estén en curso.
- No perderse en los modelos, no hay modelo ideal.
- El modelo a aplicar debe adecuarse al marco temporal.

