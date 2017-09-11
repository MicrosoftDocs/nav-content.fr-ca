---
title: "Créer des séries de numéros"
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: e42e5ed139b2487fea13ef0fd57757035764addd
ms.contentlocale: fr-ca
ms.lasthandoff: 07/19/2017

---

# <a name="create-number-series"></a><span data-ttu-id="f1553-102">Créer des séries de numéros</span><span class="sxs-lookup"><span data-stu-id="f1553-102">Create Number Series</span></span>

<span data-ttu-id="f1553-103">Pour chaque compagnie que vous configurez, vous devez affecter des codes d'identification uniques aux éléments tels que les comptes du grand livre, les comptes client et fournisseur, les factures et les documents.</span><span class="sxs-lookup"><span data-stu-id="f1553-103">For each company that you set up, you need to assign unique identification codes to things such as general ledger accounts, customer and vendor accounts, invoices, and documents.</span></span> <span data-ttu-id="f1553-104">La numérotation est importante, pas uniquement pour l'identification.</span><span class="sxs-lookup"><span data-stu-id="f1553-104">Numbering is important not only for identification.</span></span> <span data-ttu-id="f1553-105">Un système de numérotation bien conçu facilite également la gestion et l'analyse de la compagnie et permet de réduire les erreurs de saisie des données.</span><span class="sxs-lookup"><span data-stu-id="f1553-105">A well-designed numbering system also makes the company more manageable and easy to analyze, and can reduce the number of errors that occur in data entry.</span></span>

<span data-ttu-id="f1553-106">Vous pouvez configurer un système de numérotation complet avec un nombre illimité de séries de numéros.</span><span class="sxs-lookup"><span data-stu-id="f1553-106">You can set up a complete numbering system with an unlimited number of number series.</span></span> <span data-ttu-id="f1553-107">Vous pouvez utiliser des séries de numéros pour tous les types de documents et journaux, ainsi que pour les données de base, telles que les clients, les articles et les projets.</span><span class="sxs-lookup"><span data-stu-id="f1553-107">You can use number series for all types of documents and journals, as well as for master data such as customers, items, and jobs.</span></span>

<span data-ttu-id="f1553-108">Vous pouvez combiner l'utilisation des séries de numéros et la numérotation manuelle.</span><span class="sxs-lookup"><span data-stu-id="f1553-108">You can combine the use of number series with manual numbering.</span></span>

<span data-ttu-id="f1553-109">Vous créez un système de numérotation en définissant un ou plusieurs codes pour chaque type de données de base ou de document.</span><span class="sxs-lookup"><span data-stu-id="f1553-109">You create a numbering system by setting up one or more codes for each type of master data or document.</span></span> <span data-ttu-id="f1553-110">Par exemple, vous pouvez définir un code pour la numérotation de clients, un code pour la numérotation des factures vente et un autre code pour la numérotation des documents dans les feuilles comptabilité.</span><span class="sxs-lookup"><span data-stu-id="f1553-110">For example, you can set up one code for numbering customers, another code for numbering sales invoices, and another code for numbering documents in general journals.</span></span>

<span data-ttu-id="f1553-111">Une fois que vous avez défini un code, vous devez définir au moins une ligne série de numéros.</span><span class="sxs-lookup"><span data-stu-id="f1553-111">After you have set up a code, you set must set up at least one number series line.</span></span> <span data-ttu-id="f1553-112">La ligne série de numéros contient des informations telles que les premier et dernier numéros de la série et la date début.</span><span class="sxs-lookup"><span data-stu-id="f1553-112">The number series line contains information such as the first and last number in the series and the starting date.</span></span> <span data-ttu-id="f1553-113">Vous pouvez définir plusieurs lignes série de numéros par code série de numéros, avec une date début différente pour chaque ligne.</span><span class="sxs-lookup"><span data-stu-id="f1553-113">You can set up more than one number series line per number series code, with a different starting date for each line.</span></span> <span data-ttu-id="f1553-114">Les séries sont utilisées de manière consécutive, chaque série commençant à la date début respective.</span><span class="sxs-lookup"><span data-stu-id="f1553-114">The series will be used consecutively, starting each series on the respective starting date.</span></span>

<span data-ttu-id="f1553-115">Si vous voulez utiliser plusieurs codes série de numéros pour un type de données de base (par exemple, si vous voulez utiliser différentes séries de numéros pour diverses catégories d'articles), vous pouvez utiliser des liens de séries de numéros.</span><span class="sxs-lookup"><span data-stu-id="f1553-115">If you want to use more than one number series code for one type of master data - for example, if you want to use different number series for different categories of items - you can use number series relationships.</span></span>

<span data-ttu-id="f1553-116">Outre les numéros affectés manuellement ou à l'aide du système de numérotation, toutes les transactions (écritures) se voient automatiquement affecter des numéros consécutifs.</span><span class="sxs-lookup"><span data-stu-id="f1553-116">In addition to the numbers that you assign manually or by use of the numbering system, all transactions (ledger entries) are automatically assigned consecutive numbers.</span></span> <span data-ttu-id="f1553-117">Ces numéros s'affichent dans le champ **N° écriture**</span><span class="sxs-lookup"><span data-stu-id="f1553-117">These numbers can be seen in the **Entry No.**</span></span> <span data-ttu-id="f1553-118">de toutes les fenêtres écritures.</span><span class="sxs-lookup"><span data-stu-id="f1553-118">field in all the ledger entry windows.</span></span> <span data-ttu-id="f1553-119">Vous ne pouvez pas les modifier ni les supprimer.</span><span class="sxs-lookup"><span data-stu-id="f1553-119">You cannot modify or delete these numbers.</span></span>

## <a name="to-create-relationships-between-number-series"></a><span data-ttu-id="f1553-120">Pour créer des liens entre des séries de numéros</span><span class="sxs-lookup"><span data-stu-id="f1553-120">To create relationships between number series</span></span>
<span data-ttu-id="f1553-121">Si vous avez défini plusieurs codes série de numéros pour un même type d'informations ou de transactions de base, vous pouvez créer des liens entre ces codes.</span><span class="sxs-lookup"><span data-stu-id="f1553-121">If you have set up more than one number series code for the same kind of basic information or transactions, you can create relationships between the codes.</span></span> <span data-ttu-id="f1553-122">Cette fonction peut vous aider à choisir parmi ces codes lorsque vous utilisez un numéro.</span><span class="sxs-lookup"><span data-stu-id="f1553-122">This feature can assist you in deciding among the codes when you use a number.</span></span>

1. <span data-ttu-id="f1553-123">Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Souches de n°**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="f1553-123">In the top right corner, choose the **Search for Page or Report** icon, enter **No. Series**, and then choose the related link.</span></span>
2. <span data-ttu-id="f1553-124">Sélectionnez la ligne avec la souche de numéros pour laquelle vous souhaitez créer des relations, puis cliquez sur **Relations**.</span><span class="sxs-lookup"><span data-stu-id="f1553-124">Select the line with the number series you want to create relationships for and then choose **Relationships**.</span></span>
3. <span data-ttu-id="f1553-125">Dans le champ **Code souche**, entrez le code de la souche de numéros à lier à la souche sélectionnée à l'étape 2.</span><span class="sxs-lookup"><span data-stu-id="f1553-125">In the **Series Code** field, enter the code for the number series that you want to relate to the series you selected in step 2.</span></span>
4. <span data-ttu-id="f1553-126">Ajoutez une ligne pour chaque code à lier à la série de numéros sélectionnée.</span><span class="sxs-lookup"><span data-stu-id="f1553-126">Add a line for each code that you want to relate to the selected number series.</span></span>
5. <span data-ttu-id="f1553-127">Fermez la fenêtre.</span><span class="sxs-lookup"><span data-stu-id="f1553-127">Close the window.</span></span>

<span data-ttu-id="f1553-128">Désormais, pour créer un élément nécessitant un numéro, vous pourrez utiliser les liens ainsi créés et choisir parmi les séries de numéros liées.</span><span class="sxs-lookup"><span data-stu-id="f1553-128">Now when you set up something that requires a number, you can use the relationships you created to select among the related number series.</span></span>

## <a name="see-also"></a><span data-ttu-id="f1553-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f1553-129">See Also</span></span>
[<span data-ttu-id="f1553-130">Utiliser Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="f1553-130">Work with Dynamics NAV</span></span>](ui-work-product.md)

