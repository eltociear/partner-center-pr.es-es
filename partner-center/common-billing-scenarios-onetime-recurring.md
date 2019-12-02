---
title: Escenarios comunes de facturación para una sola vez y seleccione compras periódicas | Centro de Partners
ms.topic: article
ms.date: 11/21/2019
description: Escenarios de facturación comunes en el centro de partners para una sola vez y seleccione compras periódicas (por ejemplo, suscripciones de compra, agregando más suscripciones, agregando y quitando puestos).
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
Keywords: facturación, pagos, compra única, compra periódica, suscripciones, puestos
ms.localizationpriority: medium
ms.openlocfilehash: 69a7f1d4ded608942ea8b4bd7bec6054a44d52c7
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389643"
---
# <a name="one-time-and-select-recurring-purchase-billing-scenarios"></a><span data-ttu-id="d8b2d-104">Una vez y seleccione los escenarios de facturación de compra periódica</span><span class="sxs-lookup"><span data-stu-id="d8b2d-104">One-time and select recurring purchase billing scenarios</span></span>

<span data-ttu-id="d8b2d-105">Estos ejemplos de [escenarios de facturación comunes](common-billing-scenarios.md) se aplican a [una sola vez y seleccionan cargos periódicos](one-time-and-recurring-billing.md) en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-105">These example [common billing scenarios](common-billing-scenarios.md) are applicable to [one-time and select recurring charges](one-time-and-recurring-billing.md) in Partner Center.</span></span>

## <a name="purchase-a-subscription-and-add-a-seat-on-the-same-day"></a><span data-ttu-id="d8b2d-106">Comprar una suscripción y agregar un puesto en el mismo día</span><span class="sxs-lookup"><span data-stu-id="d8b2d-106">Purchase a subscription and add a seat on the same day</span></span>

<span data-ttu-id="d8b2d-107">En el escenario 1, compras una suscripción el 11 de junio a un precio unitario de 4 USD.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-107">In Scenario 1, you purchase a subscription on June 11 at a unit price of $4.</span></span> <span data-ttu-id="d8b2d-108">Más adelante el mismo día, compras otra unidad de la misma suscripción al mismo precio.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-108">Later that same day you purchase another of the same subscription at the same price.</span></span>

<span data-ttu-id="d8b2d-109">El archivo de conciliación incluirá lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="d8b2d-109">The recon file will include the following:</span></span>

- <span data-ttu-id="d8b2d-110">Factura de 4 USD para el período de servicio comprendido entre el 10 de junio y el 9 de julio.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-110">$4 bill for service period June 10 – July 9.</span></span>
- <span data-ttu-id="d8b2d-111">Renovación prorrateada de 4 USD para el período de servicio comprendido entre el 11 y el 11 de junio.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-111">$-4.00 prorated rebill for service period June 11 – June 11.</span></span> <span data-ttu-id="d8b2d-112">Este era el período cuando tenías una licencia.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-112">This is the period when you had 1 license.</span></span> <span data-ttu-id="d8b2d-113">Cálculo = (precio mensual/total de días en período de servicio total) x días del período de servicio prorrateado x número de licencias = (4/30) x 30 x 1 = 4,00.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-113">Calculation = (monthly price/total days in service period) x days in prorated service period x number of licenses = (4/30) x 30 x 1 = 4.00.</span></span>
- <span data-ttu-id="d8b2d-114">Renovación prorrateada de 8 USD para el período de servicio comprendido entre el 10 de junio y el 9 de julio.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-114">$8.00 prorated rebill for service period June 10 – July 9.</span></span> <span data-ttu-id="d8b2d-115">Este era el período cuando tenías 2 licencias.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-115">This is the period when you had 2 licenses.</span></span> <span data-ttu-id="d8b2d-116">Cálculo = (4/30) x 30 x 2 = 8,00.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-116">Calculation = (4/30) x 30 x 2 = 8.00.</span></span>

|<span data-ttu-id="d8b2d-117">**Fecha de compra**</span><span class="sxs-lookup"><span data-stu-id="d8b2d-117">**Purchase date**</span></span>   |<span data-ttu-id="d8b2d-118">**Inicio del cargo**</span><span class="sxs-lookup"><span data-stu-id="d8b2d-118">**Charge start**</span></span> |<span data-ttu-id="d8b2d-119">**Finalización del cargo**</span><span class="sxs-lookup"><span data-stu-id="d8b2d-119">**Charge end**</span></span>  |<span data-ttu-id="d8b2d-120">**Precio unitario**</span><span class="sxs-lookup"><span data-stu-id="d8b2d-120">**Unit price**</span></span>  |<span data-ttu-id="d8b2d-121">**Cantidad**</span><span class="sxs-lookup"><span data-stu-id="d8b2d-121">**Quantity**</span></span>  |<span data-ttu-id="d8b2d-122">**Volumen**</span><span class="sxs-lookup"><span data-stu-id="d8b2d-122">**Amount**</span></span> |<span data-ttu-id="d8b2d-123">**Tipo de cargo**</span><span class="sxs-lookup"><span data-stu-id="d8b2d-123">**Charge type**</span></span> |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|<span data-ttu-id="d8b2d-124">11/6/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-124">6/11/2019</span></span>      |<span data-ttu-id="d8b2d-125">10/6/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-125">6/10/2019</span></span>   |<span data-ttu-id="d8b2d-126">09/7/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-126">7/09/2019</span></span>         |<span data-ttu-id="d8b2d-127">4 USD</span><span class="sxs-lookup"><span data-stu-id="d8b2d-127">$4</span></span>                |<span data-ttu-id="d8b2d-128">1</span><span class="sxs-lookup"><span data-stu-id="d8b2d-128">1</span></span>                 |<span data-ttu-id="d8b2d-129">4 USD</span><span class="sxs-lookup"><span data-stu-id="d8b2d-129">$4</span></span>            |<span data-ttu-id="d8b2d-130">Nuevo</span><span class="sxs-lookup"><span data-stu-id="d8b2d-130">New</span></span>         |
|<span data-ttu-id="d8b2d-131">11/6/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-131">6/11/2019</span></span>     | <span data-ttu-id="d8b2d-132">10/6/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-132">6/10/2019</span></span>    |<span data-ttu-id="d8b2d-133">09/7/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-133">7/09/2019</span></span>        |<span data-ttu-id="d8b2d-134">4 USD</span><span class="sxs-lookup"><span data-stu-id="d8b2d-134">$4</span></span>        |<span data-ttu-id="d8b2d-135">1</span><span class="sxs-lookup"><span data-stu-id="d8b2d-135">1</span></span>        | <span data-ttu-id="d8b2d-136">-4 USD</span><span class="sxs-lookup"><span data-stu-id="d8b2d-136">-$4</span></span>       |<span data-ttu-id="d8b2d-137">addQuantity</span><span class="sxs-lookup"><span data-stu-id="d8b2d-137">addQuantity</span></span>           |
|<span data-ttu-id="d8b2d-138">11/6/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-138">6/11/2019</span></span>     | <span data-ttu-id="d8b2d-139">10/6/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-139">6/10/2019</span></span>    |<span data-ttu-id="d8b2d-140">09/7/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-140">7/09/2019</span></span>        |<span data-ttu-id="d8b2d-141">4 USD</span><span class="sxs-lookup"><span data-stu-id="d8b2d-141">$4</span></span>        | <span data-ttu-id="d8b2d-142">2</span><span class="sxs-lookup"><span data-stu-id="d8b2d-142">2</span></span>      |<span data-ttu-id="d8b2d-143">8 USD</span><span class="sxs-lookup"><span data-stu-id="d8b2d-143">$8</span></span>         |<span data-ttu-id="d8b2d-144">addQuantity</span><span class="sxs-lookup"><span data-stu-id="d8b2d-144">addQuantity</span></span>           |

## <a name="purchase-a-subscription-and-add-more-subscriptions-later"></a><span data-ttu-id="d8b2d-145">Comprar una suscripción y agregar más suscripciones más adelante</span><span class="sxs-lookup"><span data-stu-id="d8b2d-145">Purchase a subscription and add more subscriptions later</span></span>

<span data-ttu-id="d8b2d-146">En el escenario 2, compras una suscripción el 11 de junio a un precio unitario de 4 USD y el 12 de junio compras otra suscripción del mismo producto al mismo precio.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-146">In Scenario 2, you purchase a subscription on June 11 at a unit price of $4, and on June 12 you purchase another subscription for the same product at the same price.</span></span>

<span data-ttu-id="d8b2d-147">El archivo de conciliación incluirá lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="d8b2d-147">The recon file will include the following:</span></span>

- <span data-ttu-id="d8b2d-148">Factura de 4 USD para el período de servicio comprendido entre el 10 de junio y el 9 de julio.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-148">$4 bill for service period June 10 – July 9.</span></span>
- <span data-ttu-id="d8b2d-149">Renovación prorrateada de -3,87 USD para el período de servicio comprendido entre el 11 y el 12 de junio.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-149">$-3.87 prorated rebill for service period June 11 – June 12.</span></span> <span data-ttu-id="d8b2d-150">Este era el período cuando tenías una licencia.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-150">This is the period when you had 1 license.</span></span> <span data-ttu-id="d8b2d-151">Cálculo = (precio mensual/total de días en período de servicio total) x días del período de servicio prorrateado x número de licencias = (4/30) x 29 x 1 = 3,87.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-151">Calculation = (monthly price/total days in service period) x days in prorated service period x number of licenses = (4/30) x 29 x 1 = 3.87.</span></span>
- <span data-ttu-id="d8b2d-152">Renovación prorrateada de 7,74 USD para el período de servicio comprendido entre el 12 de junio y el 9 de julio.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-152">$7.74 prorated rebill for service period June 12 – July 9.</span></span> <span data-ttu-id="d8b2d-153">Este era el período cuando tenías 2 licencias.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-153">This is the period when you had 2 licenses.</span></span> <span data-ttu-id="d8b2d-154">Cálculo = (4/30) x 29 x 2 = 7,74.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-154">Calculation = (4/30) x 29 x 2 = 7.74.</span></span>

|<span data-ttu-id="d8b2d-155">**Fecha de compra**</span><span class="sxs-lookup"><span data-stu-id="d8b2d-155">**Purchase date**</span></span>   |<span data-ttu-id="d8b2d-156">**Inicio del cargo**</span><span class="sxs-lookup"><span data-stu-id="d8b2d-156">**Charge start**</span></span> |<span data-ttu-id="d8b2d-157">**Finalización del cargo**</span><span class="sxs-lookup"><span data-stu-id="d8b2d-157">**Charge end**</span></span>  |<span data-ttu-id="d8b2d-158">**Precio unitario**</span><span class="sxs-lookup"><span data-stu-id="d8b2d-158">**Unit price**</span></span>  |<span data-ttu-id="d8b2d-159">**Cantidad**</span><span class="sxs-lookup"><span data-stu-id="d8b2d-159">**Quantity**</span></span>  |<span data-ttu-id="d8b2d-160">**Volumen**</span><span class="sxs-lookup"><span data-stu-id="d8b2d-160">**Amount**</span></span> |<span data-ttu-id="d8b2d-161">**Tipo de cargo**</span><span class="sxs-lookup"><span data-stu-id="d8b2d-161">**Charge type**</span></span> |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|<span data-ttu-id="d8b2d-162">11/6/2019 (tienes 1 licencia)</span><span class="sxs-lookup"><span data-stu-id="d8b2d-162">6/11/2019 (you have one license)</span></span>     |<span data-ttu-id="d8b2d-163">10/6/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-163">6/10/2019</span></span>   |<span data-ttu-id="d8b2d-164">09/7/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-164">7/09/2019</span></span>         |<span data-ttu-id="d8b2d-165">4 USD</span><span class="sxs-lookup"><span data-stu-id="d8b2d-165">$4</span></span>         |<span data-ttu-id="d8b2d-166">1</span><span class="sxs-lookup"><span data-stu-id="d8b2d-166">1</span></span>        |<span data-ttu-id="d8b2d-167">4 USD</span><span class="sxs-lookup"><span data-stu-id="d8b2d-167">$4</span></span>            |<span data-ttu-id="d8b2d-168">Nuevo</span><span class="sxs-lookup"><span data-stu-id="d8b2d-168">New</span></span>         |
|<span data-ttu-id="d8b2d-169">12/6/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-169">6/12/2019</span></span>     | <span data-ttu-id="d8b2d-170">10/6/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-170">6/10/2019</span></span>    |<span data-ttu-id="d8b2d-171">09/7/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-171">7/09/2019</span></span>        |<span data-ttu-id="d8b2d-172">4 USD</span><span class="sxs-lookup"><span data-stu-id="d8b2d-172">$4</span></span>        |<span data-ttu-id="d8b2d-173">1</span><span class="sxs-lookup"><span data-stu-id="d8b2d-173">1</span></span>        | <span data-ttu-id="d8b2d-174">-3,87 USD</span><span class="sxs-lookup"><span data-stu-id="d8b2d-174">-$3.87</span></span>       |<span data-ttu-id="d8b2d-175">addQuantity</span><span class="sxs-lookup"><span data-stu-id="d8b2d-175">addQuantity</span></span>           |
|<span data-ttu-id="d8b2d-176">12/6/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-176">6/12/2019</span></span>     | <span data-ttu-id="d8b2d-177">10/6/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-177">6/10/2019</span></span>    |<span data-ttu-id="d8b2d-178">09/7/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-178">7/09/2019</span></span>        |<span data-ttu-id="d8b2d-179">4 USD</span><span class="sxs-lookup"><span data-stu-id="d8b2d-179">$4</span></span>        | <span data-ttu-id="d8b2d-180">2</span><span class="sxs-lookup"><span data-stu-id="d8b2d-180">2</span></span>      |<span data-ttu-id="d8b2d-181">7,74 USD</span><span class="sxs-lookup"><span data-stu-id="d8b2d-181">$7.74</span></span>       |<span data-ttu-id="d8b2d-182">addQuantity</span><span class="sxs-lookup"><span data-stu-id="d8b2d-182">addQuantity</span></span>           |

## <a name="purchase-a-subscription-and-remove-a-seat-on-the-same-day"></a><span data-ttu-id="d8b2d-183">Comprar una suscripción y quitar un puesto en el mismo día</span><span class="sxs-lookup"><span data-stu-id="d8b2d-183">Purchase a subscription and remove a seat on the same day</span></span>

<span data-ttu-id="d8b2d-184">En el escenario 3, compras dos suscripciones del mismo producto el 11 de junio a un precio unitario de 4 USD.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-184">In Scenario 3, you purchase two subscriptions for the same product on June 11 at a unit price of $4.</span></span> <span data-ttu-id="d8b2d-185">Más adelante el mismo día, quitas uno de los puestos.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-185">Later that same day you remove one of the seats.</span></span>  

<span data-ttu-id="d8b2d-186">El archivo de conciliación incluirá lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="d8b2d-186">The recon file will include the following:</span></span>

- <span data-ttu-id="d8b2d-187">Factura de 8 USD por dos licencias para el período de servicio comprendido entre el 10 de junio y el 9 de julio.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-187">$8 bill for two licenses for service period June 10 – July 9.</span></span>
- <span data-ttu-id="d8b2d-188">Renovación prorrateada de -8,00 USD para el período de servicio comprendido entre el 11 y el 11 de junio.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-188">$-8.00 prorated rebill for service period June 11 – June 11.</span></span> <span data-ttu-id="d8b2d-189">Este era el período cuando tenías 2 licencias.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-189">This is the period when you had 2 licenses.</span></span> <span data-ttu-id="d8b2d-190">Cálculo = (precio mensual/total de días en período de servicio total) x días del período de servicio prorrateado x número de licencias = (4/30) x 30 x 2 = 8,00.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-190">Calculation = (monthly price/total days in service period) x days in prorated service period x number of licenses = (4/30) x 30 x 2 = 8.00.</span></span>
- <span data-ttu-id="d8b2d-191">Renovación prorrateada de 4,00 USD para el período de servicio comprendido entre el 11 de junio y el 9 de julio.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-191">$4.00 prorated rebill for service period June 11 – July 9.</span></span> <span data-ttu-id="d8b2d-192">Este era el período cuando tenías una licencia.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-192">This is the period when you had 1 license.</span></span> <span data-ttu-id="d8b2d-193">Cálculo = (4/30) x 30 x 1 = 4,00.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-193">Calculation = (4/30) x 30 x 1 = 4.00.</span></span>

|<span data-ttu-id="d8b2d-194">**Fecha de compra**</span><span class="sxs-lookup"><span data-stu-id="d8b2d-194">**Purchase date**</span></span>   |<span data-ttu-id="d8b2d-195">**Inicio del cargo**</span><span class="sxs-lookup"><span data-stu-id="d8b2d-195">**Charge start**</span></span> |<span data-ttu-id="d8b2d-196">**Finalización del cargo**</span><span class="sxs-lookup"><span data-stu-id="d8b2d-196">**Charge end**</span></span>  |<span data-ttu-id="d8b2d-197">**Precio unitario**</span><span class="sxs-lookup"><span data-stu-id="d8b2d-197">**Unit price**</span></span>  |<span data-ttu-id="d8b2d-198">**Cantidad**</span><span class="sxs-lookup"><span data-stu-id="d8b2d-198">**Quantity**</span></span>  |<span data-ttu-id="d8b2d-199">**Volumen**</span><span class="sxs-lookup"><span data-stu-id="d8b2d-199">**Amount**</span></span> |<span data-ttu-id="d8b2d-200">**Tipo de cargo**</span><span class="sxs-lookup"><span data-stu-id="d8b2d-200">**Charge type**</span></span> |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|<span data-ttu-id="d8b2d-201">11/6/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-201">6/11/2019</span></span>      |<span data-ttu-id="d8b2d-202">10/6/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-202">6/10/2019</span></span>   |<span data-ttu-id="d8b2d-203">09/7/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-203">7/09/2019</span></span>         |<span data-ttu-id="d8b2d-204">4 USD</span><span class="sxs-lookup"><span data-stu-id="d8b2d-204">$4</span></span>                |<span data-ttu-id="d8b2d-205">2</span><span class="sxs-lookup"><span data-stu-id="d8b2d-205">2</span></span>                 |<span data-ttu-id="d8b2d-206">8 USD</span><span class="sxs-lookup"><span data-stu-id="d8b2d-206">$8</span></span>            |<span data-ttu-id="d8b2d-207">Nuevo</span><span class="sxs-lookup"><span data-stu-id="d8b2d-207">New</span></span>         |
|<span data-ttu-id="d8b2d-208">11/6/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-208">6/11/2019</span></span>     | <span data-ttu-id="d8b2d-209">10/6/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-209">6/10/2019</span></span>    |<span data-ttu-id="d8b2d-210">09/7/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-210">7/09/2019</span></span>        |<span data-ttu-id="d8b2d-211">4 USD</span><span class="sxs-lookup"><span data-stu-id="d8b2d-211">$4</span></span>        |<span data-ttu-id="d8b2d-212">2</span><span class="sxs-lookup"><span data-stu-id="d8b2d-212">2</span></span>        | <span data-ttu-id="d8b2d-213">-8 USD</span><span class="sxs-lookup"><span data-stu-id="d8b2d-213">-$8</span></span>       |<span data-ttu-id="d8b2d-214">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="d8b2d-214">removeQuantity</span></span>           |
|<span data-ttu-id="d8b2d-215">11/6/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-215">6/11/2019</span></span>     | <span data-ttu-id="d8b2d-216">10/6/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-216">6/10/2019</span></span>    |<span data-ttu-id="d8b2d-217">09/7/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-217">7/09/2019</span></span>        |<span data-ttu-id="d8b2d-218">4 USD</span><span class="sxs-lookup"><span data-stu-id="d8b2d-218">$4</span></span>        | <span data-ttu-id="d8b2d-219">1</span><span class="sxs-lookup"><span data-stu-id="d8b2d-219">1</span></span>      |<span data-ttu-id="d8b2d-220">4 USD</span><span class="sxs-lookup"><span data-stu-id="d8b2d-220">$4</span></span>         |<span data-ttu-id="d8b2d-221">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="d8b2d-221">removeQuantity</span></span>           |

## <a name="purchase-a-subscription-and-remove-seats-later"></a><span data-ttu-id="d8b2d-222">Compre una suscripción y quite puestos más adelante</span><span class="sxs-lookup"><span data-stu-id="d8b2d-222">Purchase a subscription and remove seats later</span></span>

<span data-ttu-id="d8b2d-223">En el escenario 4, compras 2 suscripciones el 11 de junio a un precio unitario de 4 USD y el 12 de junio quitas uno de los puestos.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-223">In Scenario 4, you purchase 2 subscriptions on June 11 at a unit price of $4, and on June 12 you remove one of the seats.</span></span>

<span data-ttu-id="d8b2d-224">El archivo de conciliación incluirá lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="d8b2d-224">The recon file will include the following:</span></span>

- <span data-ttu-id="d8b2d-225">Factura de 8 USD para el período de servicio comprendido entre el 10 de junio y el 9 de julio.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-225">$8 bill for service period June 10 – July 9.</span></span>
- <span data-ttu-id="d8b2d-226">Renovación prorrateada de -7,74 USD para el período de servicio comprendido entre el 11 y el 12 de junio.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-226">$-7.74 prorated rebill for service period June 11 – June 12.</span></span> <span data-ttu-id="d8b2d-227">Este era el período cuando tenías 2 licencias.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-227">This is the period when you had 2 licenses.</span></span> <span data-ttu-id="d8b2d-228">Cálculo = (precio mensual/total de días en período de servicio total) x días del período de servicio prorrateado x número de licencias = (4/30) x 29 x 2 = 7,74.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-228">Calculation = (monthly price/total days in service period) x days in prorated service period x number of licenses = (4/30) x 29 x 2 = 7.74.</span></span>
- <span data-ttu-id="d8b2d-229">Renovación prorrateada de 3,87 USD para el período de servicio comprendido entre el 12 de junio y el 9 de julio.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-229">$3.87 prorated rebill for service period June 12 – July 9.</span></span> <span data-ttu-id="d8b2d-230">Este era el período cuando tenías una licencia.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-230">This is the period when you had 1 license.</span></span> <span data-ttu-id="d8b2d-231">Cálculo = (4/30) x 29 x 1 = 3,87.</span><span class="sxs-lookup"><span data-stu-id="d8b2d-231">Calculation = (4/30) x 29 x 1 = 3.87.</span></span>

|<span data-ttu-id="d8b2d-232">**Fecha de compra**</span><span class="sxs-lookup"><span data-stu-id="d8b2d-232">**Purchase date**</span></span>   |<span data-ttu-id="d8b2d-233">**Inicio del cargo**</span><span class="sxs-lookup"><span data-stu-id="d8b2d-233">**Charge start**</span></span> |<span data-ttu-id="d8b2d-234">**Finalización del cargo**</span><span class="sxs-lookup"><span data-stu-id="d8b2d-234">**Charge end**</span></span>  |<span data-ttu-id="d8b2d-235">**Precio unitario**</span><span class="sxs-lookup"><span data-stu-id="d8b2d-235">**Unit price**</span></span>  |<span data-ttu-id="d8b2d-236">**Cantidad**</span><span class="sxs-lookup"><span data-stu-id="d8b2d-236">**Quantity**</span></span>  |<span data-ttu-id="d8b2d-237">**Volumen**</span><span class="sxs-lookup"><span data-stu-id="d8b2d-237">**Amount**</span></span> |<span data-ttu-id="d8b2d-238">**Tipo de cargo**</span><span class="sxs-lookup"><span data-stu-id="d8b2d-238">**Charge type**</span></span> |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|<span data-ttu-id="d8b2d-239">11/6/2019 (tienes 2 licencias)</span><span class="sxs-lookup"><span data-stu-id="d8b2d-239">6/11/2019 (you have 2 licenses)</span></span>     |<span data-ttu-id="d8b2d-240">10/6/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-240">6/10/2019</span></span>   |<span data-ttu-id="d8b2d-241">09/7/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-241">7/09/2019</span></span>         |<span data-ttu-id="d8b2d-242">4 USD</span><span class="sxs-lookup"><span data-stu-id="d8b2d-242">$4</span></span>         |<span data-ttu-id="d8b2d-243">2</span><span class="sxs-lookup"><span data-stu-id="d8b2d-243">2</span></span>        |<span data-ttu-id="d8b2d-244">8 USD</span><span class="sxs-lookup"><span data-stu-id="d8b2d-244">$8</span></span>       |<span data-ttu-id="d8b2d-245">Nuevo</span><span class="sxs-lookup"><span data-stu-id="d8b2d-245">New</span></span>       |
|<span data-ttu-id="d8b2d-246">12/6/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-246">6/12/2019</span></span>     | <span data-ttu-id="d8b2d-247">10/6/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-247">6/10/2019</span></span>    |<span data-ttu-id="d8b2d-248">09/7/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-248">7/09/2019</span></span>        |<span data-ttu-id="d8b2d-249">4 USD</span><span class="sxs-lookup"><span data-stu-id="d8b2d-249">$4</span></span>        |<span data-ttu-id="d8b2d-250">2</span><span class="sxs-lookup"><span data-stu-id="d8b2d-250">2</span></span>        | <span data-ttu-id="d8b2d-251">-7,74 USD</span><span class="sxs-lookup"><span data-stu-id="d8b2d-251">-$7.74</span></span>       |<span data-ttu-id="d8b2d-252">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="d8b2d-252">removeQuantity</span></span>           |
|<span data-ttu-id="d8b2d-253">12/6/2019 (tienes 1 licencia)</span><span class="sxs-lookup"><span data-stu-id="d8b2d-253">6/12/2019 (you have 1 license)</span></span>    | <span data-ttu-id="d8b2d-254">10/6/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-254">6/10/2019</span></span>    |<span data-ttu-id="d8b2d-255">09/7/2019</span><span class="sxs-lookup"><span data-stu-id="d8b2d-255">7/09/2019</span></span>   |<span data-ttu-id="d8b2d-256">4 USD</span><span class="sxs-lookup"><span data-stu-id="d8b2d-256">$4</span></span>    |<span data-ttu-id="d8b2d-257">1</span><span class="sxs-lookup"><span data-stu-id="d8b2d-257">1</span></span>      |<span data-ttu-id="d8b2d-258">3,87 USD</span><span class="sxs-lookup"><span data-stu-id="d8b2d-258">$3.87</span></span>    |<span data-ttu-id="d8b2d-259">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="d8b2d-259">removeQuantity</span></span> |