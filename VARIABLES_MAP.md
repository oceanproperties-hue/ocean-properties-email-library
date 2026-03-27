# OCEAN PROPERTIES — VARIABLES MAP
## ReservationKey ↔ Beds24 Template Variable Reference

Archivo de referencia para la migración y mantenimiento de templates de email.
Usar este mapa al crear o adaptar cualquier template entre sistemas.

---

## HUÉSPED

| Concepto | ReservationKey | Beds24 |
|----------|---------------|--------|
| Nombre | `{{guestfirstname}}` | `[GUESTFIRSTNAME]` |
| Apellido | `{{guestlastname}}` | `[GUESTNAME]` |
| Nombre completo | — | `[GUESTFULLNAME]` |
| Email | `{{guestemail}}` | `[GUESTEMAIL]` |
| Teléfono | `{{guestphone}}` | `[GUESTPHONE]` |
| Móvil | `{{guestmobilephone}}` | `[GUESTMOBILE]` |
| País | `{{guestcountry}}` | `[GUESTCOUNTRY]` |
| Ciudad | `{{guestcity}}` | `[GUESTCITY]` |
| Dirección | `{{guestaddress}}` | `[GUESTADDRESS]` |
| Empresa | `{{guestcompany}}` | `[GUESTCOMPANY]` |
| Notas del huésped | `{{guestnotes}}` | `[NOTES]` |
| Número de adultos | `{{numadults}}` | `[NUMADULT]` |
| Número de niños | `{{numchildren}}` | `[NUMCHILD]` |
| Total huéspedes | `{{numguests}}` | `[NUMPEOPLE]` |
| Comentarios | — | `[GUESTCOMMENTS]` |
| Idioma | — | `[GUESTLANGUAGE]` |

---

## RESERVA

| Concepto | ReservationKey | Beds24 |
|----------|---------------|--------|
| Número de reserva | `{{reservationnumber}}` | `[BOOKID]` |
| Número de reserva (últimos 4) | `{{reservationnumber_last4}}` | `[BOOKIDLAST4]` |
| Estado de reserva | `{{reservationstatus}}` | `[STATUS]` |
| Plan de tarifa | `{{rateplans}}` | `[OFFERNAME]` |
| Nombre de unidad | `{{roomname}}` | `[ROOMNAME]` |
| Descripción de unidad | `{{roomnameplusprimarydescription}}` | `[ROOMNAME]` |
| Número de unidad | `{{roomnumber}}` | `[ROOMID]` |
| Canal de origen | — | `[APISOURCETEXT]` |
| Fecha de reserva | `{{bookingdateshort}}` | `[BOOKINGDATE]` |
| Notas internas | — | `[INTERNALNOTES]` |

---

## FECHAS

| Concepto | ReservationKey | Beds24 |
|----------|---------------|--------|
| Fecha llegada (corta) | `{{arrivaldateshort}}` | `[FIRSTNIGHTSHORT]` |
| Fecha llegada (larga) | `{{arrivaldatelong}}` | `[FIRSTNIGHT:{%A, %e %B, %Y}]` |
| Día llegada (número) | `{{arrivalday2digit}}` | `[FIRSTNIGHT:{%d}]` |
| Mes llegada (nombre ES) | `{{arrivalmonthname_spanish}}` | `[FIRSTNIGHT:{%B}]` |
| Año llegada (4 dígitos) | `{{arrivalyear4digit}}` | `[FIRSTNIGHT:{%Y}]` |
| Día semana llegada (ES) | `{{arrivedayofweek_spanish}}` | `[FIRSTNIGHT:{%A}]` |
| Fecha salida (corta) | `{{departuredateshort}}` | `[LEAVINGDAYSHORT]` |
| Fecha salida (larga) | `{{departuredatelong}}` | `[LEAVINGDAY:{%A, %e %B, %Y}]` |
| Día salida (número) | `{{departureday2digit}}` | `[LEAVINGDAY:{%d}]` |
| Mes salida (nombre ES) | `{{departuremonthname_spanish}}` | `[LEAVINGDAY:{%B}]` |
| Año salida (4 dígitos) | `{{departureyear4digit}}` | `[LEAVINGDAY:{%Y}]` |
| Día semana salida (ES) | `{{departuredayofweek_spanish}}` | `[LEAVINGDAY:{%A}]` |
| Número de noches | `{{numnights}}` | `[NUMNIGHT]` |
| Fecha actual | — | `[CURRENTDATE]` |
| Días hasta check-in | — | `[DAYSTOCHECKIN]` |

---

## PAGOS Y MONTOS

| Concepto | ReservationKey | Beds24 |
|----------|---------------|--------|
| Total general | `{{grandtotal}}` | `[INVOICECHARGES]` |
| Total sin impuestos | `{{grandtotal_notax}}` | `[BASEPRICE]` |
| Monto pagado | `{{amountpaid}}` | `[INVOICEPAYMENTS]` |
| Balance pendiente | `{{balance}}` | `[INVOICEBALANCE]` |
| Depósito | `{{depositpaid}}` | `[DEPOSIT]` |
| Impuestos | `{{totaltaxes}}` | `[TAX]` |
| Descuentos | `{{totaldiscounts}}` | — |
| Último pago | `{{amountlastpayment}}` | — |
| Fecha último pago | `{{datelastpayment_short}}` | `[PAYMENTDATE]` |
| Fecha vencimiento depósito | `{{depositduedateshort}}` | — |
| Fecha vencimiento saldo | `{{balanceduedateshort}}` | — |
| Tarifa promedio por noche | `{{averageroomrate}}` | `[AVPRICE]` |

---

## LINKS Y ACCIONES

| Concepto | ReservationKey | Beds24 |
|----------|---------------|--------|
| Link de pago | `{{paymentlink}}` | `[PAYLINK]` |
| Link de pago (balance) | `{{paymentlink_balance}}` | `[PAYLINK:100%]` |
| Link de pago (monto libre) | `{{paymentlink_anyamount}}` | `[PAYLINK:200]` |
| Link de cancelación | — | `[CANCELURL]` |
| Link de reserva | `{{bookinglink}}` | — |
| Link de check-in online | `{{checkinlink}}` | `[CHECKINLINK]` |
| Link de reseña | `{{addcommentguestbooklink}}` | — |

---

## TABLA DE DETALLES DE RESERVA

| Concepto | ReservationKey | Beds24 |
|----------|---------------|--------|
| Detalles completos | `{{resdetails}}` | `[INVOICETABLE]` |
| Detalles con ledger | `{{resdetails_ledger}}` | `[INVOICETABLEVAT]` |
| Solo habitaciones | `{{resdetails_ledger_roomsonly}}` | `[INVOICETABLECHARGES]` |
| Items adicionales | `{{itemsforsale_all}}` | `[UPSELLTABLE]` |

---

## PROPIEDAD / SISTEMA

| Concepto | ReservationKey | Beds24 |
|----------|---------------|--------|
| Nombre de empresa | `{{companyname}}` | `[PROPERTYNAME]` |
| Email empresa | `{{companyemail}}` | `[PROPERTYEMAIL]` |
| Teléfono empresa | `{{companyphone}}` | `[PROPERTYPHONE]` |
| Web empresa | `{{companywebsite}}` | `[PROPERTYWEB]` |
| Política cancelación | — | `[PROPERTYCANCELPOLICY]` |
| Reglas de la casa | — | `[PROPERTYHOUSERULES]` |

---

## CAMPOS PERSONALIZADOS OCEAN PROPERTIES

| Concepto | ReservationKey | Beds24 |
|----------|---------------|--------|
| Responsable check-in | `{{RESPONSABLECHECKINCOMENTARIOS}}` | `[GUESTCUSTOMQ1]` |
| ID huésped | `{{ID}}` | `[GUESTCUSTOMQ2]` |
| Firma | `{{Signature}}` | — |
| Canal de origen | `{{ChannelName}}` | `[APISOURCETEXT]` |
| Cómo nos encontró | `{{comonosencontro}}` | `[GUESTCUSTOMQ3]` |
| Lista de huéspedes | `{{Listadodehuespedes}}` | `[GUESTCUSTOMQ4]` |
| Vehículo | `{{vehiculo}}` | `[GUESTCUSTOMQ5]` |

---

## NOTAS DE USO

- **ReservationKey:** variables con sintaxis `{{variable}}`
- **Beds24:** variables con sintaxis `[VARIABLE]`
- Las fechas en Beds24 permiten formato personalizado: `[FIRSTNIGHT:{%d de %B de %Y}]`
- Para lógica condicional en Beds24 usar: `[IF=:condición:verdadero|falso]`
- Siempre verificar en el sistema destino antes de activar un template en producción

---

*Última actualización: Marzo 2026*
*Mantenido por: Ocean Properties / 4rentpanama.com SA*
