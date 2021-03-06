---
title: "Procédure : enregistrer la consommation et la production pour un bon de production"
description: "Cette tâche d'exécution est réalisée dans la fenêtre **Journal production**. Le journal combine les fonctions des journaux de sortie et de consommation distincts en un seul journal. Vous accédez directement au journal combiné depuis un bon de production libéré. Son objectif principal est de reporter manuellement la consommation de composantes, la quantité d'articles finis produits et le temps passé dans les opérations."
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
ms.openlocfilehash: e912412475c8b62404d7c417b9ae3ebbddeb9a17
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-register-consumption-and-output-for-one-released-production-order-line"></a>Procédure : enregistrer la consommation et la sortie pour une ligne bon de production libéré
Cette tâche d'exécution est réalisée dans la fenêtre **Journal production**. Le journal combine les fonctions des journaux de sortie et de consommation distincts en un seul journal. Vous accédez directement au journal combiné depuis un bon de production libéré. Son objectif principal est de reporter manuellement la consommation de composantes, la quantité d'articles finis produits et le temps passé dans les opérations. Les valeurs sont reportées dans le grand livre sous le bon de production libéré. Les quantités consommées sont reportées comme écritures article négatives, les quantités sorties sont reportées comme écritures positives et les heures passées sont reportées comme écritures du grand livre de capacité. Ces valeurs reportées peuvent également être visualisées au bas du journal sous forme de quantités réelles.  

> [!NOTE]  
>  Parce que les données relatives à la consommation sont traitées avec celles relatives à la sortie, ce journal permet d'afficher les opérations et les composantes liées dans une structure opératoire logique. Les composantes sont décalées sous l'opération à laquelle elles correspondent. Vous devrez pour cela utiliser des codes lien itinéraire.  

> [!NOTE]  
>  Les composantes ne comportant pas de code lien itinéraire apparaissent en haut du journal.  

## <a name="to-register-consumption-and-output"></a>Pour enregistrer la consommation et la sortie  
1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Bons de production libérés**, puis sélectionnez le lien associé.  
2.  Ouvrez une ligne de bon de production libéré qui est prête à être enregistrée, puis, sur le raccourci **Lignes**, choisissez l'action **Ligne**, puis l'action **Journal production**.  

    La fenêtre **Journal production** s'ouvre et affiche les lignes journal pour la ligne bon de production en fonction des fenêtres **Composante bon de production** et **Itinéraire bon de production** Ces lignes proviennent de la nomenclature de production et de l'itinéraire affectés à l'article en cours de production. Pour plus d'informations, reportez\-vous à [Procédure : créer des nomenclatures de production](production-how-to-create-routings.md).  

3.  Dans le champ **Date report** situé en haut du journal, entrez une date de report qui s'applique à toutes les lignes. Par défaut, ce champ affiche la date de travail. Il permet d'aligner rapidement les dates de report de toutes les lignes, si nécessaire.  

    > [!NOTE]  
    >  Une date de report entrée sur une ligne prime par rapport à la date entrée dans ce champ.  

4.  Dans le champ **Filtre méthode consommation** situé en haut du journal, vous pouvez choisir d'afficher également la consommation et la sortie reportées automatiquement à l'aide des méthodes de consommation définies respectivement pour l'article et pour la ressource.  

    Sur chaque type de ligne du journal, seuls les champs appropriés sont indiqués. Les autres sont vierges et protégés en écriture.  

    À l'ouverture du journal, celui-ci comporte les quantités à reporter. Si aucune donnée n'a été reportée jusque-là, tous les champs de quantité affichent par défaut les quantités prévues issues du bon de production. Si des reports partielles ont eu lieu, les champs de quantité des lignes affichent les quantités restantes. Les quantités et délais déjà reportés pour la commande apparaissent au bas du journal en tant qu'écritures réelles.  

    Vous avez la possibilité de définir les quantités devant figurer dans le champ **Quantité sortie** lors de la première ouverture du journal. Pour ce faire, utilisez le champ **Quantité sortie prédéfinie** du raccourci **Général** de la fenêtre **Configuration de la fabrication**. 

5.  Entrez maintenant les quantités de consommation et production appropriées dans les champs modifiables.  

    > [!NOTE]  
    >  Seule la quantité sortie figurant sur la dernière ligne journal du type d'écriture **Sortie** ajuste le niveau d'inventaire durant le report du journal. Par conséquent, ne reportez le journal, avec les quantités sorties prévues sur la dernière ligne de sortie, que lorsque tous les articles finis auront été réellement produits.  

6.  Sélectionnez le champ **Terminé** des lignes de sortie pour indiquer que l'opération est terminée. Ce champ est lié au champ **État d'itinéraire** des lignes itinéraire bon de production.  
7.  Choisissez l'action **Reporter** pour enregistrer les quantités entrées, puis fermez le journal.  

S'il reste des valeurs à reporter, le journal les contiendra la prochaine fois que vous l'ouvrirez. Les valeurs reportées sont affichées sous forme de valeurs réelles au bas du journal.  

> [!NOTE]  
>  Si un article consommé est bloqué, le journal ne reporte pas les quantités de consommation pour cet article. Si une unité de production ou un atelier est bloqué, le journal ne reporte ni les quantités sortie ni les temps de traitement de la ligne de sortie en question.  

> [!NOTE]  
>  Si vous fermez le journal sans le reporter, les modifications seront perdues.  

> [!WARNING]  
>  La fenêtre **Journal production** ne peut pas être utilisée par deux utilisateurs simultanément. Cela signifie que si l'utilisateur 2 ouvre la fenêtre et entre des données alors que l'utilisateur 1 travaille déjà dans la fenêtre, l'utilisateur 2 peut perdre des données lorsque l'utilisateur 1 ferme la fenêtre.  

## <a name="see-also"></a>Voir aussi  
[Production](production-manage-manufacturing.md)    
[Paramétrage de la production](production-configure-production-processes.md)  
[Planification](production-planning.md)      
[Stock](inventory-manage-inventory.md)  
[Procédure d'achat](purchasing-manage-purchasing.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

