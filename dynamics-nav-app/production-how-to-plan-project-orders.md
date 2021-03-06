---
title: "Procédure : planifier les O.F. projets"
description: "Cette tâche de planification est lancée à partir d'un document de vente et utilise la fenêtre **Planification document de vente**. Une fois que vous avez créé un bon de production projet, vous pouvez le planifier davantage à l'aide de la fenêtre **Planification de commande**."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: a03cdaf16b25cbcf030e9a33c538ea3df96a1fe9
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-plan-project-orders"></a>Procédure : planifier les projets de commandes
Cette tâche de planification est lancée à partir d'une commande vente et utilise la fenêtre **Planification commande vente**. Une fois que vous avez créé un O.F. projet, vous pouvez le planifier davantage à l'aide de la fenêtre **Planning commande**.  

## <a name="to-create-a-project-production-order"></a>Pour créer un bon de production projet  

1.  Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Commandes vente**, puis sélectionnez le lien connexe.  
2.  Sélectionnez le document de vente qui représente le projet de production, puis choisissez l'action **Planification**.  
4.  Dans la fenêtre **Planification document de vente**, choisissez l'action **Créer bon de prod.**.  
5.  Dans la fenêtre **Créer commande à partir des ventes**, dans le champ **Type O.F.**, sélectionnez **O.F. projet**.  
6.  Cliquez sur le bouton **Oui**.  
7.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Bons de production**, puis sélectionnez le lien associé.
8. Ouvrez le bon de production que vous venez de créer.  

    Notez que le champ **Type origine** de l'ordre de fabrication indique **En-tête vente** et l'ordre comporte plusieurs lignes, une pour chaque article de la ligne vente à produire.  
9. Sélectionnez l'action **Planification**.
10. Dans la fenêtre **Planification de commande**, choisissez l'action **Actualiser** pour calculer la nouvelle demande.  

La ligne d'en-tête de commande de la commande projet s'affiche avec toutes les lignes de demandes non satisfaites développées en-dessous. Bien que l'ordre de fabrication contienne les lignes de plusieurs articles produits, la demande totale pour toutes les lignes d'O.F. est répertoriée sous une ligne d'en-tête de commande dans la fenêtre **Planning commande** et le nom du client d'origine s'affiche. Vous pouvez maintenant passer à la planification de la demande en vous reportant à la [Procédure : planifier de nouvelles demandes commande par commande](production-how-to-plan-for-new-demand.md).  

> [!NOTE]  
>  Les lignes de demandes de l'ordre de fabrication projet qui ont **Ordre de fabrication** dans leur champ **Système réappro.** représentent des ordres de fabrication sous-jacents. Après avoir généré ces ordres de fabrication, vous devez à nouveau calculer un planning dans la fenêtre **Planning ordre** pour identifier toute demande de composant non réalisée pour ceux-ci. Cela signifie que le lien projet n'est plus visible dans la fenêtre. Cependant, si vous utilisez la fonctionnalité Suivi de commande, alors vous pouvez passer en revue les commandes approvisionnement effectuées sous le document de vente d'origine.  

## <a name="see-also"></a>Voir aussi
[Planification](production-planning.md)   
[Paramétrage de la production](production-configure-production-processes.md)  
[Production](production-manage-manufacturing.md)    
[Stock](inventory-manage-inventory.md)  
[Procédure d'achat](purchasing-manage-purchasing.md)  
[Détails de conception : planification de l'approvisionnement](design-details-supply-planning.md)   
[Configurer des recommandations : planification de l'approvisionnement](setup-best-practices-supply-planning.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

