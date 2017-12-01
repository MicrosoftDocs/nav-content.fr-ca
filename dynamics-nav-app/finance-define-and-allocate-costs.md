---
title: "Définition et répartition des coûts"
description: "Les affectations de coûts déplacent les coûts et les revenus entre les types de coûts, les centres de coûts et les coûts associés. Vous pouvez définir autant d'affectations que nécessaire."
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
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: f7c34e8f4c57e2effc03b8dcd2a722d7bdbb4692
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="defining-and-allocating-costs"></a>Définition et répartition des coûts
Les affectations de coûts déplacent les coûts et les revenus entre les types de coûts, les centres de coûts et les coûts associés. Vous pouvez définir autant d'affectations que nécessaire. Chaque affectation comporte les éléments suivants :  

-   Une source affectation.  
-   Une ou plusieurs cibles d'affectation.  

La source d'affectation détermine les coûts à affecter, tandis que les cibles d'affectation déterminent à quels emplacement affecter ces coûts. Par exemple, les coûts pour le type de coût Fournitures non stockables représentent une source d'affectation. Vous affectez tous les coûts de fournitures non stockables à trois centres de coûts : Atelier, Production, et Vente. Ces centres de coûts sont les cibles d'affectation.  

Pour chaque source d'affectation, vous définissez un niveau d'affectation, une période de validité et une variante comme identificateur de regroupement. Vous pouvez utiliser un traitement en lot pour définir des filtres afin de sélectionner les définitions d'affectation, puis exécuter les affectations des coûts automatiquement.  

Pour chaque cible d'affectation, vous définissez une base d'affectation. La base d'affectation peut être statique ou dynamique.  

-   Les bases d'affectation statique dépendent d'une valeur définie, par exemple, la superficie ou un ratio d'affectation prédéfini, comme 5:2:4.  
-   Les bases d'affectation dynamique dépendent de valeurs variables, telles que le nombre d'employés dans un centre de coût ou les revenus de vente d'un objet de coûts associé pour une période donnée.  

Le tableau suivant décrit une série de tâches et inclut des liens vers les rubriques qui les décrivent.

|À|Voir|  
|--------|---------|  
|Configurez la source d'affectation et ses cibles.|[Comment configurer la source d'affectation et ses cibles](finance-how-to-set-up-allocation-source-and-targets.md)|  
|Configurez plusieurs filtres pour les bases d'affectation dynamique.|[Définition de filtres pour les bases de ventilation dynamique](finance-setting-filters-for-dynamic-allocation-bases.md)|  
|Consultez un exemple sur le mode de définition d'une affectation statique.|[Exemple de scénario : Définition des ventilations statiques en fonction du ratio d'affectation](finance-scenario-example-defining-static-allocations-based-on-allocation-ratio.md)|  
|Consultez un exemple sur le mode de définition d'une affectation dynamique.|[Exemple de scénario : Définition des ventilations dynamique sur la base des articles vendus](finance-scenario-example-defining-dynamic-allocations-based-on-items-sold.md)|  

## <a name="see-also"></a>Voir aussi  
 [Paramétrage du contrôle de gestion](finance-set-up-cost-accounting.md)   
 [Transfert et report des écritures de coûts](finance-transfer-and-post-cost-entries.md)   
 [Comptabilité pour les coûts](finance-manage-cost-accounting.md)   
 [Terminologie en comptabilité analytique](finance-terminology-in-cost-accounting.md)   
 [À propos de la comptabilité analytique](finance-about-cost-accounting.md)

