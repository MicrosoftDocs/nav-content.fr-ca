---
title: "Comprendre les méthodes TEC"
author: SorenGP
ms.custom: na
ms.date: 11/01/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: f21357897dd730d96db7abab469d5958c6fe117c
ms.contentlocale: fr-ca
ms.lasthandoff: 06/26/2017

---

# <a name="understanding-wip-methods"></a>Comprendre les méthodes TEC

Le module Dynamics NAV prend en charge les méthodes suivantes pour calculer et enregistrer la valeur des travaux en cours.

|Méthode TEC |Formule de calcul |Description du calcul|
|-----------|--------------------|-----------------------|
|Valeur de coût|Revenus réceptionnés = Facturable (prix facturé)<br /><br /> Coûts totaux estimés = Facturable (prix total) x Coût budgétaire (ratio)<br /><br /> Coûts TEC = \(Pourcentage avancement - % facturé\) x Coûts totaux estimés<br /><br /> Pourcentage avancement = Utilisation (coûts indiqués) / Budget (coûts indiqués)<br /> % facturé = Facturable (prix facturé)<br /><br /> Coûts réceptionnés facturables (prix total)= Utilisation (coûts indiqués) - TEC|Le calcul Valeur de coût commence par calculer la valeur du montant fourni en prenant une proportion des coûts totaux estimés basée sur le pourcentage d'achèvement. Les coûts facturés sont soustraits en prenant une proportion des coûts totaux estimés basée sur le pourcentage facturé.<br /><br /> Ce calcule nécessite que le prix total facturable, le prix total du budget et les coûts budgétaires totaux soient correctement renseignés pour l'ensemble du projet.|
|Coût des ventes|Revenus réceptionnés = Facturable (prix facturé)<br /><br /> Coûts réceptionnés = Coût total du budget x Pourcentage facturé<br /><br /> % facturé = Facturable (prix facturé) / Facturable (prix total)<br /><br /> \(Le % facturé apparaît sous forme de colonne dans les lignes tâche projet\)<br /><br /> Coûts TEC = Utilisation (coûts indiqués) – Coûts réceptionnés|Le calcul Coût des ventes commence par calculer les coûts réceptionnés. Les coûts sont réceptionnés proportionnellement sur la base des coûts budgétaires totaux.<br /><br /> Ce calcule nécessite que le prix total facturable et les coûts budgétaires totaux soient correctement renseignés pour l'ensemble du projet.|
|Valeur des ventes|Coûts réceptionnés = Utilisation (coûts indiqués)<br /><br /> Revenus réceptionnés = Utilisation (prix total) x Facturation prévue (ratio)<br /><br /> % recouvrement des coûts = Facturable (prix total)/Prix total du budget<br /><br /> Vente TEC = Ventes réceptionnées - Facturable (prix facturé)|Le calcul Valeur des ventes réceptionne les revenus proportionnellement sur la base de l'utilisation (coûts indiqués) et du ratio attendu de recouvrement des coûts.<br /><br /> Ce calcule nécessite que le prix total facturable et le prix budgétaire total soient correctement renseignés pour l'ensemble du projet.|
|Pourcentage d'achèvement|Coûts réceptionnés = Utilisation (coûts indiqués)<br /><br /> Revenus réceptionnés = Facturable (prix total) x Pourcentage avancement<br /><br /> Pourcentage avancement = Utilisation (coûts indiqués) / Budget (coûts indiqués)<br /><br /> \(Appelé « % achèvement coût » dans les lignes tâche projet\)<br /> Vente TEC = Ventes réceptionnées - Facturable (prix facturé)|Le calcul Pourcentage avancement réceptionne les revenus proportionnellement sur la base du pourcentage d'achèvement, soit l'utilisation (coûts indiqués) par rapport aux coûts budgétés.<br /><br /> Ce calcule nécessite que le prix total facturable et les coûts budgétaires totaux soient correctement renseignés pour l'ensemble du projet.|
|Contrat complété|Montant TEC = Montant coût TEC = Activité \(Coût total\)<br /><br /> Montant vente TEC = Facturable \(Prix facturé\)|La méthode Fin de contrat ne réceptionne pas les revenus et les coûts avant la fin du projet. Cela peut être utile lorsque l'estimation des coûts et des revenus du projet est excessivement difficile.<br /><br /> L'ensemble de l'activité est validé dans le Compte coûts TEC \(actif\) et toutes les ventes facturées sont validées dans le Compte ventes facturées TEC \(passif\) jusqu'à la fin du projet.|

## <a name="see-also"></a>Voir aussi
[Gérer des projets](projects-manage-projects.md)  
[Finance](finance-setup.md)  
[Gestion des achats](purchasing-manage-purchasing.md)         
[Gestion des ventes](sales-manage-sales.md)      
[Utiliser Dynamics NAV](ui-work-product.md)  

