# Historias de usuario de búsqueda

| Campo | Valor |
| --- | --- |
| Proyecto | Proyecto Simbiosis |
| Fecha | 28/10/2026 |
| Versión | 1 |
| Estado | Borrador |

## Fuentes comunes

- [Acta de UC-21 Buscar recetas](../captura/acta-acuerdos-uc-21-buscar-recetas.md), v1.1, Vigente.
- [Catálogo de requisitos](catalogo-requisitos.md), UR-08 y FR pertinentes.
- [Modelo de casos de uso](../modelos/modelo-casos-de-uso.md), UC-21.

## Épica de búsqueda

Como usuario registrado, quiero realizar una búsqueda de recetas con la posibilidad de añadir filtros, para encontrar recetas compatibles con mis criterios de búsqueda.

**Estado:** descompuesta en US-01, US-02 y US-03. Conserva la necesidad conjunta.

## Justificación de la división

[Justificación de los resultados útiles que separa la división.]

## US-01

**Título:** Realizar una búsqueda de recetas mediante palabras clave.

Como usuario registrado, quiero realizar una búsqueda en el catálogo de recetas que coincidan con un texto, para localizar recetas que coincidan con esas palabras clave.

**Fuentes:** UR-08; UC-21; FR-085; acta, criterios de búsqueda.

### Criterios de aceptación

- **CA-01.** Dada una búsqueda por palabra clave con resultados coincidentes, cuando se realiza la búsqueda, entonces se mostrarán los resultados.
- **CA-02.** Dada una búsqueda por palabra clave sin resultados coincidentes, cuando se realiza la búsqueda, entonces no se mostrarán resultados.

## US-02

**Título:** Añadir filtros en la búsqueda de recetas

Como usuario registrado, quiero realizar una búsqueda en base a ingredientes, para localizar las recetas que contengan o excluyan los ingredientes deseados.

**Fuentes:** UR-08; UC-21; FR-086 y FR-087; acta, criterios de búsqueda.

### Criterios de aceptación

- **CA-01.** Dada una lista de ingredientes incluidos, cuando se solicita la búsqueda, entonces se mostrarán las recetas que contengan todos los ingredientes de la lista.
- **CA-02.** Dada una lista de ingredientes excluidos, cuando se solicita la búsqueda, entonces se mostrarán las recetas que no contengan ninguno de los ingredientes de la lista.
- **CA-03.** Dado un ingrediente en la lista de incluidos y de excluidos, cuando se solicita la búsqueda, entonces se señala el conflicto y no se ejecuta la búsqueda.

## US-03

**Título:** Acceder a una receta

Como usuario registrado, quiero acceder a una receta seleccionada, para obtener más detalle sobre la receta.

**Fuentes:** UR-08; UC-21; FR-089; acta, Resultados y detalle.

### Criterios de aceptación

- **CA-01.** Dada una búsqueda con resultados coincidentes ordenados por fecha de publicación, cuando se visualizan los resultados, entonces se muestra una vista previa por cada resultado.
- **CA-02.** Dada una búsqueda con resultados coincidentes ordenados por fecha de publicación, cuando se selecciona el resultado, entonces se muestra el detalle de esa receta.
- **CA-03.** Dada una búsqueda con resultados coincidentes ordenados por fecha de publicación, cuando se solicita volver a la búsqueda, entonces se conservan los filtros de la anterior búsqueda.

## Revisión INVEST

La revisión abarca US-01, US-02 y US-03. «Aplicado» indica si se ha realizado la comprobación. «Cumple» indica si todas las historias cumplen el criterio. Si alguna no lo cumple, indicar «No» e identificar la historia y el motivo en la justificación. Si no se ha realizado la comprobación o faltan datos, indicar «Pendiente» en «Cumple».

| Criterio | Pregunta de revisión | Aplicado | Cumple | Justificación |
| --- | --- | --- | --- | --- |
| Independiente | ¿Puede implementarse cada historia y ofrecer un resultado útil sin implementar antes las otras historias del conjunto? Puede compartir infraestructura con ellas. | Sí     | Sí | [Historias y motivo] |
| Negociable | ¿Cada historia explica qué necesita la persona y deja margen para discutir los detalles de la solución, respetando los acuerdos confirmados? | Sí | Sí | [Historias y motivo] |
| Valiosa | ¿La parte «para…» de cada historia explica el beneficio que obtiene la persona al usar esa capacidad? | Sí | Sí | [Historias y motivo] |
| Estimable | ¿Están claros el alcance y los datos necesarios para estimar el trabajo de cada historia? | Sí | Sí | [Historias y motivo] |
| Pequeña | ¿Se centra cada historia en una única capacidad de alcance manejable? | Sí | Sí | [Historias y motivo] |
| Comprobable | ¿Los criterios de aceptación de cada historia describen acciones y resultados observables que permiten distinguir un comportamiento correcto de uno incorrecto? | Sí | Sí | [Historias y motivo] |

## Dudas pendientes

[Cuestiones pendientes de aclaración. Si no quedan cuestiones, indicar «Ninguna».]
