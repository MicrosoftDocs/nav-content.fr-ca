---
title: "Procédure : rangement de la production"
description: "Le mode de rangement de la production dépend du mode de configuration de l'entrepôt en tant qu'emplacement."
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
ms.openlocfilehash: 1e553752c9479ccb6b8528f47c2b63b410591c3c
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-put-away-production-or-assembly-output"></a>Procédure : rangement du résultat de fabrication ou d'assemblage
Le mode de rangement de la production dépend du mode de configuration de l'entrepôt en tant qu'emplacement. Pour plus d'informations, voir [Configuration de la gestion des entrepôts](warehouse-setup-warehouse.md).  

Dans les configurations entrepôt de base où l'emplacement exige un traitement des rangements mais pas un traitement des réceptions, vous pouvez utiliser le document **Rangement inventaire** pour organiser et enregistrer le rangement de la production.  

Dans les configurations de stockage avancées où l'emplacement nécessite un traitement à la fois de rangement et de réception, vous pouvez créer soit un document rangement interne soit un document mouvement pour ranger la production.  

La première étape dans la création d'un rangement de production consiste à créer la demande enlogement entrante. Cette demande indique à l'entrepôt que la production de l'O.F ou de l'assemblage est prête à être rangée.

## <a name="to-create-the-inbound-warehouse-request"></a>Pour créer la demande d'enlogement  
1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Ordre de production libéré**, puis sélectionnez le lien associé.  
2.  Sur l’ordre de fabrication qui est prêt pour rangement, choisissez l'action **Créer demande d’enlogement**.  

> [!NOTE]  
>  Vous pouvez également créer la demande enlogement entrepôt en sélectionnant le champ **Créer demande d'enlogement** lors de l'actualisation de l'ordre de fabrication. Pour plus d'informations, voir [Procédure : actualiser ou replanifier des ordres de fabrication](production-how-to-replan-refresh-production-orders.md).  

## <a name="to-put-output-away-with-an-inventory-put-away"></a>Pour ranger la production avec un rangement inventaire  
1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Rangement inventaire**, puis sélectionnez le lien associé.  
2.  Créez un rangement inventaire. Pour plus d'informations, voir [Procédure : ranger des articles avec le rangement stock](warehouse-how-to-put-items-away-with-inventory-put-aways.md)
3.  Pour accéder aux composantes du bon de production, choisissez l'action **Extraire documents sources**, puis sélectionnez le bon de production libéré.  
4.  Renseignez les lignes rangement en fonction des besoins.
5.  Lorsque les lignes sont prêtes à être reportées, choisissez l'action **Reporter**. Les écritures entrepôt nécessaires sont alors créées et la production des articles est reportée.  

Vous pouvez également créer un **rangement inventaire** directement à partir du bon de production libéré. Pour plus d'informations, voir [Procédure : ranger des articles avec le rangement stock](warehouse-how-to-put-items-away-with-inventory-put-aways.md)  

Lorsque vous reportez un rangement inventaire, on suppose que toutes les opérations sont reportées en fonction de l'itinéraire standard, à savoir que la quantité produite est reportée en fonction de la dernière opération. Vous pouvez utiliser le journal de sortie pour reporter les écarts de quantité produite et les temps d'exécution et de préparation. S'il est nécessaire d'effectuer un report partiel après la création d'un rangement inventaire, vous pouvez le faire au niveau des temps de préparation et des quantités pour toutes les opérations, à l'exception de la dernière. Dans ce cas, la dernière opération est contrôlée par le rangement inventaire.  

Si vous devez juste reporter le temps d'exécution ou de préparation de la dernière opération, définissez la quantité produite de la dernière opération sur 0. Vous pouvez également choisir de ne pas reporter la dernière ligne simplement en la supprimant  

## <a name="to-put-output-away-with-a-warehouse-internal-put-away"></a>Pour ranger la production dans le cadre d'un rangement interne ou d'un mouvement
1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Rangement interne entrep.**, puis sélectionnez le lien associé.  
2. Sélectionnez l'action **Nouveau**.
3. Renseignez l'en-tête d'un nouveau rangement interne en y indiquant au moins le **code d'emplacement**.  
4. Renseignez une ligne pour chaque article à déplacer vers l'entrepôt. Vous ne devez renseigner que les champs **N° article** et **Quantité**.  

    > [!NOTE]  
    >  Lorsque vous sélectionnez le champ **N° article**, la **liste des contenus de la zone** s'ouvre à la place de la **liste des articles**. En effet, vous souhaitez ranger un article qui se trouve dans une zone en particulier (contenu de la zone et pas uniquement un article) et vous connaissez déjà la zone dans laquelle l'article doit être prélevé.  

4.  Pour compléter les lignes feuille en y indiquant l'ensemble du contenu de la zone ou le contenu de la zone filtré des zones de cet emplacement, choisissez l'action **Extraire contenu de la zone**.  
5.  Choisissez l'action **Créer rangement**, et les articles que vous souhaitez sortir de l'unité de production figurent maintenant sur des instructions de rangement et attendent d'être stockés dans l'entrepôt.  

> [!NOTE]  
>  Lorsque l'emplacement entrepôt est configuré pour utiliser un prélèvement et un rangement suggérés, l'entrepôt est relié au centre de production via les zones de production par défaut : les zones enlogement et désenlogement et la zone d'atelier ouvert que vous pouvez définir sur le raccourci **Zones** de la fiche emplacement. Lorsque vous validez la production d'un O.F.,la production est placée automatiquement dans l' **emplacement désenlogement**. Suivez la procédure décrite ci-dessus pour ranger la production, mais au lieu d'utiliser la zone par défaut de l'article, vous devez déplacer ou ranger les articles de la **zone désenlogement** dans la zone par défaut de l'article.  

## <a name="to-manually-specify-a-bin-to-store-items-from-production-output"></a>Pour spécifier manuellement une zone devant stocker des articles issus de la production  
1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Feuille mouvement**, puis sélectionnez le lien associé.  
2.  Renseignez l'en-tête et créez une ligne pour chaque article à déplacer vers l'entrepôt.  
3.  Renseignez les champs **Du code emplacement** et **Du code emplacement**, puis entrez la quantité dans le champ **Quantité**.  
4.  Pour compléter les lignes feuille en y indiquant l'ensemble du contenu de la zone ou le contenu de la zone filtré des zones de cet emplacement, choisissez l'action **Extraire contenu de la zone**.  
5. Choisissez l'action **Créer mouvement**. Des instruction de mouvement entrepôt sont créées contenant des lignes Prélever et Emplacement s'adressant aux magasiniers.  

> [!NOTE]  
>  Vous ne pouvez pas saisir le numéro document origine, tel que le N° O.F., rangement interne, rangement ou documents de mouvement pour l'une ou l'autre de ces procédures.  

## <a name="see-also"></a>Voir aussi  
[Gestion d'entrepôt](warehouse-manage-warehouse.md)  
[Stock](inventory-manage-inventory.md)  
[Configuration de la gestion des entrepôts](warehouse-setup-warehouse.md)     
[Gestion d'assemblage](assembly-assemble-items.md)    
[Détails de conception : gestion d'entrepôt](design-details-warehouse-management.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

