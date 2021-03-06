---
title: "Comment prélever pour des opérations internes dans les configurations de stockage avancées"
description: "Dans les configurations d'entrepôt avancées, dans lesquelles l'emplacement est configuré pour utiliser le prélèvement ainsi que la livraison, vous pouvez prélever des composantes pour les activités de production et d'assemblage à l'aide de la fenêtre **Prélèvement entrepôt**."
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
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 08b79f573a9fc013068f7e1f5dd593a596a579a3
ms.contentlocale: fr-ca
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-pick-for-assembly-or-production-in-advanced-warehouse-configurations"></a>Procédure : prélever pour l'assemblage ou la fabrication dans les configurations de stockage avancées.
Dans les configurations d'entrepôt avancées, dans lesquelles l'emplacement est configuré pour utiliser le prélèvement ainsi que la livraison, vous pouvez prélever des composantes pour les activités de production et d'assemblage à l'aide de la fenêtre **Prélèvement entrepôt**.  

Vous pouvez également utiliser la fenêtre **Feuille mouvement** pour déplacer des articles entre emplacements ad hoc, c'est-à-dire sans référence à un document origine. Pour plus d'informations, voir [Procédure : déplacer des articles dans les configurations de stockage avancées](warehouse-how-to-move-items-in-advanced-warehousing.md).  

Pour plus d'informations sur le prélèvement d'articles pour des opérations internes dans les emplacements entrepôts de base qui sont configurés uniquement pour le prélèvement, reportez-vous à la [Procédure : déplacer les composantes vers une zone opérations dans les configurations d'entrepôt de base](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md).  

Vous ne pouvez pas créer de toutes pièces un document prélèvement entrepôt car une activité de prélèvement fait toujours partie d'un flux de travail, soit dans un scénario d'extraction, soit dans un scénario de déplacement.  

Vous pouvez créer le document prélèvement entrepôt par déplacement en sélectionnant **Créer prélèvement ent.** dans le document origine, par exemple, un ordre d'assemblage ou une expédition entrepôt lancé. Pour plus d'informations, voir [Procédure : prélever des articles avec les prélèvements entrepôt](warehouse-how-to-pick-items-for-warehouse-shipment.md).  

Sinon, vous pouvez créer le document prélèvement entrepôt par extraction à l'aide de la fenêtre **Feuille prélèvement** pour détecter les demandes de prélèvement, à la fois pour l'expédition et les opérations internes, puis créer les documents prélèvement entrepôt requis.  

La procédure suivante explique un scénario d'extraction dans lequel vous prélevez des composants d'un ordre de fabrication lancé via la fenêtre **Feuille prélèvement**. Cette procédure s'applique également pour un ordre d'assemblage.  

Pour créer des demandes de prélèvement dans le cadre de scénarios d'extraction et de déplacement, il faut que les documents origine en question soient libérés. Libérez les documents origine des opérations internes en procédant comme suit.  

|Document origine|Méthode de libération|  
|---------------------|--------------------|  
|Bon de production|Remplacez le type commande par un bon de production libéré.|  
|Ordre d'assemblage|Remplacez l'état actuel par l'état Libéré.|  

## <a name="to-pick-components-using-the-pick-worksheet"></a>Pour prélever des composants à partir des feuilles prélèvement  
1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Feuille prélèvement**, puis sélectionnez le lien associé.  
2.  Choisissez l'action **Extraire documents entrepôt**, puis sélectionnez les lignes composante du bon de production libéré.  
3.  Vérifiez les lignes, triez-les pour assurer un prélèvement optimisé et, si nécessaire, combinez les avec d'autres lignes de la feuille pour utiliser au mieux la disponibilité de l'employé.  
4.  Choisissez l'action **Créer prélèvement**.  
5.  Définissez le mode de création des documents prélèvement entrepôt et la manière de trier les lignes prélèvement en renseignant les champs de la fenêtre **Créer prélèvement** .  
6.  Cliquez sur le bouton **OK**. Les documents prélèvement entrepôt sont créés avec des lignes prélèvement pour chaque composante requise dans l'opération interne.  

Si la zone Opérations internes (par exemple, un atelier de production) est configurée avec une zone par défaut pour les composantes à utiliser dans l'opération, ce code de zone est inséré dans les lignes Emplacement qui figurent sur le document prélèvement entrepôt pour indiquer aux magasiniers où placer les articles. Pour plus d'informations, voir le champ **Code e zone avant production** ou **Code de zone vers assemblage**.

## <a name="filling-the-consumption-bin"></a>Renseignement de la zone consommation
Ce graphique indique comment le champ **Code de zone** sur les lignes composante bon de production est renseigné en fonction de la configuration de votre emplacement.

![Organigramme Flux d'emplacement](media/binflow.png "BinFlow")  

## <a name="see-also"></a>Voir aussi
[Gestion d'entrepôt](warehouse-manage-warehouse.md)  
[Stock](inventory-manage-inventory.md)  
[Configuration de la gestion des entrepôts](warehouse-setup-warehouse.md)     
[Gestion d'assemblage](assembly-assemble-items.md)    
[Détails de conception : gestion d'entrepôt](design-details-warehouse-management.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

