---
title: "Exemple de scénario - Définition des affectations dynamiques sur la base des articles vendus"
description: "Cette rubrique explique comment définir les affectations à l'aide du mode d'affectation dynamique. Dans l'exemple, vous modifiez l'affectation dynamique des coûts pour que le centre de coûts VENTES prenne en charge le nouveau ÉQUIPEMENT IT de l'objet de coûts. Les packages ÉQUIPEMENT IT ont des numéros d'articles dont la plage s'échelonne entre 8904-W et 8924-W. Vous pouvez utiliser les chiffres de ventes de l'exercice précédent pour en calculer le partage. L'affectation est reportée en fonction du type de coût d'aide 9903."
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
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: 0d892099be95d52546d98bf17705df2b19f764c7
ms.contentlocale: fr-ca
ms.lasthandoff: 10/26/2017

---
# <a name="scenario-example-defining-dynamic-allocations-based-on-items-sold"></a><span data-ttu-id="d289b-107">Exemple de scénario : Définition des ventilations dynamique sur la base des articles vendus</span><span class="sxs-lookup"><span data-stu-id="d289b-107">Scenario Example: Defining Dynamic Allocations Based on Items Sold</span></span>
<span data-ttu-id="d289b-108">Cette rubrique explique comment définir les affectations à l'aide du mode d'affectation dynamique.</span><span class="sxs-lookup"><span data-stu-id="d289b-108">This topic shows an example of how to define allocations by using the dynamic allocation method.</span></span> <span data-ttu-id="d289b-109">Dans l'exemple, vous modifiez l'affectation dynamique des coûts pour que le centre de coûts VENTES prenne en charge le nouveau ÉQUIPEMENT IT de l'objet de coûts.</span><span class="sxs-lookup"><span data-stu-id="d289b-109">In the example, you change the dynamic allocation of the costs for the SALES cost center to support the new cost object IT EQUIPMENT.</span></span> <span data-ttu-id="d289b-110">Les packages ÉQUIPEMENT IT ont des numéros d'articles dont la plage s'échelonne entre 8904-W et 8924-W.</span><span class="sxs-lookup"><span data-stu-id="d289b-110">IT EQUIPMENT packages have item numbers in the range from 8904-W to 8924-W.</span></span> <span data-ttu-id="d289b-111">Vous pouvez utiliser les chiffres de ventes de l'exercice précédent pour en calculer le partage.</span><span class="sxs-lookup"><span data-stu-id="d289b-111">You use the previous year’s sales figures to calculate the share.</span></span> <span data-ttu-id="d289b-112">L'affectation est reportée en fonction du type de coût d'aide 9903.</span><span class="sxs-lookup"><span data-stu-id="d289b-112">The allocation is posted to the helping cost type 9903.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="d289b-113">L'exemple utilise les données de démonstration dans [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="d289b-113">The example uses the demo data in the [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

## <a name="to-define-dynamic-allocations-based-on-items-sold-in-the-previous-year"></a><span data-ttu-id="d289b-114">Pour définir les ventilations dynamique en fonction des articles vendus de l'exercice précédent</span><span class="sxs-lookup"><span data-stu-id="d289b-114">To define dynamic allocations based on items sold in the previous year</span></span>  

1.  <span data-ttu-id="d289b-115">Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Affectations des coûts**, puis sélectionnez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="d289b-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Cost Allocations**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="d289b-116">Dans la fenêtre **Affectation des coûts**, sélectionnez l'action **Nouveau**.</span><span class="sxs-lookup"><span data-stu-id="d289b-116">In the **Cost Allocation** window, choose the **New** action.</span></span>  
3.  <span data-ttu-id="d289b-117">Dans le champ **ID**, appuyez sur Entrée ou saisissez un ID.</span><span class="sxs-lookup"><span data-stu-id="d289b-117">In the **ID** field, press Enter or enter an ID.</span></span>  
4.  <span data-ttu-id="d289b-118">Dans le champ **Niveau**, saisissez **1**.</span><span class="sxs-lookup"><span data-stu-id="d289b-118">In the **Level** field, enter **1**.</span></span>  
5.  <span data-ttu-id="d289b-119">Dans les champs **Valide à partir de** et **Valide jusque**, entrez les dates appropriées.</span><span class="sxs-lookup"><span data-stu-id="d289b-119">In the **Valid From** and **Valid To** fields, enter appropriate dates.</span></span>  
6.  <span data-ttu-id="d289b-120">Dans le champ **Code centre de coûts**, entrez **VENTES**.</span><span class="sxs-lookup"><span data-stu-id="d289b-120">In the **Cost Center Code** field, enter **SALES**.</span></span>  
7.  <span data-ttu-id="d289b-121">Dans le champ **Type de crédit\\\/coût**, entrez le type de coût **9903**.</span><span class="sxs-lookup"><span data-stu-id="d289b-121">In the **Credit to Cost Type** field, enter the cost type **9903**.</span></span>  
8.  <span data-ttu-id="d289b-122">Dans le champ **Type coût cible**, entrez le type de coût **9903**.</span><span class="sxs-lookup"><span data-stu-id="d289b-122">In the **Target Cost Type** field, enter the cost type **9903**.</span></span>  
9. <span data-ttu-id="d289b-123">Dans le champ **Objet de coûts cible**, sélectionnez **Nouveau** pour créer un nouvel objet de coût ÉQUIPEMENT IT et renseigner les champs, le cas échéant.</span><span class="sxs-lookup"><span data-stu-id="d289b-123">In the **Target Cost Object** field, choose **New** to create a new cost object IT EQUIPMENT and fill in fields as necessary.</span></span> <span data-ttu-id="d289b-124">Sélectionnez **ÉQUIPEMENT IT**.</span><span class="sxs-lookup"><span data-stu-id="d289b-124">Select **IT EQUIPMENT**.</span></span> <span data-ttu-id="d289b-125">Laissez le champ **Centre de coûts cible** vide.</span><span class="sxs-lookup"><span data-stu-id="d289b-125">Leave the **Target Cost Center** field blank.</span></span>  
10. <span data-ttu-id="d289b-126">Dans le champ **Type cible affectation**, sélectionnez **Tous les coûts** pour définir le mode d'affectation de tous les coûts cumulés.</span><span class="sxs-lookup"><span data-stu-id="d289b-126">In the **Allocation Target Type** field, select **All Costs** to define how all accumulated costs are allocated.</span></span>  
11. <span data-ttu-id="d289b-127">Dans le champ **Base**, sélectionnez la base d'affectation **Articles vendus (Montant)**.</span><span class="sxs-lookup"><span data-stu-id="d289b-127">In the **Base** field, select the allocation base **Items Sold (Amount)**.</span></span>  
12. <span data-ttu-id="d289b-128">Dans le champ **Filtre n°**, entrez **8904-W..8924-W**.</span><span class="sxs-lookup"><span data-stu-id="d289b-128">In the **No. Filter** field, enter **8904-W..8924-W**.</span></span>  
13. <span data-ttu-id="d289b-129">Dans le champ **Code filtre date**, entrez **Année précédente**.</span><span class="sxs-lookup"><span data-stu-id="d289b-129">In the **Date Filter Code** field, enter **Last Year**.</span></span>  
14. <span data-ttu-id="d289b-130">Choisissez l'action **Calculer la clé d'affectation** pour calculer l'action.</span><span class="sxs-lookup"><span data-stu-id="d289b-130">Choose the **Calculate Allocation Key** action to calculate the share.</span></span>  

    > [!IMPORTANT]  
    >  [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="d289b-131"> utilise les chiffres de ventes des exercices précédents pour calculer une part de 1596,50 DS avec 100 % alloués pour les packages ÉQUIPEMENT IT.</span><span class="sxs-lookup"><span data-stu-id="d289b-131"> uses the previous years’ sales figures to calculate a share of 1596.50 LCY with 100 percent for the IT EQUIPMENT packages.</span></span> <span data-ttu-id="d289b-132">Cela signifie que tous les articles vendus au cours de l'exercice précédent seront affectés à l'ÉQUIPEMENT IT des objets de coûts.</span><span class="sxs-lookup"><span data-stu-id="d289b-132">This means that all of the items sold last year will be allocated to the cost object IT EQUIPMENT.</span></span>  

## <a name="see-also"></a><span data-ttu-id="d289b-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d289b-133">See Also</span></span>  
 <span data-ttu-id="d289b-134">[Définition de filtres pour les bases d'affectation dynamique](finance-setting-filters-for-dynamic-allocation-bases.md) </span><span class="sxs-lookup"><span data-stu-id="d289b-134">[Setting Filters for Dynamic Allocation Bases](finance-setting-filters-for-dynamic-allocation-bases.md) </span></span>  
 <span data-ttu-id="d289b-135">[Comment configurer la source d'affectation et ses cibles](finance-how-to-set-up-allocation-source-and-targets.md) </span><span class="sxs-lookup"><span data-stu-id="d289b-135">[How to: Set Up Allocation Source and Targets](finance-how-to-set-up-allocation-source-and-targets.md) </span></span>  
 <span data-ttu-id="d289b-136">[Définition et répartition des coûts](finance-define-and-allocate-costs.md) </span><span class="sxs-lookup"><span data-stu-id="d289b-136">[Defining and Allocating Costs](finance-define-and-allocate-costs.md) </span></span>  
 <span data-ttu-id="d289b-137">[Terminologie en comptabilité analytique](finance-terminology-in-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="d289b-137">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span></span>  
 [<span data-ttu-id="d289b-138">À propos de la comptabilité analytique</span><span class="sxs-lookup"><span data-stu-id="d289b-138">About Cost Accounting</span></span>](finance-about-cost-accounting.md)

