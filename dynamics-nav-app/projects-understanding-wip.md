---
title: "Méthodes TEC pour calculer et enregistrer la progression d'un projet"
description: "Décrit les différentes méthodes de travaux en cours (TEC) qui peuvent être utilisées pour reporter, surveiller et calculer les données financières des projets en cours."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: work in process, work in progress, calculate project WIP
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 4a472d7a45cacfe4cd2534747f447a1e4ca7a303
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="understanding-wip-methods"></a>Comprendre les méthodes TEC
[!INCLUDE[d365fin](includes/d365fin_md.md)] prend en charge les méthodes suivantes pour calculer et enregistrer la valeur des travaux en cours.

| Méthode TEC | Formule de calcul | Description du calcul |
| --- | --- | --- |
| Valeur de coût |Revenus réceptionnés = Facturable (prix facturé)<br /><br /> Coûts totaux estimés = Facturable (prix total) x Coût budgétaire (ratio)<br /><br /> Coûts TEC = (Pourcentage avancement - % facturé) x Coûts totaux estimés<br /><br /> Pourcentage avancement = Utilisation (coûts indiqués) / Budget (coûts indiqués)<br /> % facturé = Facturable (prix facturé)<br /><br /> Coûts réceptionnés facturables (prix total)= Utilisation (coûts indiqués) - TEC |Le calcul Valeur de coût commence par calculer la valeur du montant fourni en prenant une proportion des coûts totaux estimés basée sur le pourcentage d'achèvement. Les coûts facturés sont soustraits en prenant une proportion des coûts totaux estimés basée sur le pourcentage facturé.<br /><br /> Ce calcule nécessite que le prix total facturable, le prix total du budget et les coûts budgétaires totaux soient correctement renseignés pour l'ensemble du projet. |
| Coût des ventes |Revenus réceptionnés = Facturable (prix facturé)<br /><br /> Coûts réceptionnés = Coût total du budget x Pourcentage facturé<br /><br /> % facturé = Facturable (prix facturé) / Facturable (prix total)<br /><br /> (Le % facturé apparaît sous forme de colonne dans les lignes tâche projet)<br /><br /> Coûts TEC = Utilisation (coûts indiqués) – Coûts réceptionnés |Le calcul Coût des ventes commence par calculer les coûts réceptionnés. Les coûts sont réceptionnés proportionnellement sur la base des coûts budgétaires totaux.<br /><br /> Ce calcule nécessite que le prix total facturable et les coûts budgétaires totaux soient correctement renseignés pour l'ensemble du projet. |
| Valeur des ventes |Coûts réceptionnés = Utilisation (coûts indiqués)<br /><br /> Revenus réceptionnés = Utilisation (prix total) x Facturation prévue (ratio)<br /><br /> % recouvrement des coûts = Facturable (prix total)/Prix total du budget<br /><br /> Vente TEC = Ventes réceptionnées - Facturable (prix facturé) |Le calcul Valeur des ventes réceptionne les revenus proportionnellement sur la base de l'utilisation (coûts indiqués) et du ratio attendu de recouvrement des coûts.<br /><br /> Ce calcule nécessite que le prix total facturable et le prix budgétaire total soient correctement renseignés pour l'ensemble du projet. |
| Pourcentage d'achèvement |Coûts réceptionnés = Utilisation (coûts indiqués)<br /><br /> Revenus réceptionnés = Facturable (prix total) x Pourcentage avancement<br /><br /> Pourcentage avancement = Utilisation (coûts indiqués) / Budget (coûts indiqués)<br /> (Appelé « % achèvement coût » dans les lignes tâche projet)<br /><br /> Vente TEC = Ventes réceptionnées - Facturable (prix facturé) |Le calcul Pourcentage avancement réceptionne les revenus proportionnellement sur la base du pourcentage d'achèvement, soit l'utilisation (coûts indiqués) par rapport aux coûts budgétés.<br /><br /> Ce calcule nécessite que le prix total facturable et les coûts budgétaires totaux soient correctement renseignés pour l'ensemble du projet. |
| Contrat complété |Montant TEC = Coût indiqué TEC = Utilisation (coût total)<br /><br /> Montant vente TEC = Facturable (Prix facturé) |La méthode Fin de contrat ne réceptionne pas les revenus et les coûts avant la fin du projet. Cela peut être utile lorsque l'estimation des coûts et des revenus du projet est excessivement difficile.<br /><br /> L'ensemble de l'utilisation est reporté dans le compte Coûts TEC (actif) et toutes les ventes facturées sont reportées dans le compte Ventes facturées TEC (passif) jusqu'à la fin du projet. |

## <a name="see-also"></a>Voir aussi
[Gestion de projets](projects-manage-projects.md)  
[Finance](finance.md)  
[Achats](purchasing-manage-purchasing.md)         
[Ventes](sales-manage-sales.md)      
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

