---
title: "Procédure : déplacer des articles dans les configurations de stockage avancées"
description: "Dans des configurations d'entrepôt avancées, c'est-à-dire des emplacements avec prélèvement et rangement suggérés, des mouvements entrepôt entre zones sont exécutés par un cadre qui prépare des mouvements entrepôt dans la feuille mouvement, puis crée les mouvements entrepôt que les employés d'entrepôt doivent exécuter."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/232017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: a7e26a8910b0cf7d8a78b7f86291d9cfd5d18bec
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-move-items-in-advanced-warehouse-configurations"></a>Procédure : déplacer des articles dans les configurations de stockage avancées
Dans des configurations d'entrepôt avancées, c'est-à-dire des emplacements avec prélèvement et rangement suggérés, des mouvements entrepôt entre zones sont exécutés par un cadre qui prépare des mouvements entrepôt dans la feuille mouvement, puis crée les mouvements entrepôt que les employés d'entrepôt doivent exécuter.  

## <a name="to-move-items-with-the-warehouse-movement-worksheet"></a>Pour déplacer des articles avec la feuille mouvement entrepôt
La fenêtre **Feuille mouvement** a deux fonctions qui peuvent vous aider à renseigner automatiquement les lignes. La première est la fonction **Calculer réappro. emplacement**. Cette fonction utilise les classements de zone pour suggérer le réapprovisionnement des zones les mieux classées à partir de celles moins bien classées. La seconde est la fonction de **Extraire contenu de la zone**, qui renseigne les lignes feuille avec tout le contenu de ou des zones que vous spécifiez.

1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Feuille mouvement**, puis sélectionnez le lien associé.  
2.  Renseignez comme il convient les informations de mouvement d'entrepôt dans les lignes de la feuille.  
3. Choisissez l'action **Créer mouvement** pour créer un document mouvement entrepôt qui pourra être ensuite enregistré lorsque le mouvement sera terminé.  

### <a name="to-register-the-warehouse-movement"></a>Pour enregistrer le mouvement d'entrepôt  
1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Mouvements**, puis sélectionnez le lien associé.  
2.  Ouvrez le mouvement entrepôt que vous souhaitez traiter.  
3.  Sur les lignes dont le type d'action est **Emplacement**, spécifiez où, quoi et quand déplacer l'article concerné en modifiant les champs **Code zone**, **Code emplacement** ou **Qté à traiter**, ou **Date d'échéance** .  

    Si votre entrepôt a été configuré de façon à ce que les codes de zone suivent la structure physique de l'entrepôt, vous pouvez prendre des quantités de plusieurs articles dans des zones consécutives, puis les placer dans des zones de prélèvement se trouvant en aval et pouvant être proches les uns des autres.  
4.  Sur les lignes dont le type d'action est **Prélever**, indiquez dans le champ **Qté à traiter** une quantité du contenu emplacement que vous souhaitez déplacer. Tous les autres champs sur les lignes dont le type d'action est **Prélever** sont en lecture seule.  
5.  Pour déplacer toutes les quantités proposées comme spécifiées dans le champ **Quantité**, choisissez l'action **Remplir automatiquement la quantité à traiter**.  
6. Sélectionnez l'action **Enregistrer**.  

> [!NOTE]  
>  Si l'emplacement utilise les prélèvements et rangements suggérés, vous ne pouvez pas déplacer manuellement des articles vers ou depuis une zone de type RÉCEPTIONNER, car les articles dans ce type de zone doivent être enregistrés comme étant rangés avant de faire partie de l'inventaire disponible.

## <a name="to-register-the-movement-of-an-item-that-has-already-occurred"></a>Pour enregistrer un mouvement d'un article déjà terminé  
Si, en cas d'utilisation d'un prélèvement et d'un rangement suggérés dans l'emplacement, vous devez déplacer des articles vers d'autres zones sans rangement, prélèvement ou mouvement entrepôt préexistant, vous pouvez alors enregistrer l'emplacement exact des articles dans l'entrepôt à l'aide de la fonction **Journal reclassement entrepôt**.

1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Journal de reclassement d'entrepôt**, puis sélectionnez le lien associé.  
2.  Renseignez les champs **N° article**, **Du code zone**, **Du code emplacement**, **Vers code zone** et **Du code emplacement**.  
3.  Sélectionnez l'action **Enregistrer**.  

## <a name="see-also"></a>Voir aussi  
[Gestion d'entrepôt](warehouse-manage-warehouse.md)  
[Stock](inventory-manage-inventory.md)  
[Configuration de la gestion des entrepôts](warehouse-setup-warehouse.md)     
[Gestion d'assemblage](assembly-assemble-items.md)    
[Détails de conception : gestion d'entrepôt](design-details-warehouse-management.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

