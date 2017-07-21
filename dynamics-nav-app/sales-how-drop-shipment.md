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
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: f636de789dc6b006a449ec59c390fab85e62b443
ms.contentlocale: fr-ca
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-make-drop-shipments"></a>Procédure : effectuer des livraisons directes
Lors d'une livraison directe, un ou plusieurs articles de l'un de vos fournisseurs sont livrés directement chez l'un de vos clients.

Lorsqu'une commande vente est marquée pour livraison directe, et lorsque vous créez une commande achat spécifiant le client dans le champ **N° donneur d'ordre** , vous pouvez ensuite associer les deux documents et par conséquent informer le fournisseur de procéder directement à l'envoi au client.

## <a name="to-create-a-sales-order-for-drop-shipment"></a>Pour créer un document de vente pour des livraisons directes
Pour préparer une livraison directe, vous créez un document de vente pour un article, sauf que vous devez indiquer sur la ligne vente que la vente exige la livraison directe.

1. Créez un document de vente pour un article. Pour en savoir plus, voir [Procédure : vendre des produits](sales-how-sell-products.md).
2. Sur la ligne commande vente pour l'article envoyé en livraison directe, cochez la case **Livraison directe**.

## <a name="to-create-the-purchase-order-for-drop-shipment"></a>Pour créer le bon de commande pour livraison directe
Pour préparer une livraison directe pour l'article mis en vente, vous créez un bon de commande, comme à l'accoutumée, sauf que vous devez indiquer sur le bon de commande qu'il doit être livré à votre client et non pas à vous-même.

1. Créez un bon de commande. Ne remplissez pas les champs sur les lignes. Pour plus d'informations, reportez-vous à [Procédure : enregistrer des achats](purchasing-how-record-purchases.md).
2. Dans le champ **N° donneur d'ordre** , sélectionnez le client auquel vous souhaitez vendre l'article en question.
3. Choisissez l'action **Livraisons directes**, puis choisissez l'option **Extraire commande vente**.
4. Dans la fenêtre **Liste des ventes**, sélectionnez la commande vente que vous avez préparée dans la section « Créer une commande vente pour livraison directe ».
5. Cliquez sur le bouton **OK**.

Les informations de ligne du document de vente sont insérées sur la/les ligne(s) bon de commande.

Vous pouvez maintenant informer le fournisseur quant à la livraison des articles à votre client, par exemple en envoyant le bon de commande au format PDF.     

## <a name="to-view-the-linked-purchase-order-from-the-sales-order"></a>Pour afficher le bon de commande associé à partir du document de vente
1. Sélectionnez la ligne commande vente livraison directe, choisissez l'action **Commande**, puis l'action **Livraison directe** et enfin l'action **Commande achat**.

Le bon de commande associé s'ouvre.

## <a name="to-post-a-drop-shipment"></a>Pour reporter une livraison directe
Lorsque le fournisseur a livré les articles, vous pouvez reporter le document de vente comme livré. Vous pouvez également valider la commande achat, mais uniquement avec l'option **Réceptionner** jusqu'à ce que la commande vente ait été facturée.
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Commandes vente**, puis sélectionnez le lien connexe.
2. Ouvrez les documents de vente que vous avez créés dans la section « Pour créer un document de vente pour une livraison directe ».
3. Dans le champ **Qté à expédier**, spécifiez la quantité de commandes à envoyer, la quantité de commandes partielles ou totales.
3. Sélectionnez l'action **Valider** ou **Valider et envoyer**.
4. Sélectionnez l'option **Livrer** pour facturer ultérieurement ou l'option **Livrer et facturer** pour facturer immédiatement.

## <a name="see-also"></a>Voir aussi
[Procédure : vendre des produits](sales-how-sell-products.md)    
[Procédure : enregistrer des achats](purchasing-how-record-purchases.md)  
[Gestion des ventes](sales-manage-sales.md)  
[Gestion du stock](inventory-manage-inventory.md)      
[Utiliser Dynamics NAV](ui-work-product.md)

