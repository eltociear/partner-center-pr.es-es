---
title: Escenarios comunes de facturación para una sola vez y seleccione compras periódicas | Centro de Partners
ms.topic: article
ms.date: 11/25/2019
description: Consulte los ejemplos de facturación del centro de partners para una sola vez y seleccione compras periódicas; al adquirir suscripciones, agregar más suscripciones, agregar o quitar puestos.
ms.assetid: ''
author: jasonwhowell
ms.author: jasonh
Keywords: facturación, pagos, compra única, compra periódica, suscripciones, puestos
ms.localizationpriority: medium
ms.openlocfilehash: 9f1a96bfeee667f998d163416b96c281803f7107
ms.sourcegitcommit: 5dcf8cefd2c4731c6a80e57c65b43521d7c37b6d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/30/2020
ms.locfileid: "80390124"
---
# <a name="one-time-and-select-recurring-purchase-billing-scenarios"></a>Una vez y seleccione los escenarios de facturación de compra periódica

**Roles adecuados**

- Agente de administración
- Administrador de facturación
- Agente del departamento de soporte técnico
- Agente de ventas

Estos ejemplos de [escenarios de facturación comunes](common-billing-scenarios.md) se aplican a [una sola vez y seleccionan cargos periódicos](one-time-and-recurring-billing.md) en el centro de Partners.

## <a name="purchase-a-subscription-and-add-a-seat-on-the-same-day"></a>Comprar una suscripción y agregar un puesto en el mismo día

En el escenario 1, compras una suscripción el 11 de junio a un precio unitario de 4 USD. Más adelante el mismo día, compras otra unidad de la misma suscripción al mismo precio.

El archivo de conciliación incluirá lo siguiente:

- Factura de 4 USD para el período de servicio comprendido entre el 10 de junio y el 9 de julio.
- Renovación prorrateada de 4 USD para el período de servicio comprendido entre el 11 y el 11 de junio. Este era el período cuando tenías una licencia. Cálculo = (precio mensual/total de días en período de servicio total) x días del período de servicio prorrateado x número de licencias = (4/30) x 30 x 1 = 4,00.
- Renovación prorrateada de 8 USD para el período de servicio comprendido entre el 10 de junio y el 9 de julio. Este era el período cuando tenías 2 licencias. Cálculo = (4/30) x 30 x 2 = 8,00.

|**Fecha de compra**   |**Inicio del cargo** |**Finalización del cargo**  |**Precio unitario**  |**Cantidad**  |**Volumen** |**Tipo de cargo** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019      |10/6/2019   |09/7/2019         |4 USD                |1                 |4 USD            |Nuevo         |
|11/6/2019     | 10/6/2019    |09/7/2019        |4 USD        |1        | -4 USD       |addQuantity           |
|11/6/2019     | 10/6/2019    |09/7/2019        |4 USD        | 2      |8 USD         |addQuantity           |

## <a name="purchase-a-subscription-and-add-more-subscriptions-later"></a>Comprar una suscripción y agregar más suscripciones más adelante

En el escenario 2, compras una suscripción el 11 de junio a un precio unitario de 4 USD y el 12 de junio compras otra suscripción del mismo producto al mismo precio.

El archivo de conciliación incluirá lo siguiente:

- Factura de 4 USD para el período de servicio comprendido entre el 10 de junio y el 9 de julio.
- Renovación prorrateada de -3,87 USD para el período de servicio comprendido entre el 11 y el 12 de junio. Este era el período cuando tenías una licencia. Cálculo = (precio mensual/total de días en período de servicio total) x días del período de servicio prorrateado x número de licencias = (4/30) x 29 x 1 = 3,87.
- Renovación prorrateada de 7,74 USD para el período de servicio comprendido entre el 12 de junio y el 9 de julio. Este era el período cuando tenías 2 licencias. Cálculo = (4/30) x 29 x 2 = 7,74.

|**Fecha de compra**   |**Inicio del cargo** |**Finalización del cargo**  |**Precio unitario**  |**Cantidad**  |**Volumen** |**Tipo de cargo** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019 (tienes 1 licencia)     |10/6/2019   |09/7/2019         |4 USD         |1        |4 USD            |Nuevo         |
|12/6/2019     | 10/6/2019    |09/7/2019        |4 USD        |1        | -3,87 USD       |addQuantity           |
|12/6/2019     | 10/6/2019    |09/7/2019        |4 USD        | 2      |7,74 USD       |addQuantity           |

## <a name="purchase-a-subscription-and-remove-a-seat-on-the-same-day"></a>Comprar una suscripción y quitar un puesto en el mismo día

En el escenario 3, compras dos suscripciones del mismo producto el 11 de junio a un precio unitario de 4 USD. Más adelante el mismo día, quitas uno de los puestos.  

El archivo de conciliación incluirá lo siguiente:

- Factura de 8 USD por dos licencias para el período de servicio comprendido entre el 10 de junio y el 9 de julio.
- Renovación prorrateada de -8,00 USD para el período de servicio comprendido entre el 11 y el 11 de junio. Este era el período cuando tenías 2 licencias. Cálculo = (precio mensual/total de días en período de servicio total) x días del período de servicio prorrateado x número de licencias = (4/30) x 30 x 2 = 8,00.
- Renovación prorrateada de 4,00 USD para el período de servicio comprendido entre el 11 de junio y el 9 de julio. Este era el período cuando tenías una licencia. Cálculo = (4/30) x 30 x 1 = 4,00.

|**Fecha de compra**   |**Inicio del cargo** |**Finalización del cargo**  |**Precio unitario**  |**Cantidad**  |**Volumen** |**Tipo de cargo** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019      |10/6/2019   |09/7/2019         |4 USD                |2                 |8 USD            |Nuevo         |
|11/6/2019     | 10/6/2019    |09/7/2019        |4 USD        |2        | -8 USD       |removeQuantity           |
|11/6/2019     | 10/6/2019    |09/7/2019        |4 USD        | 1      |4 USD         |removeQuantity           |

## <a name="purchase-a-subscription-and-remove-seats-later"></a>Compre una suscripción y quite puestos más adelante

En el escenario 4, compras 2 suscripciones el 11 de junio a un precio unitario de 4 USD y el 12 de junio quitas uno de los puestos.

El archivo de conciliación incluirá lo siguiente:

- Factura de 8 USD para el período de servicio comprendido entre el 10 de junio y el 9 de julio.
- Renovación prorrateada de -7,74 USD para el período de servicio comprendido entre el 11 y el 12 de junio. Este era el período cuando tenías 2 licencias. Cálculo = (precio mensual/total de días en período de servicio total) x días del período de servicio prorrateado x número de licencias = (4/30) x 29 x 2 = 7,74.
- Renovación prorrateada de 3,87 USD para el período de servicio comprendido entre el 12 de junio y el 9 de julio. Este era el período cuando tenías una licencia. Cálculo = (4/30) x 29 x 1 = 3,87.

|**Fecha de compra**   |**Inicio del cargo** |**Finalización del cargo**  |**Precio unitario**  |**Cantidad**  |**Volumen** |**Tipo de cargo** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019 (tienes 2 licencias)     |10/6/2019   |09/7/2019         |4 USD         |2        |8 USD       |Nuevo       |
|12/6/2019     | 10/6/2019    |09/7/2019        |4 USD        |2        | -7,74 USD       |removeQuantity           |
|12/6/2019 (tienes 1 licencia)    | 10/6/2019    |09/7/2019   |4 USD    |1      |3,87 USD    |removeQuantity |
