---
title: "Procédure : Utiliser des ressources pour des projets"
author: SorenGP
ms.custom: na
ms.date: 12/14/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: cced4bca42b74c2664fd18770f1616c57286e1c3
ms.contentlocale: fr-ca
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-use-resources-for-jobs"></a><span data-ttu-id="97588-102">Procédure : Utiliser des ressources pour des projets</span><span class="sxs-lookup"><span data-stu-id="97588-102">How to: Use Resources for Jobs</span></span>
<span data-ttu-id="97588-103">Vous devez enregistrer l'utilisation des ressources dans le journal projet pour suivre les coûts et les prix, ainsi que les types de travaux associés aux projets.</span><span class="sxs-lookup"><span data-stu-id="97588-103">You record the usage of resources in the job journal to keep track of costs, prices, and the work types that are linked to jobs.</span></span> <span data-ttu-id="97588-104">Pour plus d'informations, reportez-vous à [Procédure : Enregistrer l'utilisation pour les projets](projects-how-record-job-usage.md).</span><span class="sxs-lookup"><span data-stu-id="97588-104">For more information, see [How to: Record Usage for Jobs](projects-how-record-job-usage.md).</span></span>

<span data-ttu-id="97588-105">Vous pouvez aussi reporter l'utilisation d'une ressource dans un journal ressource.</span><span class="sxs-lookup"><span data-stu-id="97588-105">You can also post the usage of a resource in a resource journal.</span></span> <span data-ttu-id="97588-106">Les écritures reportées dans un journal ressource n'ont aucune incidence sur le grand livre.</span><span class="sxs-lookup"><span data-stu-id="97588-106">Entries posted in a resource journal have no effect on the general ledger.</span></span>

## <a name="to-assign-resources-to-jobs"></a><span data-ttu-id="97588-107">Pour affecter des ressources aux projets</span><span class="sxs-lookup"><span data-stu-id="97588-107">To assign resources to jobs</span></span>
<span data-ttu-id="97588-108">Vous pouvez affecter des ressources aux projets en créant des lignes planification projet pour le projet.</span><span class="sxs-lookup"><span data-stu-id="97588-108">You assign resources to jobs by creating job planning lines for the job.</span></span> <span data-ttu-id="97588-109">Pour plus d'informations, reportez-vous à [Procédure : Créer des projets](projects-how-create-jobs.md).</span><span class="sxs-lookup"><span data-stu-id="97588-109">For more information, see [How to: Create Jobs](projects-how-create-jobs.md).</span></span>

## <a name="to-record-resource-usage-for-a-job"></a><span data-ttu-id="97588-110">Pour enregistrer l'utilisation des ressources pour un projet</span><span class="sxs-lookup"><span data-stu-id="97588-110">To record resource usage for a job</span></span>

1. <span data-ttu-id="97588-111">Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Feuilles activité projet**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="97588-111">In the top right corner, choose the **Search for Page or Report** icon, enter **Job Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="97588-112">Ouvrez le lot journal projet approprié, puis complétez les champs selon vos besoins.</span><span class="sxs-lookup"><span data-stu-id="97588-112">Open a relevant job journal batch, and then fill in the fields as necessary.</span></span> <span data-ttu-id="97588-113">Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.</span><span class="sxs-lookup"><span data-stu-id="97588-113">Choose a field to read a short description of the field or link to more information.</span></span>
3. <span data-ttu-id="97588-114">Lorsque la feuille est renseignée, cliquez sur **Valider**.</span><span class="sxs-lookup"><span data-stu-id="97588-114">When the journal is complete, choose the **Post** action.</span></span>

## <a name="to-adjust-resource-prices"></a><span data-ttu-id="97588-115">Pour ajuster le prix des ressources</span><span class="sxs-lookup"><span data-stu-id="97588-115">To adjust resource prices</span></span>  
<span data-ttu-id="97588-116">Si vous souhaitez modifier le coût ou le prix d'un grand nombre de ressources, vous pouvez utiliser un traitement en lot.</span><span class="sxs-lookup"><span data-stu-id="97588-116">If you want to change costs or prices for a large number of resources, you can use a batch job.</span></span>  

1. <span data-ttu-id="97588-117">Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Ajuster coûts/prix ressource**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="97588-117">In the top right corner, choose the **Search for Page or Report** icon, enter **Adjust Resource Costs/Prices**, and then choose the related link.</span></span>
2. <span data-ttu-id="97588-118">Renseignez les autres champs selon vos besoins, puis cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="97588-118">Fill in the fields on a line as necessary, and then choose the **OK** button.</span></span>

<span data-ttu-id="97588-119">**Remarque** : Ce traitement par lots ne crée pas et n'ajuste pas les nouveaux coûts ou prix des ressources.</span><span class="sxs-lookup"><span data-stu-id="97588-119">**Note**: This batch job does not create or adjust alternate costs or prices for resources.</span></span> <span data-ttu-id="97588-120">Il modifie uniquement le contenu du champ de la fiche ressource correspondant au champ **Champ à modifier** que vous avez sélectionné dans le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="97588-120">It only changes the contents of the field on the resource card for the **Adjust Field** field that you selected in the batch job.</span></span> <span data-ttu-id="97588-121">L'ajustement s'appliquant immédiatement aux ressources, vérifiez les facteurs d'ajustement avant de lancer le traitement en lot.</span><span class="sxs-lookup"><span data-stu-id="97588-121">The adjustment will take effect immediately for resources, so check your adjustment factors before you run the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-existing-alternate-prices"></a><span data-ttu-id="97588-122">Pour obtenir des propositions de modification des prix ressource basées sur les prix secondaires existants</span><span class="sxs-lookup"><span data-stu-id="97588-122">To get resource price change suggestions based on existing alternate prices</span></span>  
<span data-ttu-id="97588-123">Si vous avez déjà configuré d'autres prix pour un certain nombre de ressources, vous pouvez utiliser un traitement en lot pour configurer d'autres prix ressource.</span><span class="sxs-lookup"><span data-stu-id="97588-123">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span></span>

1. <span data-ttu-id="97588-124">Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Nouv. prix ressource proposés**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="97588-124">In the top right corner, choose the **Search for Page or Report** icon, enter **Resource Price Changes**, and then choose the related link.</span></span>
2. <span data-ttu-id="97588-125">Sélectionnez l'action **Prop. modif. prix ress. (prix)**, puis renseignez les champs selon vos besoins.</span><span class="sxs-lookup"><span data-stu-id="97588-125">Choose the **Suggest Res. Price Chg. (Price)** action, and then fill in the fields as necessary.</span></span>
3. <span data-ttu-id="97588-126">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="97588-126">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="97588-127">Lorsque le traitement par lots est terminé, la fenêtre **Nouv. prix ressource proposés** affiche les résultats du traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="97588-127">When the batch job is finished, the **Resource Price Changes** window shows the results of the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-standard-prices"></a><span data-ttu-id="97588-128">Pour obtenir des propositions de modification des prix ressource basées sur les prix standard :</span><span class="sxs-lookup"><span data-stu-id="97588-128">To get resource price change suggestions based on standard prices</span></span>  
<span data-ttu-id="97588-129">Si vous souhaitez configurer plusieurs autres prix ressource sur la base des prix standard des fiches ressource, vous pouvez utiliser un traitement en lot.</span><span class="sxs-lookup"><span data-stu-id="97588-129">If you want to set up multiple alternate resource prices based on the standard prices on the resource cards, you can use a batch job.</span></span>  

1. <span data-ttu-id="97588-130">Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Nouv. prix ressource proposés**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="97588-130">In the top right corner, choose the **Search for Page or Report** icon, enter **Resource Price Changes**, and then choose the related link.</span></span>
2. <span data-ttu-id="97588-131">Sélectionnez l'action **Prop. modif. prix ress. (ress)**, puis renseignez les champs selon vos besoins.</span><span class="sxs-lookup"><span data-stu-id="97588-131">Choose the **Suggest Res. Price Chg. (Res.)** action, and then fill in the fields as necessary.</span></span>  
3. <span data-ttu-id="97588-132">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="97588-132">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="97588-133">Lorsque le traitement par lots est terminé, ouvrez la fenêtre **Nouv. prix ressource proposés** pour visualiser les résultats du traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="97588-133">When the batch job is finished, open the **Resource Price Changes** window to see the results of the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-alternate-prices"></a><span data-ttu-id="97588-134">Pour obtenir des propositions de modification des prix ressource basées sur les prix standard</span><span class="sxs-lookup"><span data-stu-id="97588-134">To get resource price change suggestions based on alternate prices</span></span>  
<span data-ttu-id="97588-135">Si vous avez déjà configuré d'autres prix pour un certain nombre de ressources, vous pouvez utiliser un traitement en lot pour configurer d'autres prix ressource.</span><span class="sxs-lookup"><span data-stu-id="97588-135">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span></span>

1. <span data-ttu-id="97588-136">Dans la zone **Rechercher**, saisissez **Prop. modif. prix ress. (prix)**, puis sélectionnez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="97588-136">In the **Search** box, enter **Suggest Res. Price Chg. (Price)**, and then choose the related link.</span></span>  
2. <span data-ttu-id="97588-137">Renseignez les champs selon vos besoins.</span><span class="sxs-lookup"><span data-stu-id="97588-137">Fill in the fields as necessary.</span></span>
3. <span data-ttu-id="97588-138">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="97588-138">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="97588-139">Lorsque le traitement par lots est terminé, ouvrez la fenêtre **Nouv. prix ressource proposés** pour visualiser les résultats du traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="97588-139">When the batch job is finished, open the **Resource Price Changes** window to see the results of the batch job.</span></span>

## <a name="see-also"></a><span data-ttu-id="97588-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="97588-140">See Also</span></span>
[<span data-ttu-id="97588-141">Gérer des projets</span><span class="sxs-lookup"><span data-stu-id="97588-141">Manage Projects</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="97588-142">Finance</span><span class="sxs-lookup"><span data-stu-id="97588-142">Finance</span></span>](finance-setup.md)  
<span data-ttu-id="97588-143">[Gestion des achats](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="97588-143">[Manage Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="97588-144">[Gestion des ventes](sales-manage-sales.md)   </span><span class="sxs-lookup"><span data-stu-id="97588-144">[Manage Sales](sales-manage-sales.md)   </span></span>  
[<span data-ttu-id="97588-145">Utiliser Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="97588-145">Work With Dynamics NAV</span></span>](ui-work-product.md)  

