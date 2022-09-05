## Novedades

---

### GET (ByFilter) /api/novedades

```JSON title="REQ Filtro Novedades"
{
    "numeroEnvio": "string - OPCIONAL",
    "eventoEnvio": "string - OPCIONAL",
    "cliente": "string - OPCIONAL",
    "codigoCliente": "string - OPCIONAL",
    "traduccion": "string - OPCIONAL",
    "fechaDesde": "string - OPCIONAL",
    "fechaHasta": "string - OPCIONAL"
}
```

!!! warning "Del lado de la web se va a obligar a ingresar por lo menos 1 filtro"

    Esto es una prueba

---

## Clientes

---

### GET /api/clientes/nombres

```JSON title="RES"
{
    "nombreClientes": ["avon", "meli", "..."]
}
```

---

## Traducciones por contrato

---

GET /api/traduccionesPorContrato

=== "QUERY STRING"

    ```
    "/api/traduccionesPorContrato/numeroInterno={numeroInterno}"
    ```

=== "RES"

    ```JSON
    {
        "traduccionPorContrato": {
            "id": 7280,
            "evento": "Admision",
            "movimiento": 86,
            "descripcionMotivoTraza": "*",
            "motivo": 0 null,
            "descripcionSubMotivoTraza": "*",
            "subMotivo": 0 null,
            "ciclo": 1,
            "codigoCliente1": "test",
            "codigoCliente2": "test",
            "cliente": "Prueba",
            "idContrato": 4003,
            "idTrazasConfiguracionTMSs": 2
        },
        "numeroInterno": "123123",
        "tms": "INTEGRA"
    }
    ```

### GET de trazas

!!! warning "Primero lista desplegable de TMS"
