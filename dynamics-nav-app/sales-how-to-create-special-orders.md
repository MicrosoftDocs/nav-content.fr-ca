---
title: "Procédure : créer des commandes spéciales"
description: "Vous pouvez créer une commande spéciale pour un article spécifique non stocké à livrer à un client particulier. Le fournisseur livre l'article à votre entrepôt et vous pouvez ensuite le livrer à votre client seul ou avec d'autres articles issus d'autres commandes."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 6460c643a07f92e478aafb84044c90ff3ed3a236
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-special-orders"></a>Procédure : créer des commandes spéciales
Vous pouvez créer une commande spéciale pour un article spécifique non stocké à livrer à un client particulier. Le fournisseur livre l'article à votre entrepôt et vous pouvez ensuite le livrer à votre client seul ou avec d'autres articles issus d'autres commandes.  

Dans le cadre d'une commande spéciale, le bon de commande et le document de vente sont liés pour s'assurer que l'article non stocké précis est prélevé et livré au client.  

Pour pouvoir utiliser cette fonction, vous devez d'abord configurer les fiches client, fournisseur, et article nécessaires à la commande.  

## <a name="to-create-a-special-order"></a>Pour créer une commande spéciale  
1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Document de vente**, puis sélectionnez le lien associé.  
2. Sélectionnez l'action **Nouveau**. Créez et renseignez un document de vente pour l'article. Pour en savoir plus, voir [Procédure : vendre des produits](sales-how-sell-products.md).
3.  Sous le raccourci **Lignes**, renseignez la ligne vente. Dans le champ **Procédure achat**, sélectionnez une procédure achat dont le champ **Commande spéciale** est sélectionné.

    Vous devez maintenant créer un bon de commande à partir d'une feuille de réquisition.  
4. Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Feuille de réquisition**, puis sélectionnez le lien associé.  
5. Choisissez l'action **Commande spéciale**, puis choisissez l'action **Extraire documents de vente**.  
6.  Dans la fenêtre **Extraire documents de vente**, affichez les résultats dans lesquels le **N° document** correspond au numéro de document de vente. Cliquez sur le bouton **OK**. Une ligne de feuille de réquisition est créée pour l'article.  
7.  Dans la ligne demande achat, sélectionnez **Nouveau** dans le champ **Message d'action**.  
8.  Dans la fenêtre **Demande achat**, sélectionnez l'action **Traiter messages d'action**. La fenêtre **Traiter messages d'action - Demande** s'affiche. Cliquez sur le bouton **OK**.  

    Le message qui s'affiche indique que les commandes achat ont été créées. Cliquez sur le bouton **OK**.  

Un bon de commande créé comme commande spécial pour un document de vente est respecté par le système de planification lorsqu'il équilibre l'offre et la demande. Ainsi, le bon de commande (approvisionnement) reste lié au document de vente (demande), même si ce bon de commande pourrait approvisionner une autre demande antérieure. Pour plus d'informations, voir [Détails de conception : méthodes de réapprovisionnement](design-details-reservation-order-tracking-and-action-messaging.md).  

> [!NOTE]  
>  Vous ne pouvez pas utiliser la fonctionnalité de commande spéciale si l'élément est déjà réservé. Par conséquent, pour les articles qui sont vendus en commandes spéciales, assurez\-vous que le champ **Réserver** sur la fiche article n'est pas défini sur **Toujours**.  

## <a name="see-also"></a>Voir aussi  
[Procédure : utiliser des articles non stockés](inventory-how-work-nonstock-items.md)  
[Ventes](sales-manage-sales.md)  
[Procédure : effectuer des livraisons directes](sales-how-drop-shipment.md)   
[Détails de conception : méthodes de réapprovisionnement](design-details-reservation-order-tracking-and-action-messaging.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

