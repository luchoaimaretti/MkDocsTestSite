## Novedades

---

### Base de datos

| Nombre        | Tipo                 |
| ------------- | -------------------- |
| Servidor      | ITGTESTDCSRV1        |
| Base De Datos | GeneradorDeNovedades |
| Tabla         | Novedades            |
| Usuario       | andreani_test        |
| Contraseña    | cualquiercosa        |

---

### Filtros

| Nombre        | Tipo           | Obligacion |
| ------------- | -------------- | ---------- |
| NumeroDeEnvio | Texto          | OPCIONAL   |
| eventoEnvio   | Texto          |            |
| Cliente       | Desplegable    | MANDATORIO |
| CodigoCliente | Texto          | OPCIONAL   |
| fechaDesde    | DataTimePicker | OPCIONAL   |
| fechaHasta    | DataTimePicker | OPCIONAL   |

!!! abstract "Tanto fechaDesde como fechaHasta son fechas de incidencia."

---

### Generador De Novedades

Novedades = Grilla

| Nombre          | Tipo                                                           |
| --------------- | -------------------------------------------------------------- |
| id              |                                                                |
| numeroDeEnvio   | Numero Andreani                                                |
| eventoEnvio     | Evento de Integra que se generó para el envío                  |
| cliente         | Cliente dueño del envío                                        |
| codigoCliente   | Un codigo definido por el cliente para un evento en particular |
| traduccion      | Un codigo definido por el cliente para un evento en particular |
| fechaIncidencia | Fecha del movimiento                                           |
| mensajeEnviado  | Mensaje generado que se envió al cliente                       |

---

## Contrato

---

### Contratos

| Nombre             | Descripcion                                                |
| ------------------ | ---------------------------------------------------------- |
| Cliente            | Este dato sale de la tabla Contratos columna Cliente       |
| Numero De Contrato | Este dato sale de la tabla Contratos columna NumeroInterno |

---

### TMS

| Nombre    | Descripcion                                                                     |
| --------- | ------------------------------------------------------------------------------- |
| Evento    | Este dato sale de la tabla TrazasConfiguracionTMSs columna Evento               |
| Motivo    | Este dato sale de la tabla TrazasConfiguracionTMSs columna MotivoDescripcion    |
| Submotivo | Este dato sale de la tabla TrazasConfiguracionTMSs columna SubmotivoDescripcion |
| Ciclo     | Este dato sale de la tabla TrazasConfiguracionTMSs columna Ciclo                |
| TSM       | Este dato sale de la tabla TrazasConfiguracionTMSs columna TMS                  |

---

### TradXContratos

| Nombre         | Descripcion                                                               |
| -------------- | ------------------------------------------------------------------------- |
| CodigoCliente1 | Este dato sale de la tabla TraduccionesPorContrato columna CodigoCliente1 |
| CodigoCliente2 | Este dato sale de la tabla TraduccionesPorContrato columna CodigoCliente2 |

---

### Botones

| Nombre         | Descripcion                                                                  |
| -------------- | ---------------------------------------------------------------------------- |
| Acciones       | Boton Editar (Abre la misma ventana que Nueva Configuración)/ Boton Eliminar |
| CodigoCliente2 | Este dato sale de la tabla TraduccionesPorContrato columna CodigoCliente2    |

---

## Nueva Configuración

| Nombre                    | Descripcion                                                    |
| ------------------------- | -------------------------------------------------------------- |
| Botón Nueva Configuración | Abre una nueva “ventana” para agregar una nueva configuración. |
| CodigoCliente2            |                                                                |

---

### La ventana tendrá los siguientes campos:

| Nombre                        | Descripcion                                                                                                                        |
| ----------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| TMS (Lista Desplegable)       | Abre una nueva “ventana” para agregar una nueva configuración.                                                                     |
| Evento (Lista Desplegable)    | Este dato sale de la tabla TrazasConfiguracionTMSs columna Evento (Depende de la selección de los campos anteriores)               |
| Motivo (Lista Desplegable)    | Este dato sale de la tabla TrazasConfiguracionTMSs columna MotivoDescripcion (Depende de la selección de los campos anteriores)    |
| Submotivo (Lista Desplegable) | Este dato sale de la tabla TrazasConfiguracionTMSs columna SubmotivoDescripcion (Depende de la selección de los campos anteriores) |
| Ciclo (Lista Desplegable)     | Este dato sale de la tabla TrazasConfiguracionTMSs columna Ciclo (Depende de la selección de los campos anteriores)                |
| CodigoCliente1 (Text Box)     | Este dato sale de la tabla TraduccionesPorContrato columna CodigoCliente1                                                          |
| CodigoCliente2 (Text Box)     | Este dato sale de la tabla TraduccionesPorContrato columna CodigoCliente2                                                          |

---

### Botón Guardar/Actualizar

En el caso de llegar a esta ventana por el boton “Nueva Configuración”, todos los campos se pueden editar.

En el caso que se llegue a esta ventana por un botón Editar, los siguientes campos NO se pueden cambiar:

-   TMS
-   Evento
-   Motivo
-   Submotivo
-   Ciclo

Solo se puede cambiar el valor de los siguientes campos:

-   CodigoCliente1
-   CodigoClietne2
-   3 tablas contratos traducc tms, c/u de esas tablas se muestran juntas, solo tengo que actualizar solo.

---
