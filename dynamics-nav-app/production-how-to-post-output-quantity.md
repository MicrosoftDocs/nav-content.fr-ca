---
title: "Procédure : exécuter en lot la sortie de production et les temps d'exécution"
description: "La quantité produite représente l'avancée des travaux en prenant en compte la quantité achevée."
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
ms.openlocfilehash: 266c3f52dda22133acebf6052326ab57551b2ec0
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-batch-post-output-and-run-times"></a>Procédure : exécuter en lot la sortie et les temps d'exécution
La quantité produite représente l'avancée des travaux en prenant en compte la quantité achevée.  

> [!NOTE]
> L'inventaire est automatiquement mis à jour uniquement lorsque vous reportez la quantité sortie durant la dernière opération.  

## <a name="to-post-output-quantities-for-one-or-more-production-order-lines"></a>Pour reporter les quantités sorties pour une ou plusieurs lignes bon de production
1. Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Journal de sortie**, puis sélectionnez le lien associé.  
2. Renseignez les champs en indiquant les données relatives à la fabrication et à la production. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Si l'opération est achevée, sélectionnez le champ **Terminé**.  

    Si l'emplacement entrepôt dans lequel les articles doivent être rangés utilise des zones mais n'exige pas le traitement des rangements, affectez un code de zone à la ligne journal pour indiquer l'endroit où les articles doivent être placés dans l'entrepôt. Pour plus d'informations, voir [Procédure : rangement du résultat de fabrication ou d'assemblage](warehouse-how-to-put-away-production-output.md).  

4. Choisissez l'action **Reporter** pour reporter les opérations. La quantité produite est reportée. L'article peut être livré.  

## <a name="to-post-run-times-for-one-or-more-production-order-lines"></a>Pour reporter les temps d'exécution pour une ou plusieurs lignes bon de production
Le temps d'exécution représente l'avancement des travaux en prenant en compte le temps de travail nécessaire.    

1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Journal de sortie**, puis sélectionnez le lien associé.  
2. Renseignez les champs en indiquant les données relatives à la fabrication et à la production.  
3.  Si l'opération est achevée, sélectionnez le champ **Terminé**.  
4. Choisissez l'action **Reporter** pour reporter le temps passé par opération. Les écritures du grand livre de capacité sont mises à jour pour les unités de production ou les ateliers utilisés.

## <a name="see-also"></a>Voir aussi  
[Production](production-manage-manufacturing.md)    
[Paramétrage de la production](production-configure-production-processes.md)  
[Planification](production-planning.md)      
[Stock](inventory-manage-inventory.md)  
[Procédure d'achat](purchasing-manage-purchasing.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

