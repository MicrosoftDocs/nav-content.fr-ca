---
title: "Procédure : Reporter une écriture de fermeture de fin d'exercice"
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: fe32ee973c90ba857852ae092acf03db09e648ee
ms.contentlocale: fr-ca
ms.lasthandoff: 07/19/2017

---
# <a name="how-to-post-year-end-closing-entry"></a><span data-ttu-id="0dc49-102">Procédure : Reporter une écriture de fermeture de fin d'exercice</span><span class="sxs-lookup"><span data-stu-id="0dc49-102">How to: Post Year-End Closing Entry</span></span>
<span data-ttu-id="0dc49-103">Dans le cadre de la fermeture des registres pour un exercice financier, vous allez exécuter le traitement en lot Fermer l'état des résultats pour transférer le résultat annuel vers un compte de bilan et fermer les comptes d'état des résultats.</span><span class="sxs-lookup"><span data-stu-id="0dc49-103">As part of closing the books for a fiscal year, you will run the Close Income Statement batch job to transfer the year's result to an account in the balance sheet and close the income statement accounts.</span></span> <span data-ttu-id="0dc49-104">Après avoir utilisé le traitement en lot Fermer l'état des résultats, vous devez ouvrir le journal spécifié dans le traitement en lot, puis consulter et reporter les écritures.</span><span class="sxs-lookup"><span data-stu-id="0dc49-104">After you run the Close Income Statement batch job, you must open the journal you specified in the batch job, and then review and post the entries.</span></span>

## <a name="to-post-the-year-end-closing-entry"></a><span data-ttu-id="0dc49-105">Pour reporter l'écriture de fermeture de fin d'exercice</span><span class="sxs-lookup"><span data-stu-id="0dc49-105">To post the year end closing entry</span></span>
1. <span data-ttu-id="0dc49-106">Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Feuille comptabilité**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="0dc49-106">In the top right corner, choose the **Search for Page or Report** icon, enter **General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="0dc49-107">Dans la fenêtre **Feuille comptabilité**, dans le champ **Nom de la feuille**, sélectionnez la feuille qui contient les écritures de clôture.</span><span class="sxs-lookup"><span data-stu-id="0dc49-107">In the **General Journal** window, in the **Batch Name** field, select the batch that contains the closing entries.</span></span>
3. <span data-ttu-id="0dc49-108">Examinez les écritures.</span><span class="sxs-lookup"><span data-stu-id="0dc49-108">Review the entries.</span></span>
4. <span data-ttu-id="0dc49-109">Pour valider la feuille, sélectionnez l'action **Valider**.</span><span class="sxs-lookup"><span data-stu-id="0dc49-109">To post the journal, choose the **Post** action.</span></span>

<span data-ttu-id="0dc49-110">**Remarque** : en cas de détection d'une erreur, un message d'erreur s'affiche.</span><span class="sxs-lookup"><span data-stu-id="0dc49-110">**Note**: If an error is detected, an error message is displayed.</span></span> <span data-ttu-id="0dc49-111">Si le report réussit, les entrées reportées sont supprimées du journal.</span><span class="sxs-lookup"><span data-stu-id="0dc49-111">If the posting is successful, the posted entries are removed from the journal.</span></span> <span data-ttu-id="0dc49-112">Une fois le report terminé, une entrée est reportée sur chaque compte état des résultats, de façon à ce que son solde indique zéro et à ce que les résultats de l'exercice soient transférés dans le bilan.</span><span class="sxs-lookup"><span data-stu-id="0dc49-112">After posting is complete, an entry is posted to each income statement account so that its balance becomes zero and the year's result is transferred to the balance sheet.</span></span>

## <a name="see-also"></a><span data-ttu-id="0dc49-113">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0dc49-113">See Also</span></span>
[<span data-ttu-id="0dc49-114">Clôture des livres</span><span class="sxs-lookup"><span data-stu-id="0dc49-114">Close Books</span></span>](year-close-books.md)  
[<span data-ttu-id="0dc49-115">Clôturer exercice comptable</span><span class="sxs-lookup"><span data-stu-id="0dc49-115">Close Income Statement</span></span>](year-close-income-statement.md)  
[<span data-ttu-id="0dc49-116">Procédure : clôture des périodes comptables</span><span class="sxs-lookup"><span data-stu-id="0dc49-116">How to: Close Accounting Periods</span></span>](year-close-account-periods.md)  
