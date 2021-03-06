---
title: "Procédure : créer des flux de travail à partir de modèles de flux de travail"
description: "Pour gagner du temps lors de la création de workflows, vous pouvez créer des workflows à partir de modèles de workflow existants."
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
ms.openlocfilehash: b0c2143b85a7301711498ecd40d6f6685be17eda
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-workflows-from-workflow-templates"></a>Procédure : créer des workflows à partir de modèles de workflow
Pour gagner du temps lors de la création de workflows, vous pouvez créer des workflows à partir de modèles de workflow existants.  

 Les modèles de workflow sont des workflows non modifiables qui existent dans la version générique de [!INCLUDE[d365fin](includes/d365fin_md.md)]. Les codes des modèles de workflow ajoutés par Microsoft ont le préfixe « MS- ».  

 Un autre moyen rapide de créer un workflow consiste à importer un workflow existant qui est stocké dans un fichier en dehors de [!INCLUDE[d365fin](includes/d365fin_md.md)]. Pour plus d'informations, voir [Procédure : exporter et importer des flux de travail](across-how-to-export-and-import-workflows.md).  

Dans la fenêtre **Workflow**, créez un workflow en répertoriant les étapes concernées sur les lignes. Chaque étape comprend un événement de workflow modéré par des conditions d'événement, et une réponse de workflow modérée par des options de réponse. Définissez les phases de workflow en renseignez les champs des lignes de workflow à partir de listes fixes de valeurs d'événement et de réponse qui sont les scénarios pris en charge par le code de l'application. Pour plus d'informations, reportez\-vous à [Procédure : créer des flux de travail](across-how-to-create-workflows.md).  

## <a name="to-create-a-workflow-from-workflow-template"></a>Pour créer un workflow à partir d'un modèle de workflow  
1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Flux de travail**, puis sélectionnez le lien associé.  
2.  Choisissez l'action **Créer le flux de travail à partir du modèle**. La fenêtre **Modèles flux de travail** s'ouvre.  
3.  Sélectionnez un modèle de workflow et cliquez sur le bouton **OK**.  

     La fenêtre **Flux de travail** s'ouvre pour un nouveau flux de travail contenant toutes les informations du modèle sélectionné. La valeur du champ **Code** est étendue avec « -01 », par exemple, pour indiquer que ce premier workflow est créé à partir du modèle de workflow.  
4.  Créez ensuite le workflow en modifiant les étapes de workflow ou en ajoutant de nouvelles étapes. Pour plus d'informations, reportez\-vous à [Procédure : créer des flux de travail](across-how-to-create-workflows.md).  

## <a name="see-also"></a>Voir aussi  
 [Procédure : créer des workflows](across-how-to-create-workflows.md)   
 [Procédure : exporter et importer des workflows](across-how-to-export-and-import-workflows.md)   
 [Procédure : afficher des instances d'étape de workflow archivées](across-how-to-view-archived-workflow-step-instances.md)   
 [Procédure : supprimer des workflows](across-how-to-delete-workflows.md)   
 [Procédure pas à pas : Configuration et utilisation d'un flux d'approbation achat](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md)   
 [Paramétrage des workflows](across-set-up-workflows.md)   
 [Utilisation des workflows](across-use-workflows.md)   
 [Flux de travail](across-workflow.md)   

