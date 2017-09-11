---
title: "Procédure : effectuer des livraisons directes"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: a726c8c24d8f843b33b4df4d85ad2b5eab3790e7
ms.contentlocale: fr-ca
ms.lasthandoff: 07/19/2017

---

# <a name="how-to-make-drop-shipments"></a><span data-ttu-id="1759a-102">Procédure : effectuer des livraisons directes</span><span class="sxs-lookup"><span data-stu-id="1759a-102">How to: Make Drop Shipments</span></span>
<span data-ttu-id="1759a-103">Lors d'une livraison directe, un ou plusieurs articles de l'un de vos fournisseurs sont livrés directement chez l'un de vos clients.</span><span class="sxs-lookup"><span data-stu-id="1759a-103">A drop shipment is the shipment of items from one of your vendors directly to one of your customers.</span></span>

<span data-ttu-id="1759a-104">Lorsqu'une commande vente est marquée pour livraison directe, et lorsque vous créez une commande achat spécifiant le client dans le champ **N° donneur d'ordre**</span><span class="sxs-lookup"><span data-stu-id="1759a-104">When a sales order is marked for drop shipment, and you create a purchase order specifying the customer in the **Sell-to Customer No.**</span></span> <span data-ttu-id="1759a-105">, vous pouvez ensuite associer les deux documents et par conséquent informer le fournisseur de procéder directement à l'envoi au client.</span><span class="sxs-lookup"><span data-stu-id="1759a-105">field, then you can link the two documents and thereby instruct the vendor to ship directly to the customer.</span></span>

## <a name="to-create-a-sales-order-for-drop-shipment"></a><span data-ttu-id="1759a-106">Pour créer un document de vente pour des livraisons directes</span><span class="sxs-lookup"><span data-stu-id="1759a-106">To create a sales order for drop shipment</span></span>
<span data-ttu-id="1759a-107">Pour préparer une livraison directe, vous créez un document de vente pour un article, sauf que vous devez indiquer sur la ligne vente que la vente exige la livraison directe.</span><span class="sxs-lookup"><span data-stu-id="1759a-107">To prepare a drop shipment, you create a sales order for an item as normal, except you must indicate on the sales line that the sale requires drop shipment.</span></span>

1. <span data-ttu-id="1759a-108">Créez un document de vente pour un article.</span><span class="sxs-lookup"><span data-stu-id="1759a-108">Create a sales order for an item.</span></span> <span data-ttu-id="1759a-109">Pour en savoir plus, voir [Procédure : vendre des produits](sales-how-sell-products.md).</span><span class="sxs-lookup"><span data-stu-id="1759a-109">For more information, see [How to: Sell Products](sales-how-sell-products.md).</span></span>
2. <span data-ttu-id="1759a-110">Sur la ligne commande vente pour l'article envoyé en livraison directe, cochez la case **Livraison directe**.</span><span class="sxs-lookup"><span data-stu-id="1759a-110">On the sales order line for the drop-shipment item, select the **Drop Shipment** check box.</span></span>

## <a name="to-create-the-purchase-order-for-drop-shipment"></a><span data-ttu-id="1759a-111">Pour créer le bon de commande pour livraison directe</span><span class="sxs-lookup"><span data-stu-id="1759a-111">To create the purchase order for drop shipment</span></span>
<span data-ttu-id="1759a-112">Pour préparer une livraison directe pour l'article mis en vente, vous créez un bon de commande, comme à l'accoutumée, sauf que vous devez indiquer sur le bon de commande qu'il doit être livré à votre client et non pas à vous-même.</span><span class="sxs-lookup"><span data-stu-id="1759a-112">To prepare a drop shipment for the item to be sold, you create a purchase order as normal, except you must indicate on the purchase order that it must be shipped to your customer, not to yourself.</span></span>

1. <span data-ttu-id="1759a-113">Créez un bon de commande.</span><span class="sxs-lookup"><span data-stu-id="1759a-113">Create a purchase order.</span></span> <span data-ttu-id="1759a-114">Ne remplissez pas les champs sur les lignes.</span><span class="sxs-lookup"><span data-stu-id="1759a-114">Do not fill any fields on the lines.</span></span> <span data-ttu-id="1759a-115">Pour plus d'informations, reportez-vous à [Procédure : enregistrer des achats](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="1759a-115">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).</span></span>
2. <span data-ttu-id="1759a-116">Dans le champ **N° donneur d'ordre**</span><span class="sxs-lookup"><span data-stu-id="1759a-116">In the **Sell-to Customer No.**</span></span> <span data-ttu-id="1759a-117">, sélectionnez le client auquel vous souhaitez vendre l'article en question.</span><span class="sxs-lookup"><span data-stu-id="1759a-117">field, select the customer that you are selling to.</span></span>
3. <span data-ttu-id="1759a-118">Choisissez l'action **Livraisons directes**, puis choisissez l'option **Extraire commande vente**.</span><span class="sxs-lookup"><span data-stu-id="1759a-118">Choose the **Drop Shipments** action, and then choose the **Get Sales Order** action.</span></span>
4. <span data-ttu-id="1759a-119">Dans la fenêtre **Liste des ventes**, sélectionnez la commande vente que vous avez préparée dans la section « Créer une commande vente pour livraison directe ».</span><span class="sxs-lookup"><span data-stu-id="1759a-119">In the **Sales List** window, select the sales order that you prepared in the "To create a sales order for drop shipment" section.</span></span>
5. <span data-ttu-id="1759a-120">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="1759a-120">Choose the **OK** button.</span></span>

<span data-ttu-id="1759a-121">Les informations de ligne du document de vente sont insérées sur la/les ligne(s) bon de commande.</span><span class="sxs-lookup"><span data-stu-id="1759a-121">The line information from the sales order is inserted on the purchase order line(s).</span></span>

<span data-ttu-id="1759a-122">Vous pouvez maintenant informer le fournisseur quant à la livraison des articles à votre client, par exemple en envoyant le bon de commande au format PDF.</span><span class="sxs-lookup"><span data-stu-id="1759a-122">You can now instruct the vendor to ship the items to your customer, for example, by mailing the purchase order as a PDF.</span></span>     

## <a name="to-view-the-linked-purchase-order-from-the-sales-order"></a><span data-ttu-id="1759a-123">Pour afficher le bon de commande associé à partir du document de vente</span><span class="sxs-lookup"><span data-stu-id="1759a-123">To view the linked purchase order from the sales order</span></span>
1. <span data-ttu-id="1759a-124">Sélectionnez la ligne commande vente livraison directe, choisissez l'action **Commande**, puis l'action **Livraison directe** et enfin l'action **Commande achat**.</span><span class="sxs-lookup"><span data-stu-id="1759a-124">Select the drop-shipment sales order line, choose the **Order** action, choose the **Drop Shipment** action, and then choose the **Purchase Order** action.</span></span>

<span data-ttu-id="1759a-125">Le bon de commande associé s'ouvre.</span><span class="sxs-lookup"><span data-stu-id="1759a-125">The linked purchase order opens.</span></span>

## <a name="to-post-a-drop-shipment"></a><span data-ttu-id="1759a-126">Pour reporter une livraison directe</span><span class="sxs-lookup"><span data-stu-id="1759a-126">To post a drop shipment</span></span>
<span data-ttu-id="1759a-127">Lorsque le fournisseur a livré les articles, vous pouvez reporter le document de vente comme livré.</span><span class="sxs-lookup"><span data-stu-id="1759a-127">When the vendor has shipped the items, you can post the sales order as shipped.</span></span> <span data-ttu-id="1759a-128">Vous pouvez également valider la commande achat, mais uniquement avec l'option **Réceptionner** jusqu'à ce que la commande vente ait été facturée.</span><span class="sxs-lookup"><span data-stu-id="1759a-128">You can also post the purchase order, but only with the **Receive** option until the sales order has been invoiced.</span></span>
1. <span data-ttu-id="1759a-129">Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Commandes vente**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="1759a-129">In the top right corner, choose the **Search for Page or Report** icon, enter **Sales orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="1759a-130">Ouvrez les documents de vente que vous avez créés dans la section « Pour créer un document de vente pour une livraison directe ».</span><span class="sxs-lookup"><span data-stu-id="1759a-130">Open the sales order that you created in the "To create a sales order for a drop shipment" section.</span></span>
3. <span data-ttu-id="1759a-131">Dans le champ **Qté à expédier**, spécifiez la quantité de commandes à envoyer, la quantité de commandes partielles ou totales.</span><span class="sxs-lookup"><span data-stu-id="1759a-131">In the **Qty. to Ship** field, specify how many of the order quantity to ship, the full or a partial order quantity.</span></span>
3. <span data-ttu-id="1759a-132">Sélectionnez l'action **Valider** ou **Valider et envoyer**.</span><span class="sxs-lookup"><span data-stu-id="1759a-132">Choose the **Post** or **Post and Send** action.</span></span>
4. <span data-ttu-id="1759a-133">Sélectionnez l'option **Livrer** pour facturer ultérieurement ou l'option **Livrer et facturer** pour facturer immédiatement.</span><span class="sxs-lookup"><span data-stu-id="1759a-133">Choose either the **Ship** option to invoice later, or the **Ship and Invoice** option to invoice immediately.</span></span>

## <a name="see-also"></a><span data-ttu-id="1759a-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1759a-134">See Also</span></span>
<span data-ttu-id="1759a-135">[Procédure : vendre des produits](sales-how-sell-products.md)  </span><span class="sxs-lookup"><span data-stu-id="1759a-135">[How to: Sell Products](sales-how-sell-products.md)  </span></span>  
[<span data-ttu-id="1759a-136">Procédure : enregistrer des achats</span><span class="sxs-lookup"><span data-stu-id="1759a-136">How to: Record Purchases</span></span>](purchasing-how-record-purchases.md)  
[<span data-ttu-id="1759a-137">Gestion des ventes</span><span class="sxs-lookup"><span data-stu-id="1759a-137">Manage Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="1759a-138">[Gestion du stock](inventory-manage-inventory.md)    </span><span class="sxs-lookup"><span data-stu-id="1759a-138">[Manage Inventory](inventory-manage-inventory.md)    </span></span>  
[<span data-ttu-id="1759a-139">Utiliser Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="1759a-139">Work with Dynamics NAV</span></span>](ui-work-product.md)

