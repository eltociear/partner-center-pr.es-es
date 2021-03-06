---
title: Confirmación de la aceptación por parte del cliente del Contrato de cliente de Microsoft | Centro de partners
ms.topic: article
ms.date: 04/07/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Obtén información sobre cómo confirmar la aceptación por parte del cliente del Contrato de cliente de Microsoft. Puede ser necesario para hacer pedidos de productos y servicios de Microsoft para los clientes.
author: LauraBrenner
ms.author: labrenne
keywords: cliente, clientes, consentimiento, MCA, Contrato de cliente de Microsoft, plantillas de contrato de cliente
ms.localizationpriority: high
ms.openlocfilehash: 2223a8e05a9df4c2d6ac377fc6f6b5a06944adc9
ms.sourcegitcommit: ee7f8600f566799838bda64e26c54799137f2cd5
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/11/2020
ms.locfileid: "81123327"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>Confirmación de la aceptación por parte del cliente del Contrato de cliente de Microsoft

**Se aplica a**
-  Centro de partners

**Roles adecuados**

- Agente de administrador
- Agente de ventas

> [!NOTE]
> Actualmente, el recurso de contrato solo es compatible con el Centro de partners en la nube pública de Microsoft. No es aplicable a:
> * Centro de partners operado por 21Vianet
> * Centro de partners para Microsoft Cloud Alemania
> * Centro de partners para Microsoft Cloud for US Government

>[!NOTE]
>A partir del 31 de enero de 2020, todos los clientes, existentes y nuevos, deben firmar el nuevo Contrato de cliente de Microsoft. Para obtener más detalles, consulta [Confirmación de la aceptación por parte del cliente del Contrato de cliente de Microsoft](confirm-customer-agreement.md).

Como partner, debes obtener la aceptación por parte de tu cliente del Contrato de cliente de Microsoft antes de pedir productos y servicios de Microsoft para dicho cliente. Para ayudar mejor a los partners a cumplir con los requisitos de cumplimiento, Microsoft les pide que confirmen la aceptación, proporcionando los siguientes detalles de la persona que aceptó el contrato:

- Nombre

- Apellido

- Dirección de correo electrónico

- Número de teléfono (opcional)

- Fecha de aceptación

Los partners de factura directa y los proveedores indirectos deben confirmar la aceptación por parte del cliente del Contrato de cliente de Microsoft cuando realicen transacciones a través del Centro de partners o la API del Centro de partners. La confirmación es *obligatoria*.

Si no se facilita la confirmación para un cliente determinado:

-    No podrás crear nuevos pedidos para este cliente.

-    No podrás cambiar el número de puestos de las suscripciones basadas en puestos existentes para este cliente.

La confirmación de la aceptación del cliente puede hacerse a través del panel del Centro de partners o la API del Centro de partners. Para hacerlo a través de la API del Centro de partners, consulta los temas siguientes: 

-   [Obtención de la confirmación del consentimiento del cliente](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-consent)

-   [Obtención de metadatos del contrato](https://docs.microsoft.com/partner-center/develop/get-agreement-metadata)

-   [Confirmación del consentimiento del cliente](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent)


Se aplica a los entornos de producción y de espacio aislado.

## <a name="confirming-customer-acceptance-in-partner-center"></a>Confirmación de la aceptación por parte del cliente en el Centro de partners

### <a name="confirm-customer-acceptance-for-a-new-customer"></a>Confirmación de la aceptación por parte del cliente para un nuevo cliente

Usa el siguiente procedimiento para confirmar la aceptación por parte del cliente mientras creas un nuevo inquilino en el panel del Centro de partners. Ten en cuenta que debes ser agente de administración o agente de ventas para poder hacer esto.

1. Selecciona **Clientes**, después **Nuevo cliente** y, a continuación, selecciona **Información de la cuenta**.
2. Escribe la información sobre la **Compañía** y el **Contacto principal**.

![Información sobre la compañía](images/mca/mca1.png)

3. En **Contrato de cliente de Microsoft**, selecciona **El cliente ha aceptado el Contrato de cliente de Microsoft más reciente**.
4. En **Fecha de aceptación del contrato**, introduce la fecha adecuada. No puedes elegir para esto una fecha futura.
5. Escribe los detalles del usuario que proporciona la aceptación.

![Adición de la fecha de aceptación](images/mca/MCA3.png)

De manera predeterminada, se muestra la información del usuario de contacto principal. Si esto no es correcto, selecciona **Actualizar** y, a continuación, introduce el **Nombre**, los **Apellidos**, la **Dirección de correo electrónico** y el **Número de teléfono* (opcional) de la persona que aceptó el contrato.

6. Selecciona **Siguiente** para continuar con los pasos restantes para crear el inquilino del cliente.

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Confirmación de la aceptación del cliente para un cliente existente

Debes ser agente de administración o agente de ventas para poder hacer esto.

1. Selecciona **Clientes** y, a continuación, busca y selecciona el cliente que quieras ver.
2. Selecciona **Información de cuenta**.
3. En **Contrato de cliente de Microsoft**, selecciona **Actualizar**.

![Actualizar](images/mca/mca4.png)

4. Escribe el **Nombre**, los **Apellidos**, la **Dirección de correo electrónico** y el **Número de teléfono** (opcional) del usuario que aceptó el contrato.
5. En **Fecha de aceptación del contrato**, introduce la fecha adecuada. No puedes elegir para esto una fecha futura.
6. Selecciona **Guardar y continuar**.

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Confirmación de la aceptación del cliente durante la creación de un nuevo pedido para un cliente existente

Si intentas crear un nuevo pedido para un cliente existente que no has confirmado con anterioridad, recibirás un aviso para completar la confirmación. Usa el siguiente procedimiento para hacerlo.

1. Escribe el **Nombre**, los **Apellidos**, la **Dirección de correo electrónico** y el **Número de teléfono** (opcional) del usuario que aceptó el contrato.
2. En **Fecha de aceptación del contrato**, introduce la fecha adecuada. No puedes elegir para esto una fecha futura.
3. Selecciona **Guardar y continuar**.

### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Recuperación de la confirmación de aceptación por parte del cliente para un cliente existente

Puedes recuperar la confirmación de la aceptación por parte del cliente para un cliente existente que hayas proporcionado anteriormente con el siguiente procedimiento. Debes ser agente de administración o agente de ventas para poder hacer esto.

1. Selecciona **Clientes** y, a continuación, busca y selecciona el cliente que quieras ver.
2. Selecciona **Información de cuenta**.
3. En **Contrato de cliente de Microsoft**, verás si se ha proporcionado o no la confirmación de este cliente.
