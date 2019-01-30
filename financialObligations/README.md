## Transaction Additional Fields
 
In Honduras, a payment process is compose by 2 different stages, 
- financialObligation (F01-Devengado): when the suppliers make the invoice to receive the payment.
- transaction (Orden de Transferencia Pago): when the payment is done by Secretaria de Finanzas and the money is deposit to the supplier.
The current transaction object only covers the last part of the process, and the other stage is relevant for the process, too.

## Example
```json
{
"implementation": {
            "transactions": [
              {
                "id": "T2018-449-1-TRB-93064",
                "date": "2018-04-12T14:04:47Z",
                "value": {
                  "amount": 583845.44,
                  "currency": "HNL"
                },
                "payer": {
                  "id": "HN-ENG-449",
                  "name": "Servicios Financieros de la Administración Central"
                },
                "payee": {
                  "id": "HN-RTN-05069999182490",
                  "name": "AGUAS DE PUERTO CORTES S.A. DE C.V."
                },
                "uri": "http://localhost:4511/transacciones/T2018-449-1-TRB-93064",
                "budgetSources": [
                  "2018-50-1-5-1-0-0-12-11-1-21200-0"
                ],
                "financialObligationIds": [
                  "D2018-50-1-563-1-1"
                ]
              }
            ],
            "financialObligations": [
              {
                "id": "D2018-50-1-563-1-1",
                "description": "CANCELACION DE SERVICIO DE AGUA POTABLE DE LOS DIFERENTES CENTROS EDUCATIVOS DE PUERTO CORTES CORRESPONDIENTE A LOS MESES DE SEPTIEMBRE,OCTUBRE,Y NOVIEMBRE DEL\nAÑO 2,017 (QUEDO PENDIENTE POR FALTA DE PRESUPUESTO)",
                "bill": {
                  "id": "2199,2620,2621-DGA-",
                  "type": "OFI",
                  "description": "CANCELACION DE SERVICIO DE AGUA POTABLE DE LOS DIFERENTES CENTROS EDUCATIVOS DE PUERTO CORTES CORRESPONDIENTE A LOS MESES DE SEPTIEMBRE,OCTUBRE,Y NOVIEMBRE DEL\nAÑO 2,017 (QUEDO PENDIENTE POR FALTA DE PRESUPUESTO)",
                  "date": "2018-03-08T00:03:00Z",
                  "amount": {
                    "amount": 583845.44,
                    "currency": "HNL"
                  }
                },
                "retentions": [],
                "approvalDate": "2018-03-12T11:03:46Z"
              }
            ]
        }
 }
```
