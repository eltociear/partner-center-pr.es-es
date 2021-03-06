---
title: Archivos de conciliación única y periódica | Centro de Partners
ms.topic: article
ms.date: 01/03/2020
description: Comprenda los archivos de conciliación única y periódica en el centro de Partners.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 6f381189fc1d8fad692ef248dcdcbf5ab8b0af43
ms.sourcegitcommit: fe1f2730a14ec394caccdbb59b00ef5908acaa29
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/09/2020
ms.locfileid: "75757238"
---
# <a name="one-time-and-recurring-reconciliation-files"></a>Archivos de conciliación única y periódica

**Se aplica a**

- Centro de partners
- Centro de partners para Microsoft Cloud for US Government

**Roles adecuados**
-   Administrador global
-   Administrador de usuarios
-   Administrador de facturación
-   Agente de administración
-   Agente de ventas

En este tema se explica cómo leer archivos de conciliación única y periódica en el centro de Partners.

## <a name="fields-in-one-time-and-recurring-reconciliation-files"></a>Campos de archivos de conciliación única y periódica

| Column | Descripción |
| ------ | ----------- |
| PartnerId | Identificador de inquilino de Azure Active Directory único (Azure AD) para una entidad de facturación específica, en formato GUID. No es necesario para la reconciliación. Igual en todas las filas. |
| CustomerId | Identificador único del inquilino de Azure AD, en formato GUID. Identifica al cliente. |
| CustomerName | Nombre de la organización del cliente, según figura en el Centro de partners. |
| CustomerDomainName | Nombre de dominio del cliente. Este campo puede aparecer en blanco hasta el segundo ciclo de facturación. *No utilice este campo como identificador único para el cliente. El cliente o asociado puede actualizar el personal o el dominio predeterminado a través del portal de Office 365.* |
| CustomerCountry | El país donde se encuentra el cliente. |
| InvoiceNumber | Número de factura donde aparece la transacción especificada. |
| MpnId | Identificador de MPN del asociado de CSP. |
| OrderId | Identificador único para un pedido en la plataforma de comercio de Microsoft. No se usa para la conciliación. |
| OrderDate | Fecha de realización del pedido. |
| ProductId | Identificador del producto. |
| SkuId | Identificador de una SKU determinada (unidad de mantenimiento de existencias). |
| AvailabilityId | Identificador de la disponibilidad de una SKU determinada. Esto muestra si la SKU está disponible para su compra en el país determinado, la moneda, el segmento del sector, etc. |
| SkuName | Título para un SKU concreto. |
| ProductName | Nombre del producto. |
| ChargeType | Tipo de cargo o ajuste. |
| UnitPrice | El precio unitario publicado en la lista de precios en el momento de la compra. *Asegúrese de que coincide con la información almacenada en el sistema de facturación durante la conciliación.* |
| Cantidad | Número de unidades. *Asegúrese de que coincide con la información almacenada en el sistema de facturación durante la conciliación.* |
| SubTotal | Total sin impuestos. Comprueba si el subtotal coincide con el total esperado, en caso de que se trate de un descuento. |
| TaxTotal | Cargo del importe de los impuestos. En función de las reglas de impuestos y las circunstancias específicas de su mercado. |
| Total | Total con impuestos. Comprueba si se cobran impuestos en la factura. |
| Moneda | Tipo de moneda. Cada entidad de facturación tiene una sola moneda. Asegúrese de que coincide con la primera factura y vuelva a comprobarlo después de cualquier actualización de la plataforma de facturación principal. |
| PriceAdjustmentDescription | Explicación de cualquier descuento aplicable. |
| PublisherName | Nombre del anunciante del producto.
| PublisherId | Identificador único para un publicador determinado. |
| SubscriptionDescription | Nombre descriptivo de una suscripción. |
| SubscriptionId | Identificador único de una suscripción en la plataforma de comercio de Microsoft. No se usa para la conciliación. *Este identificador no es el mismo que el **identificador de suscripción** en la consola de administración de socios comerciales.* |
| ChargeStartDate | Día de inicio de los cargos. La hora siempre corresponde al comienzo del día, 0:00. |
| ChargeEndDate | Día de finalización de los cargos. La hora siempre corresponde al fin del día, 23:59. |
| TermAndBillingcycle | La duración del período y el ciclo de facturación de la compra (por ejemplo, *1 año, mensualmente*). |
| EffectiveUnitPrice | Precio unitario tras realizar los ajustes. |
| UnitType | Tipo de unidad que se va a adquirir. |
| AlternateId | Un identificador alternativo a un **identificador de pedido**. |
| BillableQuantity | Representa el total de unidades adquiridas o consumidas. |
| BillingFrequency | Describe si el elemento de línea es una frecuencia de facturación mensual o única. *Actualmente solo se admite para Azure RI, con valores admitidos mensualmente. Si el RI se compra con una frecuencia de facturación única, este campo del archivo de conciliación aparecerá en blanco.* |
| PricingCurrency | Precio de venta del recurso u oferta. |
| PCToBCExchangeRate | Tasa de cambio que se aplica para la moneda de facturación. |
| PCToBCExchangeRateDate | Fecha en la que se determina la moneda de los precios de la moneda de facturación. |
| MeterDescription | La descripción del medidor para el elemento de línea de consumo. |


