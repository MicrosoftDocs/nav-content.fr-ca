---
title: "Détails de conception - Gestion des méthodes de réapprovisionnement"
description: "Aperçu des tâches pour définir une méthode de réapprovisionnement dans la planification des approvisionnements."
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
ms.openlocfilehash: 2cd1d0e770e5fd7daa92e98486038aefdb678c5a
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-handling-reordering-policies"></a>Détails de conception : gestion des méthodes de réapprovisionnement
Pour qu'un article participe à la planification des approvisionnements, une méthode de regroupement doit être définie. Les quatre méthodes de réapprovisionnement disponibles sont les suivantes :  
  
* Qté fixe de commande.  
* Qté maximum  
* Ordre  
* Lot pour lot  
  
Les méthodes Qté fixe de commande et Qté maximum sont liées à la planification de l'inventaire. Bien que la planification de l'inventaire soit techniquement plus simple que la procédure de contrepartie, ces stratégies doivent coexister avec la contrepartie pas à pas de l'approvisionnement et du suivi de commande. Pour contrôler l'intégration entre les deux, et livrer la visibilité dans la logique de planification utilisée, des principes stricts régissent la façon dont les méthodes de réapprovisionnement sont traitées.  
  
## <a name="in-this-section"></a>Dans cette section  
[Détails de conception : Le rôle du point de commande](design-details-the-role-of-the-reorder-point.md)  
[Détails de conception : surveillance du niveau de stock prévisionnel et du point de commande](design-details-monitoring-the-projected-inventory-level-and-the-reorder-point.md)  
[Détails de conception : Le rôle de l'intervalle de planification](design-details-the-role-of-the-time-bucket.md)  
[Détails de conception : rester sous le niveau de dépassement de capacité](design-details-staying-under-the-overflow-level.md)  
[Détails de conception : traitement du stock prévisionnel négatif](design-details-handling-projected-negative-inventory.md)  
[Détails de conception : méthodes de réapprovisionnement](design-details-reordering-policies.md)  
  
## <a name="see-also"></a>Voir aussi  
[Détails de conception : paramètres de planification](design-details-planning-parameters.md)   
[Détails de conception : tableau d'affectation de planification](design-details-planning-assignment-table.md)   
[Détails de conception : concepts centraux du système de planification](design-details-central-concepts-of-the-planning-system.md)   
[Détails de conception : équilibrage de la demande et de l'approvisionnement](design-details-balancing-demand-and-supply.md)   
[Détails de conception : planification de l'approvisionnement](design-details-supply-planning.md)
