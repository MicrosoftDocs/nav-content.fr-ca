---
title: "Détails de conception - Gestion des méthodes de réapprovisionnement"
description: "Aperçu des tâches pour définir une méthode de réapprovisionnement dans la planification des approvisionnements."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 281f87c446ef95cf3e8bbe119184d2202699f4df
ms.contentlocale: fr-ca
ms.lasthandoff: 12/01/2017

---
# <a name="design-details-handling-reordering-policies"></a><span data-ttu-id="61e97-103">Détails de conception : gestion des méthodes de réapprovisionnement</span><span class="sxs-lookup"><span data-stu-id="61e97-103">Design Details: Handling Reordering Policies</span></span>
<span data-ttu-id="61e97-104">Pour qu'un article participe à la planification des approvisionnements, une méthode de regroupement doit être définie.</span><span class="sxs-lookup"><span data-stu-id="61e97-104">For an item to participate in supply planning, a reorder policy must be defined.</span></span> <span data-ttu-id="61e97-105">Les quatre méthodes de réapprovisionnement disponibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="61e97-105">The following four reordering policies exist:</span></span>  
  
* <span data-ttu-id="61e97-106">Qté fixe de commande.</span><span class="sxs-lookup"><span data-stu-id="61e97-106">Fixed Reorder Qty.</span></span>  
* <span data-ttu-id="61e97-107">Qté maximum</span><span class="sxs-lookup"><span data-stu-id="61e97-107">Maximum Qty.</span></span>  
* <span data-ttu-id="61e97-108">Ordre</span><span class="sxs-lookup"><span data-stu-id="61e97-108">Order</span></span>  
* <span data-ttu-id="61e97-109">Lot pour lot</span><span class="sxs-lookup"><span data-stu-id="61e97-109">Lot-for-Lot</span></span>  
  
<span data-ttu-id="61e97-110">Les méthodes Qté fixe de commande et Qté maximum sont liées à la planification de l'inventaire.</span><span class="sxs-lookup"><span data-stu-id="61e97-110">Fixed Reorder Qty. and Maximum Qty. policies relate to inventory planning.</span></span> <span data-ttu-id="61e97-111">Bien que la planification de l'inventaire soit techniquement plus simple que la procédure de contrepartie, ces stratégies doivent coexister avec la contrepartie pas à pas de l'approvisionnement et du suivi de commande.</span><span class="sxs-lookup"><span data-stu-id="61e97-111">Although inventory planning is technically simpler than the balancing procedure, these policies must coexist with the step-by-step balancing of supply and order tracking.</span></span> <span data-ttu-id="61e97-112">Pour contrôler l'intégration entre les deux, et livrer la visibilité dans la logique de planification utilisée, des principes stricts régissent la façon dont les méthodes de réapprovisionnement sont traitées.</span><span class="sxs-lookup"><span data-stu-id="61e97-112">To control the integration between the two, and to provide visibility into the involved planning logic, strict principles govern how reordering policies are handled.</span></span>  
  
## <a name="in-this-section"></a><span data-ttu-id="61e97-113">Dans cette section</span><span class="sxs-lookup"><span data-stu-id="61e97-113">In This Section</span></span>  
[<span data-ttu-id="61e97-114">Détails de conception : Le rôle du point de commande</span><span class="sxs-lookup"><span data-stu-id="61e97-114">Design Details: The Role of the Reorder Point</span></span>](design-details-the-role-of-the-reorder-point.md)  
[<span data-ttu-id="61e97-115">Détails de conception : surveillance du niveau de stock prévisionnel et du point de commande</span><span class="sxs-lookup"><span data-stu-id="61e97-115">Design Details: Monitoring the Projected Inventory Level and the Reorder Point</span></span>](design-details-monitoring-the-projected-inventory-level-and-the-reorder-point.md)  
[<span data-ttu-id="61e97-116">Détails de conception : Le rôle de l'intervalle de planification</span><span class="sxs-lookup"><span data-stu-id="61e97-116">Design Details: The Role of the Time Bucket</span></span>](design-details-the-role-of-the-time-bucket.md)  
[<span data-ttu-id="61e97-117">Détails de conception : rester sous le niveau de dépassement de capacité</span><span class="sxs-lookup"><span data-stu-id="61e97-117">Design Details: Staying under the Overflow Level</span></span>](design-details-staying-under-the-overflow-level.md)  
[<span data-ttu-id="61e97-118">Détails de conception : traitement du stock prévisionnel négatif</span><span class="sxs-lookup"><span data-stu-id="61e97-118">Design Details: Handling Projected Negative Inventory</span></span>](design-details-handling-projected-negative-inventory.md)  
[<span data-ttu-id="61e97-119">Détails de conception : méthodes de réapprovisionnement</span><span class="sxs-lookup"><span data-stu-id="61e97-119">Design Details: Reordering Policies</span></span>](design-details-reordering-policies.md)  
  
## <a name="see-also"></a><span data-ttu-id="61e97-120">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="61e97-120">See Also</span></span>  
<span data-ttu-id="61e97-121">[Détails de conception : paramètres de planification](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="61e97-121">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
<span data-ttu-id="61e97-122">[Détails de conception : tableau d'affectation de planification](design-details-planning-assignment-table.md) </span><span class="sxs-lookup"><span data-stu-id="61e97-122">[Design Details: Planning Assignment Table](design-details-planning-assignment-table.md) </span></span>  
<span data-ttu-id="61e97-123">[Détails de conception : concepts centraux du système de planification](design-details-central-concepts-of-the-planning-system.md) </span><span class="sxs-lookup"><span data-stu-id="61e97-123">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span></span>  
<span data-ttu-id="61e97-124">[Détails de conception : équilibrage de la demande et de l'approvisionnement](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="61e97-124">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
[<span data-ttu-id="61e97-125">Détails de conception : planification de l'approvisionnement</span><span class="sxs-lookup"><span data-stu-id="61e97-125">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
