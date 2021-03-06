---
title: "Procédure : vendre des articles en inventaire dans des flux à assembler pour commande"
description: "Si l'article est configuré pour la fiche d'assemblage pour commande, le processus par défaut de document de vente considère que l'article n'est pas en inventaire et doit être assemblé pour ce document de vente spécifique. Par conséquent, un ordre d'assemblage lié est automatiquement créé lorsque vous ajoutez l'article à une ligne document de vente."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 0d907c5f96c4af0e28a04292bee2c21865346593
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-sell-inventory-items-in-assemble-to-order-flows"></a>Procédure : vendre des articles en inventaire dans des flux à assembler pour commande
Si le champ **Politique d'assemblage** de la fiche article d'un élément d'assemblage indique **Assembler pour commande**, le processus par défaut de document de vente considère que l'article n'est pas en inventaire et doit être assemblé pour ce document de vente spécifique. Par conséquent, un ordre d'assemblage lié est automatiquement créé lorsque vous ajoutez l'article à une ligne document de vente. Pour plus d'informations sur le paramétrage des éléments d'assemblage, voir [Procédure : Vente d'articles à assembler pour commande](assembly-how-to-sell-items-assembled-to-order.md). Toutefois, si une partie de la quantité sur commande vente est déjà disponible en stock, alors vous pouvez diminuer la quantité d'ordre d'assemblage en changeant le champ **Quantité à assembler pour commande** de la ligne commande vente.  

Ce scénario est rare parce que les articles à assembler pour commande sont toujours censés être personnalisés, et il est peu probable qu'ils soient en inventaire dans la configuration qui est demandée par un autre client. Néanmoins, si une compagnie a des quantités assembler pour commande en inventaire à cause de retours ou d'annulations de commande, ces quantités doivent être prélevées et vendues avant que de nouvelles soient assemblées.  

> [!NOTE]  
>  Aucune fonctionnalité n'existe sur les commandes vente qui vous alerte automatiquement ou vous aide à déduire les quantités d'ordre d'assemblage qui sont déjà disponibles. Au lieu de cela, vous devez contrôler les informations de disponibilité, par exemple dans le récapitulatif **Détails ligne vente**.  

Une fonctionnalité similaire est disponible lorsque vous vendez des éléments d'assemblage de l'inventaire et qu'une partie ou l'ensemble de la quantité n'est pas disponible et peut être fournie dans un ordre d'assemblage. Pour plus d’informations, reportez-vous à la section [Procédure : vendre simultanément des articles à assembler pour commande et des articles en inventaire](assembly-how-to-sell-assemble-to-order-items-and-inventory-items-together.md).  

> [!NOTE]  
>  Certaines règles s'appliquent au champ **Qté à livrer** sur les lignes document de vente qui contiennent une combinaison de quantités assembler pour commande et de quantités inventaire. Pour plus d'informations, voir la section Scénarios de combinaison dans [Description des processus Assembler pour commande et Assembler pour stock](assembly-assemble-to-order-or-assemble-to-stock.md).  

Dans cette procédure, vous remplacez les quantités à assembler pour commande par les quantités en inventaire sur une ligne document de vente. Les étapes comprennent la vérification des disponibilités existantes, la détection de la quantité de l'ordre d'assemblage associé, puis la réservation de la quantité en inventaire pour s'assurer qu'elle est prélevée et livrée pour la commande.  

## <a name="to-sell-inventory-items-in-assemble-to-order-flows"></a>Vendre des articles en inventaire dans des flux assembler pour commande  
1.  Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Commandes vente**, puis sélectionnez le lien connexe.  
2.  Créez un document de vente. Pour en savoir plus, voir [Procédure : vendre des produits](sales-how-sell-products.md).  
3.  Sur une ligne document de vente pour un article à assembler pour commande, dans le champ **Quantité**, entrez la quantité demandée.  
4.  Dans le récapitulatif **Détails ligne vente**, déterminez si une partie ou la totalité de la quantité demandée est disponible.  
5.  Dans le champ **Quantité à assembler pour commande**, déduisez la quantité disponible de manière à ce que seule la quantité indisponible soit assemblée à la commande. Le champ **Quantité réservée** est diminué en conséquence pour refléter que la relation ordre pour ordre, ou la réservation, s'applique uniquement à la quantité à assembler.  
6.  Sur le raccourci **Lignes**, choisissez **Fonctions**, puis choisissez l'action **Réserver**.  
7.  Dans la fenêtre **Réservation**, sélectionnez la ou les lignes d'écriture article qui contiennent les quantités disponibles, sélectionnez **Réserver à partir de la ligne courante**, puis sélectionnez le bouton **OK**.  

    Dans la fenêtre **Commande vente**, le champ **Quantité réservée** indique maintenant que l'ensemble de la quantité ligne commande est réservé. Le champ **Quantité à assembler pour commande** indique toujours la sous-quantité qui doit être assemblée.  

8.  Libérez le document de vente pour prélever les articles en inventaire et assembler les articles indisponibles. Pour plus d'informations, voir [Procédure : assembler des articles](assembly-how-to-assemble-items.md).  

> [!CAUTION]  
>  Le champ **Code de zone** du document de vente peut être prérempli en fonction du champ **Code zone livr. ass. pr comm.** ou du champ **Code zone depuis assemblage** de la fiche emplacement. Dans ce cas, le champ **Code de zone** de la ligne document de vente peut être incorrect dans cette combinaison de quantités assembler pour commande et assembler pour stock. Il est judicieux de consulter le champ **Code emplacement** et de s'assurer que le placement fonctionne pour toutes les quantités. Sinon, entrez les deux quantités différentes sur des lignes document de vente distinctes.  

## <a name="see-also"></a>Voir aussi  
[Gestion d'assemblage](assembly-assemble-items.md)  
[Procédure : réserver des articles](inventory-how-to-reserve-items.md)  
[Procédure : utiliser les nomenclatures](inventory-how-work-BOMs.md)  
[Stocks](inventory-manage-inventory.md)  
[Détails de conception : gestion d'entrepôt](design-details-warehouse-management.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

