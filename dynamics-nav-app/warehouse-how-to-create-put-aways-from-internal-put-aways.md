---
title: "Procédure : créer un rangement à partir du rangement interne"
description: "Une fois les articles rangés et avant qu'ils ne soient prélevés pour répondre aux besoins d'un bon de production ou d'une livraison, ils sont stockés dans l'entrepôt comme faisant partie de l'inventaire disponible."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 970b9b9046018b0dcea5b9996d10e19e444a7639
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-pick-and-put-away-without-a-source-document"></a>Procédure : Prélever et ranger sans document origine
Une fois les articles rangés et avant qu'ils ne soient prélevés pour répondre aux besoins d'un bon de production ou d'une livraison, ils sont stockés dans l'entrepôt comme faisant partie de l'inventaire disponible.  

Vous pouvez être amené à sortir temporairement des articles des emplacements prélèvement entrepôt, par exemple pour les présenter au cours d'une argumentation. Ces articles appartiennent toujours à la compagnie et font partie de l'inventaire ; par contre, ils ne peuvent pas être prélevés. Ils sont enregistrés dans une zone spécial que vous créez à cet effet ; techniquement, les articles se trouvent dans l'entrepôt, mais physiquement, ils peuvent se trouver dans une salle de conférences ou d'exposition.  

Il peut également arriver que l'unité de fabrication ait inopinément besoin de quelques pièces pour un processus. Vous pouvez prélever des articles pour les emplacements fabrication à l'aide du prélèvement interne. Une fois le processus terminé et la production réalisée, vous reportez la consommation des articles et videz la zone production, ce qui a pour effet de réduire la quantité de l'article dans votre emplacement.  

De même, des articles peuvent être retournés à l'entrepôt pour être rangés. Il est possible que les articles aient été prélevés dans l'inventaire disponible pour répondre à un bon de production, mais sans être utilisés du tout. Pour qu'ils fassent de nouveau partie de l'inventaire disponible, ils doivent faire l'objet d'un rangement dans la zone.  

Les **rangements internes** vous permettent d'effectuer des rangements sans avoir à vous référer à un document origine spécifique. Vous pouvez facilement configurer toutes les informations nécessaires pour créer une instruction entrepôt de rangement.  

> [!NOTE]  
>  Lorsque vous n'utilisez pas de prélèvements ni de rangements internes, vous pouvez effectuer ces ajustements en déplaçant les articles d'une zone vers une autre ou en reportant les ajustements des quantités d'une zone.  
>   
>  Lorsque l'emplacement utilise le prélèvement et le rangement suggérés et, par conséquent, utilise des types de zone, vous ne pouvez pas déplacer manuellement des articles vers ou depuis une zone de type RÉCEPTIONNER, car les articles dans ce type de zone doivent être enregistrés comme étant rangés avant de faire partie de l'inventaire disponible.  

## <a name="to-create-an-internal-pick"></a>Pour créer un prélèvement interne  
1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Prélèvement interne entrep.**, puis sélectionnez le lien associé.  
2.  Renseignez le champ **N°** et **Vers code emplacement** du raccourci **Général**. Le champ **Du code emplacement** indique l'emplacement où se trouvent les articles que vous souhaitez. Pour des raisons de production, cette zone représente la zone enlogement ou la zone d'atelier ouvert. Pour d'autres raisons, vous devez choisir un code de zone de destination d'un type de zone qui n'est pas utilisé pour le prélèvement (par exemple, une zone d'échelonnement, de livraison ou une zone spéciale).  
3.  Sélectionnez un article dans le champ **N° article**, puis renseignez les quantités à prélever.  
4. Choisissez l'action **Créer prélèvement**. Une instruction prélèvement entrepôt est maintenant créée pour un magasinier.  

## <a name="to-create-an-internal-put-away"></a>Pour créer un rangement interne  
1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Rangement interne entrep.**, puis sélectionnez le lien associé.  
2.  Renseignez le champ **N°** et **Du code emplacement** du raccourci **Général**. Le champ **Du code emplacement** indique l'emplacement où se trouvent les articles retournés à l'entrepôt (par l'unité de production, par exemple).  
3.  Renseignez les numéros article et les quantités sur les lignes.  
4.  Choisissez l'action **Créer rangement**. Une instruction rangement entrepôt est maintenant créée pour un employé d'entrepôt.  

## <a name="see-also"></a>Voir aussi  
[Gestion d'entrepôt](warehouse-manage-warehouse.md)  
[Stock](inventory-manage-inventory.md)  
[Configuration de la gestion des entrepôts](warehouse-setup-warehouse.md)     
[Gestion d'assemblage](assembly-assemble-items.md)    
[Détails de conception : gestion d'entrepôt](design-details-warehouse-management.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

