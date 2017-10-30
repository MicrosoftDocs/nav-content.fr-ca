---
title: "Définition et répartition des coûts"
description: "Les affectations de coûts déplacent les coûts et les revenus entre les types de coûts, les centres de coûts et les coûts associés. Vous pouvez définir autant d'affectations que nécessaire."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: f7c34e8f4c57e2effc03b8dcd2a722d7bdbb4692
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="defining-and-allocating-costs"></a><span data-ttu-id="13070-104">Définition et répartition des coûts</span><span class="sxs-lookup"><span data-stu-id="13070-104">Defining and Allocating Costs</span></span>
<span data-ttu-id="13070-105">Les affectations de coûts déplacent les coûts et les revenus entre les types de coûts, les centres de coûts et les coûts associés.</span><span class="sxs-lookup"><span data-stu-id="13070-105">Cost allocations move costs and revenues between cost types, cost centers, and cost objects.</span></span> <span data-ttu-id="13070-106">Vous pouvez définir autant d'affectations que nécessaire.</span><span class="sxs-lookup"><span data-stu-id="13070-106">You can define as many allocations as you need.</span></span> <span data-ttu-id="13070-107">Chaque affectation comporte les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="13070-107">Each allocation consists of:</span></span>  

-   <span data-ttu-id="13070-108">Une source affectation.</span><span class="sxs-lookup"><span data-stu-id="13070-108">An allocation source.</span></span>  
-   <span data-ttu-id="13070-109">Une ou plusieurs cibles d'affectation.</span><span class="sxs-lookup"><span data-stu-id="13070-109">One or more allocation targets.</span></span>  

<span data-ttu-id="13070-110">La source d'affectation détermine les coûts à affecter, tandis que les cibles d'affectation déterminent à quels emplacement affecter ces coûts.</span><span class="sxs-lookup"><span data-stu-id="13070-110">The allocation source establishes which costs must be allocated, and the allocation targets determine where the costs must be allocated.</span></span> <span data-ttu-id="13070-111">Par exemple, les coûts pour le type de coût Fournitures non stockables représentent une source d'affectation.</span><span class="sxs-lookup"><span data-stu-id="13070-111">For example, an allocation source can be the costs for the Electricity and Heating cost type.</span></span> <span data-ttu-id="13070-112">Vous affectez tous les coûts de fournitures non stockables à trois centres de coûts : Atelier, Production, et Vente.</span><span class="sxs-lookup"><span data-stu-id="13070-112">You allocate all electricity and heating costs to three cost centers: Workshop, Production, and Sales.</span></span> <span data-ttu-id="13070-113">Ces centres de coûts sont les cibles d'affectation.</span><span class="sxs-lookup"><span data-stu-id="13070-113">These cost centers are your allocation targets.</span></span>  

<span data-ttu-id="13070-114">Pour chaque source d'affectation, vous définissez un niveau d'affectation, une période de validité et une variante comme identificateur de regroupement.</span><span class="sxs-lookup"><span data-stu-id="13070-114">For each allocation source, you define an allocation level, a validity period, and a variant as grouping identifier.</span></span> <span data-ttu-id="13070-115">Vous pouvez utiliser un traitement en lot pour définir des filtres afin de sélectionner les définitions d'affectation, puis exécuter les affectations des coûts automatiquement.</span><span class="sxs-lookup"><span data-stu-id="13070-115">You can use a batch job to set filters to select allocation definitions and then run cost allocations automatically.</span></span>  

<span data-ttu-id="13070-116">Pour chaque cible d'affectation, vous définissez une base d'affectation.</span><span class="sxs-lookup"><span data-stu-id="13070-116">For each allocation target, you define an allocation base.</span></span> <span data-ttu-id="13070-117">La base d'affectation peut être statique ou dynamique.</span><span class="sxs-lookup"><span data-stu-id="13070-117">The allocation base can be either static or dynamic.</span></span>  

-   <span data-ttu-id="13070-118">Les bases d'affectation statique dépendent d'une valeur définie, par exemple, la superficie ou un ratio d'affectation prédéfini, comme 5:2:4.</span><span class="sxs-lookup"><span data-stu-id="13070-118">Static allocation bases are based on a definite value, such as square footage or an established allocation ratio, such as 5:2:4.</span></span>  
-   <span data-ttu-id="13070-119">Les bases d'affectation dynamique dépendent de valeurs variables, telles que le nombre d'employés dans un centre de coût ou les revenus de vente d'un objet de coûts associé pour une période donnée.</span><span class="sxs-lookup"><span data-stu-id="13070-119">Dynamic allocation bases depend on changeable values, such as the number of employees in a cost center or sales revenue of a cost object throughout a certain time period.</span></span>  

<span data-ttu-id="13070-120">Le tableau suivant décrit une série de tâches et inclut des liens vers les rubriques qui les décrivent.</span><span class="sxs-lookup"><span data-stu-id="13070-120">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

|<span data-ttu-id="13070-121">À</span><span class="sxs-lookup"><span data-stu-id="13070-121">To</span></span>|<span data-ttu-id="13070-122">Voir</span><span class="sxs-lookup"><span data-stu-id="13070-122">See</span></span>|  
|--------|---------|  
|<span data-ttu-id="13070-123">Configurez la source d'affectation et ses cibles.</span><span class="sxs-lookup"><span data-stu-id="13070-123">Set up allocation source and its targets.</span></span>|[<span data-ttu-id="13070-124">Comment configurer la source d'affectation et ses cibles</span><span class="sxs-lookup"><span data-stu-id="13070-124">How to: Set Up Allocation Source and Targets</span></span>](finance-how-to-set-up-allocation-source-and-targets.md)|  
|<span data-ttu-id="13070-125">Configurez plusieurs filtres pour les bases d'affectation dynamique.</span><span class="sxs-lookup"><span data-stu-id="13070-125">Set up various filters for dynamic allocation bases.</span></span>|[<span data-ttu-id="13070-126">Définition de filtres pour les bases de ventilation dynamique</span><span class="sxs-lookup"><span data-stu-id="13070-126">Setting Filters for Dynamic Allocation Bases</span></span>](finance-setting-filters-for-dynamic-allocation-bases.md)|  
|<span data-ttu-id="13070-127">Consultez un exemple sur le mode de définition d'une affectation statique.</span><span class="sxs-lookup"><span data-stu-id="13070-127">See an example of how to define a static allocation.</span></span>|[<span data-ttu-id="13070-128">Exemple de scénario : Définition des ventilations statiques en fonction du ratio d'affectation</span><span class="sxs-lookup"><span data-stu-id="13070-128">Scenario Example: Defining Static Allocations Based on Allocation Ratio</span></span>](finance-scenario-example-defining-static-allocations-based-on-allocation-ratio.md)|  
|<span data-ttu-id="13070-129">Consultez un exemple sur le mode de définition d'une affectation dynamique.</span><span class="sxs-lookup"><span data-stu-id="13070-129">See an example of how to define a dynamic allocation.</span></span>|[<span data-ttu-id="13070-130">Exemple de scénario : Définition des ventilations dynamique sur la base des articles vendus</span><span class="sxs-lookup"><span data-stu-id="13070-130">Scenario Example: Defining Dynamic Allocations Based on Items Sold</span></span>](finance-scenario-example-defining-dynamic-allocations-based-on-items-sold.md)|  

## <a name="see-also"></a><span data-ttu-id="13070-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="13070-131">See Also</span></span>  
 <span data-ttu-id="13070-132">[Paramétrage du contrôle de gestion](finance-set-up-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="13070-132">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span></span>  
 <span data-ttu-id="13070-133">[Transfert et report des écritures de coûts](finance-transfer-and-post-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="13070-133">[Transferring and Posting Cost Entries](finance-transfer-and-post-cost-entries.md) </span></span>  
 <span data-ttu-id="13070-134">[Comptabilité pour les coûts](finance-manage-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="13070-134">[Accounting for Costs](finance-manage-cost-accounting.md) </span></span>  
 <span data-ttu-id="13070-135">[Terminologie en comptabilité analytique](finance-terminology-in-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="13070-135">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span></span>  
 [<span data-ttu-id="13070-136">À propos de la comptabilité analytique</span><span class="sxs-lookup"><span data-stu-id="13070-136">About Cost Accounting</span></span>](finance-about-cost-accounting.md)

