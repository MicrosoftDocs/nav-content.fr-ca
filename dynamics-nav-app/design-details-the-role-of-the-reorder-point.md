---
title: "Détails de conception - Le rôle du point de commande"
description: "Cette rubrique met l'accent sur l'importance de définir un point de réapprovisionnement, afin de déterminer quand commander plus d'inventaire."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: desigh, reorder, demand, supply
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 8035a670077e53981e9c366d22bdb20df06d8c1b
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-the-role-of-the-reorder-point"></a>Détails de conception : Le rôle du point de commande
En plus de l'équilibrage général de la demande et de l'approvisionnement, le système de planification doit également surveiller les niveaux d'inventaire des articles affectés pour respecter les stratégies de réapprovisionnement définies.  
  
Un point de commande représente la demande lors d'un délai. Lorsque l'inventaire prévisionnel passe en dessous du niveau d'inventaire défini par le point de réapprovisionnement, il est temps de commander une plus grande quantité. Par ailleurs, l'inventaire doit diminuer progressivement et probablement atteindre zéro (ou le niveau d'inventaire de sécurité), jusqu'au moment du réapprovisionnement.  
  
Par conséquent, le système de planification suggère une commande d'approvisionnement planifiée en aval au moment où l'inventaire prévisionnel passe sous le point de réapprovisionnement.  
  
Le point de réapprovisionnement indique un certain niveau d'inventaire. Cependant, les niveaux d'inventaire peuvent changer de façon significative au cours de la plage de temps et, par conséquent, le système de planification doit constamment contrôler l'inventaire prévisionnel disponible.  
  
## <a name="see-also"></a>Voir aussi  
[Détails de conception : méthodes de réapprovisionnement](design-details-reordering-policies.md)   
[Détails de conception : paramètres de planification](design-details-planning-parameters.md)   
[Détails de conception : gestion des méthodes de réapprovisionnement](design-details-handling-reordering-policies.md)   
[Détails de conception : planification de l'approvisionnement](design-details-supply-planning.md)
