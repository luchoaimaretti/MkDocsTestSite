## Crear una pagina nueva ABM de configuraciones por Contrato

| Nombre         | Descripcion                                         | Query                                                                               |
| -------------- | --------------------------------------------------- | ----------------------------------------------------------------------------------- |
| Contratos      | Tiene la info del numero de contrato y el cliente   | `SELECT * FROM GeneradorDeNovedades..Contrato`                                      |
| Datos Maestros | Tiene los “templates” de las configuraciones        | `SELECT * FROM GeneradorDeNovedades..TrazasConfiguracionTMS`                        |
| Configuracion  | Tiene las configuraciones por contratos de clientes | `SELECT * FROM GeneradorDeNovedades..TraduccionesPorContrato where idContrato = 59` |

---

## La nueva página llamada “Traducciones Por Contrato” tiene que tener:

---

### Filtros

-   Contrato: Sale de la tabla contrato: Mostrar Cliente-NumeroInterno ordenado por Cliente, NumeroInterno (Mostrar solo los que tienen Activo = 1)

-   Ejemplo de datos en la lista:

    Seleccionar

    -   Claro - 300005406
    -   Claro - 300006553
    -   DirecTv - 300007027
    -   DirecTv - 300007028
    -   DirecTv - 300007030
    -   Meli - 400010302
    -   Meli - 400010303
