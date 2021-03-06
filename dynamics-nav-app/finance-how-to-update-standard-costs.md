---
title: "Procédure : mise à jour des coûts standard"
description: "Vous devez régulièrement mettre à jour les coûts standard des composants et remonter les nouveaux coûts dans l'article parent."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/09/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: dd2bb16af611be7f7720fdf07eb65fd268aba039
ms.contentlocale: fr-ca
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-update-standard-costs"></a>Procédure : mise à jour des coûts standard
Vous devez régulièrement mettre à jour les coûts standard des composants et remonter les nouveaux coûts dans l'article parent. Le processus comprend généralement les quatre étapes suivantes :  

1.  Mettre à jour les coûts aux niveaux des composantes et de la capacité. Pour plus d'informations, voir le traitement en lot **Suggérer un coût standard d'article**.  
2.  La consolidation et le calcul multi-niveau des coûts des composantes et de capacité permettent de déterminer le coût total de fabrication ou d'assemblage des articles.  
3.  Appliquer les coûts standard entrés lorsque vous lancez les traitements par lots précédents. Les coûts standard n'entrent en vigueur que lorsqu'ils sont mis en œuvre. Pour plus d'informations, voir Appliquer nouv. coût standard.  
4.  Appliquer les modifications pour mettre à jour le champ **Coût unitaire** de la fiche article et effectuer une réévaluation du stock. Pour plus d'informations, voir [Procédure : réévaluer le stock](inventory-how-revalue-inventory.md).  

Pour plus d'informations, voir [À propos du calcul des coûts standard](finance-about-calculating-standard-cost.md) .  
## <a name="to-update-standard-costs"></a>Pour mettre à jour des coûts standard  
1.  Exécutez le traitement en lot **Ajuster coûts - Écr. article**.  
2.  Exécutez le traitement en lot **Reporter le coût de l'inventaire au grand livre**.  
3.  Ouvrez la **Feuille coût standard** et utilisez une ou plusieurs des fonctions suivantes :  

    1.  Exécutez le traitement en lot **Suggérer un coût standard d'article**.  
    2.  Vérifiez les résultats et apportez des modifications si nécessaire.  
    3.  Exécutez le traitement en lot **Suggérer le coût standard de la capacité**.  
    4.  Vérifiez les résultats et apportez des modifications si nécessaire.
    5. Exécutez le traitement en lot **Cumuler le coût standard**.
    6.  Vérifiez les résultats et apportez des modifications si nécessaire.
    7.  Exécutez le traitement en lot **Appliquer les modifications de coût standard**.  
4.  Vérifiez et reportez la fenêtre **Journal réévaluation** renseignée avec les entrées des étapes précédentes de ce processus.  

## <a name="see-also"></a>Voir aussi  
 [À propos du calcul des coûts standard](finance-about-calculating-standard-cost.md)   
 [Gestion des coûts ajustés](finance-manage-inventory-costs.md)   
 [Détails de conception : modes évaluation stock](design-details-costing-methods.md) [[Finance](finance.md)  
 [Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

