---
title: "Fermer des périodes"
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: ac1ed2d1dcf8bf780bda91fbf0a04e5c5e8d106a
ms.contentlocale: fr-ca
ms.lasthandoff: 06/26/2017

---
# <a name="close-periods"></a><span data-ttu-id="b635c-102">Fermer des périodes</span><span class="sxs-lookup"><span data-stu-id="b635c-102">Close Periods</span></span>
<span data-ttu-id="b635c-103">L'application ne vous oblige pas à fermer les périodes. Toutefois, il existe de nombreuses activités de fin de période (fin de mois) que vous pouvez effectuer dans l'application si vous le souhaitez.</span><span class="sxs-lookup"><span data-stu-id="b635c-103">The application does not force you to close periods, however, there are many period-end (month-end) activities that can be performed in the application if you want.</span></span> <span data-ttu-id="b635c-104">Cette rubrique présente un aperçu de ces processus et activités, qui peuvent ou non être nécessaires pour votre compagnie.</span><span class="sxs-lookup"><span data-stu-id="b635c-104">This topic provides an overview of these processes and activities, which may or may not be necessary for your company.</span></span>

## <a name="general-ledger"></a><span data-ttu-id="b635c-105">Grand livre</span><span class="sxs-lookup"><span data-stu-id="b635c-105">General Ledger</span></span>
* <span data-ttu-id="b635c-106">Spécifiez des périodes de report à l'échelle du système et spécifiques à l'utilisateur.</span><span class="sxs-lookup"><span data-stu-id="b635c-106">Specify system-wide and user-specific posting period.</span></span>

    <span data-ttu-id="b635c-107">Cela spécifie les dates entre lesquelles les validation sont autorisées.</span><span class="sxs-lookup"><span data-stu-id="b635c-107">This specifies the dates between which postings are allowed.</span></span> <span data-ttu-id="b635c-108">En fonction des besoins de votre activité, vous pouvez restreindre les plages de date de report utilisateur au début du processus de fin d'exercice ou à une date ultérieure vers la fin de l'exercice.</span><span class="sxs-lookup"><span data-stu-id="b635c-108">Depending on your business needs, you may want to restrict user posting date ranges at the start of the period-end process or at later time towards the end of the period.</span></span> <span data-ttu-id="b635c-109">Pour plus d'informations, reportez vous à [Procédure: spécifier des périodes de validation](finance-setup-how-specify-posting-periods.md).</span><span class="sxs-lookup"><span data-stu-id="b635c-109">For more information, see [How to: Specify Posting Periods](finance-setup-how-specify-posting-periods.md).</span></span>
* <span data-ttu-id="b635c-110">Effectuez tous les ajustements nécessaires dans le GL.</span><span class="sxs-lookup"><span data-stu-id="b635c-110">Make all necessary G/L adjustments.</span></span>
* <span data-ttu-id="b635c-111">Mettez à jour et reportez les journaux récurrents.</span><span class="sxs-lookup"><span data-stu-id="b635c-111">Update and post Recurring Journals.</span></span>
<!--* Process Consolidations-->
* <span data-ttu-id="b635c-112">Exécutez les tableaux d'analyse comme suit :</span><span class="sxs-lookup"><span data-stu-id="b635c-112">Run account schedules as follows:</span></span>
  1. <span data-ttu-id="b635c-113">Ouvrez la fenêtre **Tableau d'analyse**, puis sélectionnez l'action **Imprimer**.</span><span class="sxs-lookup"><span data-stu-id="b635c-113">Open the **Account Schedule** window, and choose the **Print** action.</span></span>
  2. <span data-ttu-id="b635c-114">Renseignez le formulaire de sélection **Tableau d'analyse**, puis sélectionnez l'action **Imprimer**.</span><span class="sxs-lookup"><span data-stu-id="b635c-114">Fill the **Account Schedule** request window and choose the **Print** action.</span></span>

## <a name="sales--receivables"></a><span data-ttu-id="b635c-115">Ventes</span><span class="sxs-lookup"><span data-stu-id="b635c-115">Sales & Receivables</span></span>
* <span data-ttu-id="b635c-116">Reportez l'ensemble des documents de vente, factures, notes de crédit et retours vente.</span><span class="sxs-lookup"><span data-stu-id="b635c-116">Post all sales orders, invoices, credit memos, and return orders.</span></span>
* <span data-ttu-id="b635c-117">Reportez l'ensemble des journaux des encaissements.</span><span class="sxs-lookup"><span data-stu-id="b635c-117">Post all cash receipt journals.</span></span>
* <span data-ttu-id="b635c-118">Mettez à jour et validez les feuilles abonnement associées aux ventes.</span><span class="sxs-lookup"><span data-stu-id="b635c-118">Update and post recurring journals that are related to Sales & Receivables.</span></span>
* <span data-ttu-id="b635c-119">Rapprocher les comptes clients avec le grand livre.</span><span class="sxs-lookup"><span data-stu-id="b635c-119">Reconcile accounts receivable to the general ledger.</span></span>
* <span data-ttu-id="b635c-120">Exécutez le traitement par lots **Supprimer cdes vente facturées**.</span><span class="sxs-lookup"><span data-stu-id="b635c-120">Run the **Delete Invoiced Sales Orders** batch job.</span></span>

## <a name="purchases--payables"></a><span data-ttu-id="b635c-121">Achats</span><span class="sxs-lookup"><span data-stu-id="b635c-121">Purchases & Payables</span></span>
* <span data-ttu-id="b635c-122">Reportez l'ensemble des bons de commande, factures, notes de crédit et retours achat.</span><span class="sxs-lookup"><span data-stu-id="b635c-122">Post all purchase orders, invoices, credit memos, and return orders.</span></span>
* <span data-ttu-id="b635c-123">Reportez l'ensemble des journaux paiement.</span><span class="sxs-lookup"><span data-stu-id="b635c-123">Post all payment journals.</span></span>
* <span data-ttu-id="b635c-124">Mettez à jour et validez les feuilles abonnement associées aux achats.</span><span class="sxs-lookup"><span data-stu-id="b635c-124">Update and post recurring journals that are related to purchases & payables.</span></span>
* <span data-ttu-id="b635c-125">Générez l'état **Comptabilité fournisseur âgée** et rapprochez la comptabilité fournisseur de la comptabilité.</span><span class="sxs-lookup"><span data-stu-id="b635c-125">Run the **Aged Accounts Payable** report and reconcile accounts payable to the general ledger.</span></span>
* <span data-ttu-id="b635c-126">Exécutez le traitement par lots **Supprimer cdes achat facturées**.</span><span class="sxs-lookup"><span data-stu-id="b635c-126">Run the **Delete Invoiced Purchase Orders** batch job.</span></span>

<!-- ### Fixed Assets
* Post all maintenance costs have been posted through the fixed asset journals or invoices.
* Post adjustments.
* Post appreciation.
* Post depreciation.
* Update and post the recurring fixed asset journal.-->

<!--### Intercompany
* Process Intercompany Postings.-->

## <a name="calculate-and-process-sales-tax"></a><span data-ttu-id="b635c-127">Calculez et traitez la taxe de vente.</span><span class="sxs-lookup"><span data-stu-id="b635c-127">Calculate and Process Sales Tax</span></span>
*  <span data-ttu-id="b635c-128">Renseignez les déclarations de TVA.</span><span class="sxs-lookup"><span data-stu-id="b635c-128">Complete Tax Statements.</span></span>

## <a name="see-also"></a><span data-ttu-id="b635c-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b635c-129">See Also</span></span>
[<span data-ttu-id="b635c-130">Clôture des exercices et des périodes</span><span class="sxs-lookup"><span data-stu-id="b635c-130">Closing Years and Periods</span></span>](year-close-years-periods.md)  
[<span data-ttu-id="b635c-131">Clôture des livres</span><span class="sxs-lookup"><span data-stu-id="b635c-131">Close Books</span></span>](year-close-books.md)

