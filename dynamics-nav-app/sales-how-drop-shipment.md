---
title: "Créer un document de vente liée à un bon de commande pour une livraison directe"
description: "Décrit comment créer un document de vente liée à un bon de commande pour permettre la livraison directe du fournisseur au client."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: direct shipment
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 6a8210808532ff8945660c23f0bf91719e2f2963
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-make-drop-shipments"></a>Procédure : effectuer des livraisons directes
Lors d'une livraison directe, un ou plusieurs articles de l'un de vos fournisseurs sont livrés directement chez l'un de vos clients.

Lorsqu'une commande vente est marquée pour livraison directe, et lorsque vous créez une commande achat spécifiant le client dans le champ **N° donneur d'ordre** , vous pouvez ensuite associer les deux documents et par conséquent informer le fournisseur de procéder directement à la livraison au client.

## <a name="to-create-a-sales-order-for-drop-shipment"></a>Pour créer un document de vente pour des livraisons directes
Pour préparer une livraison directe, vous créez un document de vente pour un article, sauf que vous devez indiquer sur la ligne vente que la vente exige la livraison directe.

1. Créez un document de vente pour un article. Pour en savoir plus, voir [Procédure : vendre des produits](sales-how-sell-products.md).
2. Sur la ligne commande vente pour l'article envoyé, cochez la case **Livraison directe**. Utilisez la fonction **Choisir les colonnes** si le champ n'est pas visible. Pour plus d'informations, voir [Personnalisation utilisateur](ui-user-personalization.md).

## <a name="to-create-the-purchase-order-for-drop-shipment"></a>Pour créer le bon de commande pour livraison directe
Pour préparer une livraison directe pour l'article mis en vente, vous créez un bon de commande, comme à l'accoutumée, sauf que vous devez indiquer sur le bon de commande qu'il doit être envoyé à votre client et non pas à vous-même.

1. Créez un bon de commande. Ne remplissez pas les champs sur les lignes. Pour plus d'informations, reportez-vous à [Procédure : enregistrer des achats](purchasing-how-record-purchases.md).
2. Dans le champ **N° donneur d'ordre** , sélectionnez le client auquel vous souhaitez vendre l'article en question.
3. Choisissez l'action **Livraisons directes**, puis choisissez l'option **Extraire commande vente**.
4. Dans la fenêtre **Liste des ventes**, sélectionnez la commande vente que vous avez préparée dans la section « Créer une commande vente pour livraison directe ».
5. Cliquez sur le bouton **OK**.

Les informations de ligne du document de vente sont insérées sur la/les ligne(s) bon de commande.

Vous pouvez maintenant informer le fournisseur quant à la livraison des articles à votre client, par exemple en envoyant le bon de commande au format PDF.     

## <a name="to-view-the-linked-purchase-order-from-the-sales-order"></a>Pour afficher le bon de commande associé à partir du document de vente
* Sélectionnez la ligne commande vente livraison directe, choisissez l'action **Commande**, puis l'action **Livraison directe** et enfin l'action **Commande achat**.

## <a name="to-post-a-drop-shipment"></a>Pour reporter une livraison directe
Lorsque le fournisseur a livré les articles, vous pouvez reporter le document de vente comme envoyé. Vous pouvez également valider la commande achat, mais uniquement avec l'option **Réceptionner** jusqu'à ce que la commande vente ait été facturée.

1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Commandes vente**, puis sélectionnez le lien connexe.
2. Ouvrez les documents de vente que vous avez créés dans la section « Pour créer un document de vente pour une livraison directe ».
3. Dans le champ **Qté à expédier**, spécifiez la quantité de commandes à envoyer, la quantité de commandes partielles ou totales.
4. Sélectionnez l'action **Valider** ou **Valider et envoyer**.
5. Sélectionnez l'option **Livrer** pour facturer ultérieurement ou l'option **Livrer et facturer** pour facturer immédiatement.

## <a name="see-also"></a>Voir aussi
[Procédure : créer des commandes spéciales](sales-how-to-create-special-orders.md)|  
[Procédure : vendre des produits](sales-how-sell-products.md)  
[Procédure : enregistrer des achats](purchasing-how-record-purchases.md)  
[Vente](sales-manage-sales.md)  
[Stocks](inventory-manage-inventory.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

