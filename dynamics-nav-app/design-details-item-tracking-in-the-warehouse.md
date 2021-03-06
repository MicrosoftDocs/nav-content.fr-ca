---
title: "Détails de conception - Disponibilité traçabilité"
description: "Cette rubrique décrit comment les personnes qui traitent les commandes peuvent se baser sur la disponibilité des numéros de série ou de lot."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, item, tracking, serial number, lot number, outbound documents
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 1e632e2d7e0b4afe167721d0b68102b48f820307
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-item-tracking-availability"></a>Détails de conception : disponibilité traçabilité
Les fenêtres **Lignes traçabilité** et **Disponibilité traçabilité** fournissent des informations de disponibilité dynamique pour les numéros de série ou de lot. L'objectif de cela est d'augmenter la transparence pour les utilisateurs dans les documents sortants, tels que des commandes vente, en leur indiquant les numéros de série ou le nombre d'unités d'un numéro de lot qui sont affectés actuellement à d'autres documents ouverts. Cela réduit l'incertitude liée à la double affectation et assure aux préparateurs de commande que les numéros de suivi d'article et les dates qu'ils promettent sur les documents de vente non reportés puissent être respectés. Pour plus d'informations, reportez\-vous à [Détails de conception : fenêtre Lignes traçabilité](design-details-item-tracking-lines-window.md).  
  
Lorsque vous ouvrez la fenêtre **Lignes traçabilité**, les données de disponibilité sont récupérées à partir du tableau **Écriture comptable article** et du tableau **Ecriture réservation** sans aucun filtre de date. Lorsque vous choisissez le champ **N° de série** ou le champ **N° lot**, la fenêtre **Disponibilité traçabilité** s'ouvre et affiche un résumé des informations de suivi article dans le tableau **Ecriture réservation**. Le résumé contient les informations suivantes sur chaque numéro de série ou de lot dans la ligne traçabilité :  
  
|Champ|Description|  
|---------------------------------|---------------------------------------|  
|**Quantité totale**|Quantité totale du numéro de série/lot actuellement en inventaire.|  
|**Quantité totale demandée**|Quantité totale du numéro de série/lot actuellement demandé dans tous les documents.|  
|**Quantité suspendue actuelle**|La quantité qui est saisie dans l'instance active de la fenêtre **Lignes traçabilité**, mais n'est pas encore consignée dans la base de données.|  
|**Quantité totale disponible**|La quantité de numéros de série ou de numéro de lot qui est disponible pour l'utilisateur à la demande.<br /><br /> Cette quantité est calculée d'autres champs de la fenêtre comme suit :<br /><br /> quantité totale – (quantité totale demandée + quantité suspendue actuelle).|  
  
> [!NOTE]  
>  Vous pouvez également visualiser les informations du tableau précédent à l'aide de la fonction **Sélectionner écritures** de la fenêtre **Lignes traçabilité**.  
  
Pour préserver les performances de la base de données, les données de disponibilité ne sont récupérées qu'une fois depuis la base de données lorsque vous ouvrez la fenêtre **Lignes traçabilité** et utilisez la fonction **Actualiser disponibilité** dans la fenêtre.  
  
## <a name="calculation-formula"></a>Formule de calcul  
Comme indiqué dans le tableau précédent, la disponibilité d'un numéro de série ou de lot spécifique est calculée comme suit :  
  
* quantité totale disponible = quantité en inventaire – (toutes les demandes + quantité pas encore consignée dans la base de données)  
  
> [!IMPORTANT]  
>  Cette formule implique que le calcul de disponibilité de numéro de série ou de lot ne considère que l'inventaire et ignore les reçus prévus. Par conséquent, l'approvisionnement qui n'a pas encore été reporté dans l'inventaire n'affecte pas la disponibilité de la traçabilité, contrairement à la disponibilité d'un article normal, où les réceptions projetées sont incluses.  
  
## <a name="see-also"></a>Voir aussi  
[Détails de conception : traçabilité](design-details-item-tracking.md)
