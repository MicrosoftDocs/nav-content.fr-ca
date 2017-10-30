---
title: "Vérifier et reporter l'écriture de fermeture de fin d'exercice"
description: "Décrit comment ouvrir le journal spécifié dans le traitement en lot Fermer l'état des résultats, puis examiner et reporter l'écriture de fermeture de fin d'exercice."
documentationcenter: 
author: jswymer
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: year closing, close accounting period, close fiscal year, bank account detailed trial balance
ms.date: 03/29/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: eeffd585b18c2b839db7be3f89d19497080b10ef
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-post-the-year-end-closing-entry"></a><span data-ttu-id="7a10c-103">Procédure : reporter l'écriture de fermeture de fin d'exercice</span><span class="sxs-lookup"><span data-stu-id="7a10c-103">How to: Post the Year-End Closing Entry</span></span>
<span data-ttu-id="7a10c-104">Après avoir utilisé le traitement par lots **Solder les comptes de gestion** pour générer les écritures de clôture d'exercice, vous devez ouvrir la feuille spécifiée dans le traitement par lots, puis consulter et valider les écritures.</span><span class="sxs-lookup"><span data-stu-id="7a10c-104">After you use the **Close Income Statement** batch job to generate the year-end closing entry or entries, you must open the journal you specified in the batch job, and then review and post the entries.</span></span>

## <a name="to-post-the-year-end-closing-entry"></a><span data-ttu-id="7a10c-105">Pour reporter l'écriture de fermeture de fin d'exercice</span><span class="sxs-lookup"><span data-stu-id="7a10c-105">To post the year end closing entry</span></span>
1. <span data-ttu-id="7a10c-106">Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Feuille comptabilité**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="7a10c-106">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="7a10c-107">Dans la fenêtre **Feuille comptabilité**, dans le champ **Nom de la feuille**, sélectionnez la feuille qui contient les écritures de clôture.</span><span class="sxs-lookup"><span data-stu-id="7a10c-107">In the **General Journal** window, in the **Batch Name** field, select the batch that contains the closing entries.</span></span>
3. <span data-ttu-id="7a10c-108">Examinez les écritures.</span><span class="sxs-lookup"><span data-stu-id="7a10c-108">Review the entries.</span></span>
4. <span data-ttu-id="7a10c-109">Pour valider la feuille, sélectionnez l'action **Valider**.</span><span class="sxs-lookup"><span data-stu-id="7a10c-109">To post the journal, choose the **Post** action.</span></span>

> [!NOTE]  
>   <span data-ttu-id="7a10c-110">En cas de détection d'une erreur, un message d'erreur s'affiche.</span><span class="sxs-lookup"><span data-stu-id="7a10c-110">If an error is detected, an error message is displayed.</span></span> <span data-ttu-id="7a10c-111">Si le report réussit, les entrées reportées sont supprimées du journal.</span><span class="sxs-lookup"><span data-stu-id="7a10c-111">If the posting is successful, the posted entries are removed from the journal.</span></span> <span data-ttu-id="7a10c-112">Une fois le report terminé, une entrée est reportée sur chaque compte état des résultats, de façon à ce que son solde indique zéro et à ce que les résultats de l'exercice soient transférés dans le bilan.</span><span class="sxs-lookup"><span data-stu-id="7a10c-112">After posting is complete, an entry is posted to each income statement account so that its balance becomes zero and the year's result is transferred to the balance sheet.</span></span>

## <a name="see-also"></a><span data-ttu-id="7a10c-113">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7a10c-113">See Also</span></span>
[<span data-ttu-id="7a10c-114">Procédure : clôture des périodes comptables</span><span class="sxs-lookup"><span data-stu-id="7a10c-114">How to: Close Accounting Periods</span></span>](year-close-account-periods.md)  
[<span data-ttu-id="7a10c-115">Clôture plans</span><span class="sxs-lookup"><span data-stu-id="7a10c-115">Closing Books</span></span>](year-close-books.md)  
[<span data-ttu-id="7a10c-116">Clôturer exercice comptable</span><span class="sxs-lookup"><span data-stu-id="7a10c-116">Close Income Statement</span></span>](year-close-income-statement.md)  
<span data-ttu-id="7a10c-117">[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="7a10c-117">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

