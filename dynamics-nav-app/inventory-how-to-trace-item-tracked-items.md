---
title: "Procédure : tracer des articles suivis"
description: "Vous pouvez voir où un article suivi a été utilisé, y compris le mode et le moment de réception ou de production, de transfert, de vente, de consommation ou de retour. Vous pouvez également rechercher toutes les instances d'informations d'un numéro de série ou de lot particulier dans la base de données. Vous procédez à l'aide des fonctionnalités Traçabilité et Naviguer."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 6d25a7b60f8b1b37ef9de34d5ffc098a89828ea8
ms.contentlocale: fr-ca
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-trace-item-tracked-items"></a>Procédure : tracer des articles suivis
Vous pouvez voir où un article suivi a été utilisé, y compris le mode et le moment de réception ou de production, de transfert, de vente, de consommation ou de retour. Vous pouvez également rechercher toutes les instances d'informations d'un numéro de série ou de lot particulier dans la base de données. Vous procédez à l'aide des fonctionnalités Traçabilité et Naviguer.  

 Ces fonctions sont particulièrement utiles pour le contrôle qualité, lorsque vous devez déterminer quels clients ont reçu des produits correspondant à un numéro de lot particulier ou le lot dont provenait une composante défectueuse.  

 Dans la fenêtre **Traçabilité**, vous pouvez effectuer une traçabilité en aval et en amont dans une série de transactions d'inventaire reportées pour le numéro de lot ou de série.  

 Dans la fenêtre **Naviguer**, vous ne pouvez pas voir la séquence de transactions, mais vous pouvez afficher tous les enregistrements des numéros de série ou de lot, à la fois les écritures reportées et les enregistrements ouverts.  

 Les deux fonctions peuvent être utilisées en association en transférant un numéro de série ou de lot suivi dans la fenêtre **Naviguer** pour terminer un scénario complet de suivi. Pour plus d'informations, voir [Procédure pas à pas : suivi des numéros de série et des numéros de lot](walkthrough-tracing-serial-lot-numbers.md).  

## <a name="to-trace-item-tracked-items"></a>Pour tracer des articles suivis  

1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Repérage d'article**, puis sélectionnez le lien associé.  
2.  Dans les champs de filtre dans le haut de la fenêtre, entrez les numéros d'article spécifiques ou un filtre pour les numéros d'article que vous voulez suivre.  
3.  Dans le champ **Afficher composantes**, indiquez si vous voulez également voir d'où provenaient les composantes des articles. Les options disponibles dans ce champ sont les suivantes.  

    |Champ|Description|  
    |----------------------------------|---------------------------------------|  
    |**Non**|Sélectionnez cette option si vous ne voulez voir aucune composante.|  
    |**Avec traçabilité uniquement**|Sélectionnez cette option si vous ne voulez voir que les composantes ayant des numéros de lot ou de série.|  
    |**Tout**|Sélectionnez cette option si vous voulez voir toutes les composantes.|  

4.  Dans le champ **Méthode de suivi**, sélectionnez la méthode que vous voulez utiliser pour suivre l'article. Les options sont les suivantes  

    |Champ|Description|  
    |----------------------------------|---------------------------------------|  
    |**Utilisation->origine**|Cette méthode suit l'article à partir de l'endroit où il a été utilisé jusqu'à l'endroit d'où il vient. Par exemple, si un article fabriqué a été vendu à un client, la fenêtre **Traçabilité** présente ce dernier en montrant d'abord la ligne livraison vente, que vous pouvez développer pour voir le bon de production dont il provenait.|  
    |**Origine->utilisation**|Cette méthode suit l'article à partir de l'endroit dont il provient dans l'inventaire jusqu'à l'endroit où il a été utilisé. Par exemple, si un article fabriqué a été vendu à un client, la fenêtre **Traçabilité** présente ce dernier en montrant d'abord le bon de production terminé, que vous pouvez développer pour voir les lignes livraison vente où l'article a été utilisé.|  

5.  Sélectionnez l'action **Suivi** pour exécuter le suivi.  

> [!NOTE]  
>  Si vous avez reçu le même lot sur plusieurs transactions, la fenêtre **Traçabilité** peut ne pas afficher toutes les transactions. Seules les transactions affectées sont affichées.  

> [!NOTE]  
>  Si l'historique d'une transaction supplémentaire dans une ligne traçabilité a déjà été suivi par une autre ligne au-dessus de celle-ci, la case à cocher **Déjà tracé** est activée. Pour une vue plus simple, ces lignes sous-jacentes ne s'affichent pas.  
>   
>  Pour trouver les lignes traçabilité où l'historique des transactions a déjà été suivi, cliquez sur le bouton **Aller sur déjà tracé**. La ligne traçabilité en question est sélectionnée et toutes les lignes sous-jacentes sont développées.  

## <a name="to-find-item-tracked-items-with-navigate"></a>Pour rechercher des articles suivis avec Naviguer  

1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Naviguer**, puis sélectionnez le lien associé.  
2.  Sur le raccourci **Traçabilité**, dans les champs **N° de série** et **N° lot**, entrez les numéros traçabilité que vous voulez suivre.  
3.  Sélectionnez l'action **Rechercher** pour rechercher toutes les instances du numéro de série ou de lot dans la base de données.  

## <a name="see-also"></a>Voir aussi  
[Stock](inventory-manage-inventory.md)  
[Détails de conception : traçabilité](design-details-item-tracking.md)
[Détails de conception : traçabilité et réservations](design-details-item-tracking-and-reservations.md)  
[Procédure : réserver des articles](inventory-how-to-reserve-items.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
[Procédure pas à pas : suivi des numéros de série et des numéros de lot](walkthrough-tracing-serial-lot-numbers.md)

