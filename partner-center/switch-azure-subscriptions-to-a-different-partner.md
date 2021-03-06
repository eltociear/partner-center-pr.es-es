---
title: Transferir suscripciones de Azure | Centro de partners
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo trabajar con un cliente para cambiar qué asociado del programa proveedor de soluciones en la nube usará el cliente para los servicios de Azure.
ms.assetid: 42D1D9AB-613D-4FC1-A846-EE769923E699
author: jasonwhowell
ms.author: jasonh
keywords: suscripción de azure, alternar partner, cambiar partner, obtener nuevo partner, otro partner
ms.localizationpriority: medium
ms.openlocfilehash: 3a709ad7eac9b2a4db7063a47713c27dc41d7833
ms.sourcegitcommit: 5dcf8cefd2c4731c6a80e57c65b43521d7c37b6d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/30/2020
ms.locfileid: "80390624"
---
# <a name="transfer-azure-subscriptions"></a>Transferir suscripciones de Azure 

**Se aplica a**

- Centro de partners para Microsoft Cloud for US Government
- Centro de partners para Microsoft global Cloud

Un cliente puede decidir cambiarse a un partner del Proveedor de soluciones en la nube u otro partner para los servicios de Microsoft Azure. Sin embargo, este es un proceso manual que requiere acciones del partner y del cliente.

>[!Note]  
>En este momento, solo los proveedores directos o indirectos pueden transferir suscripciones.
>Por el momento, no es posible cambiar los partners de las suscripciones de Proveedor de soluciones en la nube para las suscripciones de Office 365, Enterprise Mobility Suite o Microsoft Dynamics CRM.



**Cambiar asociados para suscripciones de Azure**

1. Para transferir una suscripción de Azure a un socio nuevo, el cliente debe iniciar el proceso y ponerse en contacto con su partner de registro actual por escrito. 
>[!Note]
>Es responsabilidad del partner actual crear el vale de servicio que inicia el proceso de transferencia. Microsoft no puede intervenir en nombre del cliente o del nuevo partner. El cliente debe tener previsto trabajar estrechamente con el partner actual para que la transición se realice sin problemas.

2. El partner de la suscripción debe realizar las siguientes tareas:

Crear un vale de servicio de Azure desde el Centro de partners para solicitar una transferencia de suscripción:
-   En el menú del centro de Partners, seleccione **clientes**, seleccione el cliente en la lista y, a continuación, seleccione **Administración de servicios**. En la sección **Vales de soporte**, selecciona la lista desplegable **Nuevo vale** y elige **Microsoft Azure**.

-   Desde el portal de Azure, selecciona **Nueva solicitud de soporte técnico**.

En el paso 1, elige **Administración de suscripciones** como tipo de problema, especifica el Id. de suscripción que quieres transferir y selecciona **Proveedor de soluciones en la nube** como el plan de soporte técnico.

En el paso 2, seleccione **C-impacto mínimo** y elija **otras preguntas generales** como tipo de problema.

Descarga el [formulario de transferencia de suscripción de CSP](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip).

3. Para el partner de la suscripción: rellena el [formulario de transferencia de suscripción de CSP](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip), fírmalo y luego envíalo al cliente. Para rellenar el formulario, necesitarás la siguiente información:

- Información de contacto del partner actual e Id. de Microsoft. En el menú del centro de Partners, seleccione Configuración de la **cuenta** &gt; Perfil de la **organización**y use el **identificador de Microsoft**, el nombre de la **organización**y la **Dirección** que aparecen en ella.

- Id. Microsoft del cliente En el menú del Centro de partners, selecciona **Clientes** y, después, expande la lista del cliente para ver su **Id. Microsoft**.

- Id. de suscripción que se va a transferir. En el listado de clientes expandido, selecciona **Ver suscripciones** y, a continuación, expande la suscripción seleccionada para ver el **Id. de suscripción**.

>[!Note]
>Transferir una suscripción genera dos identificadores de suscripción que verás en la página **Editar suscripción** de la suscripción transferida: **1**- El identificador de suscripción del Centro de partners se usa para fines de facturación. 
**2**- El identificador de suscripción original de Azure se conserva y aparecerá en el Centro de partners, así como en el portal de administración de Azure. Este identificador aparecerán en el archivo de conciliación.  **Al registrar vales de soporte técnico, debe usar ambos identificadores.**

4. Para el cliente y el nuevo partner para la suscripción:

Revisa el formulario, rellena la información sobre el nuevo partner y fírmalo. Comprueba que el nuevo cliente tiene un acuerdo contractual en vigor. Vuelve a enviar el formulario al partner de registro actual.

*Importante*: si el nuevo partner de CSP no tiene una relación de revendedor con el cliente, debe establecer una antes de que se transfiera la suscripción. [Puedes encontrar información sobre cómo hacer esto aquí](request-a-relationship-with-a-customer.md).

>[!Note]
>El nuevo asociado de CSP y el inquilino del cliente deben estar en el mismo país. 

5. Partner actual:

Asegúrate de que el formulario incluye información de contacto para ambos administradores de partners. Soporte técnico de Microsoft se pondrá en contacto con ambos para comprobar la transferencia. Asegúrate de que las tres firmas estén en su lugar y, a continuación, adjunta el formulario rellenado a la solicitud de servicio existente mediante la opción **Carga de archivos**. Un ingeniero de soporte técnico de Microsoft se pondrá en contacto contigo en un plazo de 8 horas laborales para validar la recepción y la finalización.

6. Nuevo partner:

Actualiza la configuración de suscripción de Azure para quitar el partner antiguo de la cuenta. Para ver qué asignaciones de roles están aprovisionadas, ejecuta dos commandlets de Powershell.

-   Agrega el nuevo asociado como el revendedor de la cuenta:

**PS C:\\&gt; Add-AzureRMAccount-tenant "CustomerDomainName"**

Para encontrar el valor de customerDomainName: en el menú del Centro de partners, selecciona **Clientes**. En la lista de clientes, selecciona el cliente. En el menú del cliente, selecciona **Cuenta** y usa el valor de **Nombre de dominio**.

-   Observa los roles de la cuenta, incluidos los asociados de CSP anteriores:

**PS C:\\&gt; Get-AzureRMRoleAssignment**

7. Quitar permisos de acceso obsoletos

-  En el menú del Centro de partners, selecciona **Clientes**. 
-  Expande la lista del cliente y selecciona **Ver suscripciones**. 
-  En el menú del cliente, selecciona **Administración de servicios**. 
-  En **Microsoft Azure**, haz clic en el vínculo para ir al **Portal de administración de Microsoft Azure**.

 

 



