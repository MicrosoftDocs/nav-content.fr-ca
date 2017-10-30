---
title: "Détails de conception - Planification de l'approvisionnement"
description: "Cette rubrique donne un aperçu des concepts et principes qui sont utilisés avec les fonctionnalités de planification de l'approvisionnement dans [!INCLUDE[d365fin](includes/d365fin_md.md)]."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, supply, planning, reordering, replenishment
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: a3a5197ba727404ce7e6dea5ee529ced6dcfa68e
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-supply-planning"></a><span data-ttu-id="3bb5c-103">Détails de conception : planification de l'approvisionnement</span><span class="sxs-lookup"><span data-stu-id="3bb5c-103">Design Details: Supply Planning</span></span>
<span data-ttu-id="3bb5c-104">Cette documentation fournit une analyse technique détaillée des concepts et principes qui sont utilisés dans les fonctions Supply Planning dans [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="3bb5c-104">This documentation provides detailed technical insight to the concepts and principles that are used within the Supply Planning features in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

<span data-ttu-id="3bb5c-105">Elle explique comment le système de planification fonctionne et comment modifier les algorithmes pour répondre aux exigences de planification dans différents environnements.</span><span class="sxs-lookup"><span data-stu-id="3bb5c-105">It explains how the planning system works and how to adjust the algorithms to meet planning requirements in different environments.</span></span> <span data-ttu-id="3bb5c-106">Il présente d'abord les concepts centraux de la solution, puis décrit la logique du mécanisme central, l'équilibrage d'approvisionnement, avant d'indiquer la manière dont la planification de l'inventaire est exécutée à l'aide de méthodes de réapprovisionnement.</span><span class="sxs-lookup"><span data-stu-id="3bb5c-106">It first introduces central solution concepts and then describes the logic of the central mechanism, supply balancing, before proceeding to explain how inventory planning is performed with the use of reordering policies.</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="3bb5c-107">Dans cette section</span><span class="sxs-lookup"><span data-stu-id="3bb5c-107">In This Section</span></span>  
[<span data-ttu-id="3bb5c-108">Détails de conception : concepts centraux du système de planification</span><span class="sxs-lookup"><span data-stu-id="3bb5c-108">Design Details: Central Concepts of the Planning System</span></span>](design-details-central-concepts-of-the-planning-system.md)  
[<span data-ttu-id="3bb5c-109">Détails de conception : réservation, chaînage et message d'action</span><span class="sxs-lookup"><span data-stu-id="3bb5c-109">Design Details: Reservation, Order Tracking, and Action Messaging</span></span>](design-details-reservation-order-tracking-and-action-messaging.md)  
[<span data-ttu-id="3bb5c-110">Détails de conception : équilibrage de la demande et de l'approvisionnement</span><span class="sxs-lookup"><span data-stu-id="3bb5c-110">Design Details: Balancing Demand and Supply</span></span>](design-details-balancing-demand-and-supply.md)  
[<span data-ttu-id="3bb5c-111">Détails de conception : gestion des méthodes de réapprovisionnement</span><span class="sxs-lookup"><span data-stu-id="3bb5c-111">Design Details: Handling Reordering Policies</span></span>](design-details-handling-reordering-policies.md)  
[<span data-ttu-id="3bb5c-112">Détails de conception : paramètres de planification</span><span class="sxs-lookup"><span data-stu-id="3bb5c-112">Design Details: Planning Parameters</span></span>](design-details-planning-parameters.md)  
[<span data-ttu-id="3bb5c-113">Détails de conception : tableau d'affectation de planification</span><span class="sxs-lookup"><span data-stu-id="3bb5c-113">Design Details: Planning Assignment Table</span></span>](design-details-planning-assignment-table.md)  
[<span data-ttu-id="3bb5c-114">Détails de conception : demande à un magasin vide.</span><span class="sxs-lookup"><span data-stu-id="3bb5c-114">Design Details: Demand at Blank Location</span></span>](design-details-demand-at-blank-location.md)  
[<span data-ttu-id="3bb5c-115">Détails de conception : transferts de planification</span><span class="sxs-lookup"><span data-stu-id="3bb5c-115">Design Details: Transfers in Planning</span></span>](design-details-transfers-in-planning.md)

