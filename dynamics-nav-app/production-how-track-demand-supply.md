---
title: "Procédure : suivre les relations entre l'offre et la demande"
description: "À partir d'un document d'approvisionnement ou de demande dans le réseau d'ordres, vous pouvez suivre la demande de commande (quantité suivie), les prévisions, les commandes permanentes ventes ou les paramètres de planification (quantité non suivie) qui ont donné lieu à la ligne planification en question."
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
ms.openlocfilehash: acf030ab57c9251671900b1262dd8441c241c185
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-track-relations-between-demand-and-supply"></a>Procédure : suivre les relations entre l'offre et la demande
À partir d'un document d'approvisionnement ou de demande dans le réseau d'ordres, vous pouvez suivre la demande de commande (quantité suivie), les prévisions, les commandes permanentes ventes ou les paramètres de planification (quantité non suivie) qui ont donné lieu à la ligne planification en question.

Les feuilles planification incluent également des informations de planification sur les entités sans rapport avec les commandes pour aider le gestionnaire à obtenir un programme d'approvisionnement optimal. Pour plus d'informations, voir la section « Éléments planification sans suivi ».

## <a name="to-track-linked-items"></a>Pour chaîner des articles liés
Par l'intermédiaire des systèmes de planification et de réservation, le suivi de commande montre de quelle manière les documents de vente, les bons de production et les bons de commande sont reliés aux ordres de fabrication.

La procédure suivante décrit comment chaîner des articles liés sur un ordre de fabrication planifié ferme. La procédure est similaire pour tous les autres types de commande, et à partir des lignes feuille planification.

1. Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Ordre de production planifié ferme**, puis sélectionnez le lien associé.
2. Ouvrez le bon de production planifié ferme approprié dans la liste.
3. Sur le raccourci **Lignes**, choisissez l'action **Fonctions**, puis l'action **Chaînage**.

Les lignes de la fenêtre **Chaînage** affichent les documents liés à la ligne de l'ordre de fabrication en cours.

## <a name="untracked-planning-elements"></a>Éléments de planification sans traçabilité
La fenêtre **Éléments planification sans suivi** s'affiche lorsque vous cliquez sur le champ **Qté sans suivi** dans la fenêtre **Planification commande**. Elle a deux objectifs :

1. Stockage d'informations sur les quantités non chaînées qui s'affichent lorsque l'utilisateur affiche la fenêtre Chaînage.
2. Stockage des messages d'avertissement qui s'affichent lorsque l'utilisateur clique sur l'icône **Avertissement** dans la fenêtre **Feuille planification**

La fenêtre inclut les écritures représentant une quantité excédentaire non chaînée du réseau de chaînage. Ces écritures sont générées au cours de l'exécution de la planification et expliquent la provenance de la quantité excédentaire non chaînée des lignes chaînage. Cet excédent non chaîné peut provenir des lignes suivantes :

- Prévisions production ;
- Commandes ouvertes ;
- Stock de sécurité ;
- Point de commande ;
- Inventaire maximum
- Quantité de réappro. ;
- Qté maximum commande ;
- Qté minimum commande ;
- Commandé par ;
- Seuil (% taille lot).

## <a name="see-also"></a>Voir aussi  
[Planification](production-planning.md)   
[Paramétrage de la production](production-configure-production-processes.md)  
[Production](production-manage-manufacturing.md)    
[Stock](inventory-manage-inventory.md)  
[Procédure d'achat](purchasing-manage-purchasing.md)  
[Détails de conception : réservation, chaînage et message d'action](design-details-reservation-order-tracking-and-action-messaging.md)  
[Détails de conception : planification de l'approvisionnement](design-details-supply-planning.md)   
[Configurer des recommandations : planification de l'approvisionnement](setup-best-practices-supply-planning.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

