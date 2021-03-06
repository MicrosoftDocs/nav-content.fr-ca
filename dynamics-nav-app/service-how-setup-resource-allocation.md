---
title: Configurer l'affectation des ressources
description: "Découvrez comment le système peut vous aider à affecter une personne dotée des compétences requises à la fourniture d'un service."
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: resource, skill, service, zones
ms.date: 08/22/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 9ca6bb733eb0f7cf090551da7a6d5c7b5cd3216b
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---

# <a name="how-to-set-up-resource-allocation"></a>Procédure : configurer l'affectation des ressources
Pour assurer la bonne exécution d'une tâche service, il est important de trouver une ressource qualifiée. Vous pouvez configurer [!INCLUDE[d365fin](includes/d365fin_md.md)] de manière à affecter facilement une ressource disposant des compétences appropriées pour le travail. Dans [!INCLUDE[d365fin](includes/d365fin_md.md)], ce processus est appelé _affectation de ressources_. Vous pouvez affecter des ressources en fonction de leur compétence, de leur disponibilité, ou selon qu'elles se trouvent dans la même zone service que le client. 

Pour utiliser l'affectation des ressources, vous devez définir :  
  
* Les compétences nécessaires à la réparation et la maintenance des articles de service. Vous les affectez aux articles de service et aux ressources.  
* Les régions géographiques, appelées zones, que vous définissez pour votre marché. Par exemple, est, ouest, centre, etc. Vous les affectez aux clients et aux ressources.  
* Si les compétences ressource et les zones doivent être affichées, et si un avertissement doit être affiché si une ressource non qualifiée ou une ressource qui ne figure pas dans la zone du client est sélectionnée.  

## <a name="to-set-up-skills"></a>Pour configurer des compétences
1. Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Compétences**, puis sélectionnez le lien associé.  
2. Renseignez les champs selon vos besoins. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-assign-skills-to-service-items-and-resources"></a>Pour affecter des compétences aux articles de service et aux ressources
1. Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Articles de service** ou **Ressources**, puis sélectionnez le lien associé.  
2. Ouvrez la fiche de l'article de service ou de la ressource, puis sélectionnez l'une des options suivantes :  
  
    * Pour les articles de service, sélectionnez **Compétences ressource**.  
    * Pour les ressources, sélectionnez **Compétences**.  

## <a name="to-set-up-zones"></a>Pour configurer des zones
1. Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Zones**, puis sélectionnez le lien associé.  
2. Renseignez les champs selon vos besoins. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-assign-zones-to-customers-and-resources"></a>Pour affecter des zones aux clients et aux ressources 
1. Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Clients** ou **Ressources**, puis sélectionnez le lien associé.  
2. Ouvrez la fiche de l'article de service ou de la ressource, puis sélectionnez l'une des options suivantes :  
  
    * Pour les clients, sélectionnez une zone dans le champ **Code zone service**.  
    * Pour les ressources, sélectionnez l'action **Zones service**.  

## <a name="to-specify-what-to-show-when-a-resource-is-chosen"></a>Pour spécifier les éléments à afficher lorsqu'une ressource est sélectionnée
1. Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Configuration de service**, puis sélectionnez le lien associé. 
2. Dans le champ **Compétences ressources**, sélectionnez l'une des options décrites dans le tableau suivant.  
  
    |**Option**|**Description**|  
    |------------|-------------|  
    |Afficher code seulement | Affiche le code uniquement.|  
    |Utiliser alertes et afficher | Affiche les informations et un avertissement si vous choisissez une ressource qui n'est pas qualifiée.|  
    |Aucun affichage | N'affiche pas ces informations.|  

## <a name="to-update-resource-capacity"></a>Pour mettre à jour la capacité ressource  
Vous devrez peut-être modifier la capacité des ressources.  
  
1. Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Capacité des ressources**, puis sélectionnez le lien associé.  
2. Sélectionnez la ressource, puis l'action **Paramétrage capacité ressource**.  
3. Apportez les modifications, puis sélectionnez **Mettre à jour la capacité**.  

## <a name="to-update-skills-for-items-service-items-or-service-item-groups"></a>Pour mettre à jour les compétences pour des articles, des articles de service ou des groupes d'articles de service
Vous pouvez modifier les codes compétence affectés à des articles, par exemple de **PC** à **PCS**, pour un article, un article de service ou pour tous les articles d'un groupe articles de service.  
  
1. Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Articles**, **Article de service** ou **Groupe articles de service**, puis sélectionnez le lien associé.  
2. Sélectionnez l'entité à mettre à jour, puis sélectionnez l'action **Compétences ressource**.  
3. Sur la ligne contenant le code à modifier, dans le champ **Code compétence**, sélectionnez le code compétence.  
4.  Si des articles de service sont associés à l'article, une boîte de dialogue incluant les deux options suivantes s'ouvre :  
  
    * Attribue la valeur sélectionnée aux codes compétence : sélectionnez cette option pour remplacer l'ancien code compétence de tous les articles de service associés par le nouveau code.  
    * Supprime les codes compétence ou met à jour leur relation : sélectionnez cette option pour modifier le code compétence de l'article uniquement. Le code compétence des articles de service associés sera réaffecté, c'est-à-dire que le champ **Affecté à partir de** sera mis à jour.  
  
## <a name="see-also"></a>Voir aussi
[Procédure : affecter des ressources](service-how-to-allocate-resources.md)  
[Procédure : configurer des heures de travail et des heures de service](service-how-setup-work-service-hours.md)  
[Procédure : configurer la génération de rapports de pannes](service-how-setup-fault-reporting.md)  
[Procédure : configurer des codes prestations standard](service-how-setup-service-coding.md)  
 


