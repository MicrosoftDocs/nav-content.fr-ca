---
title: Comment imprimer un avis de remise
description: "Vous pouvez aider vos fournisseurs à effectuer des rapprochements en imprimant des avis de remise avant de reporter un journal des paiements et après avoir reporté un règlement."
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/26/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 7c7004ac5ded9436861bf5034f59a9c2bcd99dd0
ms.contentlocale: fr-ca
ms.lasthandoff: 12/01/2017

---

#<a name="how-to-print-remittance-advice"></a><span data-ttu-id="be844-103">Procédure : imprimer un avis de remise</span><span class="sxs-lookup"><span data-stu-id="be844-103">How to: Print Remittance Advice</span></span>
<span data-ttu-id="be844-104">Vous pouvez imprimer l'avis de remise avant de reporter un journal des paiements et après avoir reporté un règlement.</span><span class="sxs-lookup"><span data-stu-id="be844-104">You can print remittance advice before posting a payment journal and after posting a payment.</span></span> <span data-ttu-id="be844-105">Cette option affiche les numéros de facture fournisseur, ce qui permet aux fournisseurs d'effectuer les rapprochements.</span><span class="sxs-lookup"><span data-stu-id="be844-105">This advice displays vendor invoice numbers, which helps vendors to perform reconciliations.</span></span>

##<a name="to-print-remittance-advice"></a><span data-ttu-id="be844-106">Pour imprimer un avis de remise</span><span class="sxs-lookup"><span data-stu-id="be844-106">To print remittance advice</span></span>
1. <span data-ttu-id="be844-107">Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Feuilles paiement**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="be844-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="be844-108">Dans la fenêtre **Journal des paiements**, sélectionnez le paiement pour lequel l'avis de remise doit être imprimé.</span><span class="sxs-lookup"><span data-stu-id="be844-108">In the **Payment Journal** window, select the payment for which remittance advice must be printed.</span></span>  
3. <span data-ttu-id="be844-109">Choisissez l'action **Imprimer l'avis de remise**.</span><span class="sxs-lookup"><span data-stu-id="be844-109">Choose the **Print Remittance Advice** action.</span></span>  
4. <span data-ttu-id="be844-110">Dans le traitement en lot **Avis de remise - Journal**, sous le raccourci **Ligne journal général**, sélectionnez les filtres appropriés.</span><span class="sxs-lookup"><span data-stu-id="be844-110">In the **Remittance Advice - Journal** batch job, on the **Fen. Journal Line** FastTab, choose the appropriate filters.</span></span>  
  
    >[!Note]
    > <span data-ttu-id="be844-111">Vous pouvez appliquer un filtre en utilisant le numéro de document externe provenant du fournisseur pour refléter les paiements avec les factures.</span><span class="sxs-lookup"><span data-stu-id="be844-111">You can filter using the vendor's external document number to match payments with invoices.</span></span>

5. <span data-ttu-id="be844-112">Sur le raccourci **Fournisseur**, choisissez les filtres appropriés.</span><span class="sxs-lookup"><span data-stu-id="be844-112">On the **Vendor** FastTab, choose the appropriate filters.</span></span>  
6. <span data-ttu-id="be844-113">Choisissez **Imprimer** pour imprimer le rapport ou **Aperçu** pour l'afficher maintenant.</span><span class="sxs-lookup"><span data-stu-id="be844-113">Choose **Print** to print the report, or choose **Preview** to view it now.</span></span>  

## <a name="using-remittance-advice-reports"></a><span data-ttu-id="be844-114">Utilisation des rapports d'avis de remise</span><span class="sxs-lookup"><span data-stu-id="be844-114">Using Remittance Advice Reports</span></span>
<span data-ttu-id="be844-115">Le tableau suivant décrit les rapports que vous pouvez utiliser avec les avis de remise :</span><span class="sxs-lookup"><span data-stu-id="be844-115">The following table describes the reports that you can use with remittance advice:</span></span>

|<span data-ttu-id="be844-116">Rapport</span><span class="sxs-lookup"><span data-stu-id="be844-116">Report</span></span>|<span data-ttu-id="be844-117">Description</span><span class="sxs-lookup"><span data-stu-id="be844-117">Description</span></span>|
|----|----|
|<span data-ttu-id="be844-118">Rapport Avis de remise - Journal</span><span class="sxs-lookup"><span data-stu-id="be844-118">Remittance Advice - Journal Report</span></span>|<span data-ttu-id="be844-119">Ce rapport indique les documents qui sont inclus dans le paiement.</span><span class="sxs-lookup"><span data-stu-id="be844-119">This report indicates which documents are included in the payment.</span></span> <span data-ttu-id="be844-120">Pour les lignes journal général, vous pouvez spécifier le modèle journal et le lot journal à partir desquels les avis de remise seront imprimés, la date de la première activité à imprimer, et filtrer sur un numéro de document.</span><span class="sxs-lookup"><span data-stu-id="be844-120">For general journal lines, you can specify the journal template and journal batch from which the remittance advices will be printed, the date of the first activity to print, and filter on a document number.</span></span> <span data-ttu-id="be844-121">Pour les fournisseurs, vous pouvez saisir les numéros de fournisseur à inclure dans le rapport.</span><span class="sxs-lookup"><span data-stu-id="be844-121">For vendors, you can enter the vendor numbers to include in the report.</span></span> |
|<span data-ttu-id="be844-122">Rapport Avis de remise - Écritures</span><span class="sxs-lookup"><span data-stu-id="be844-122">Remittance Advice - Entries Report</span></span>| <span data-ttu-id="be844-123">Ce rapport indique les documents qui sont inclus dans le paiement.</span><span class="sxs-lookup"><span data-stu-id="be844-123">This report indicates which documents are included in the payment.</span></span> <span data-ttu-id="be844-124">Définissez le contenu du rapport en définissant des filtres.</span><span class="sxs-lookup"><span data-stu-id="be844-124">You define the report contents by setting filters.</span></span> <span data-ttu-id="be844-125">Vous pouvez définir des champs supplémentaires sous l'onglet en cliquant sur le champ **Champ**.</span><span class="sxs-lookup"><span data-stu-id="be844-125">You can set additional fields on the tab by choosing the **Field** field.</span></span> <span data-ttu-id="be844-126">Pour les écritures fournisseur, vous pouvez spécifier les fournisseurs à inclure dans le rapport, la date de la première activité d'impression, la devise et le numéro d'écriture à inclure.</span><span class="sxs-lookup"><span data-stu-id="be844-126">For vendor ledger entries, you can specify the vendors to include in the report, the date of the first activity to print, the currency, and the entry number to include.</span></span> |

> [!Note]
> <span data-ttu-id="be844-127">Le rapport Avis de remise - Journal ne prend pas en charge les scénarios d'affectation de devises croisées ni les tolérances de règlement.</span><span class="sxs-lookup"><span data-stu-id="be844-127">The Remittance Advice - Journal Report does not support cross currency application scenarios or payment tolerances.</span></span> <span data-ttu-id="be844-128">Pour en savoir plus, voir [Procédure : activer le lettrage d'écritures comptables client en devises différentes](finance-how-enable-application-ledger-entries-different-currencies.md).</span><span class="sxs-lookup"><span data-stu-id="be844-128">For more information, see [How to: Enable Application of Ledger Entries in Different Currencies](finance-how-enable-application-ledger-entries-different-currencies.md).</span></span>

> [!Tip]
> <span data-ttu-id="be844-129">Pour plus d'informations sur l'utilisation des rapports, consultez [Affichage de rapports de test avant le report](ui-how-view-test-reports-posting.md), [Utiliser des rapports](ui-work-report.md) et [Recherche, filtrage et tri de données](ui-enter-criteria-filters.md).</span><span class="sxs-lookup"><span data-stu-id="be844-129">For more information about how to work with reports, see [Viewing Test Reports before Posting](ui-how-view-test-reports-posting.md), [Work with Reports](ui-work-report.md), and [Searching, Filtering, and Sorting Data](ui-enter-criteria-filters.md).</span></span>

##<a name="see-also"></a><span data-ttu-id="be844-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="be844-130">See Also</span></span>  
[<span data-ttu-id="be844-131">Bienvenue dans Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="be844-131">Welcome to Dynamics NAV</span></span>](across-get-started.md)
