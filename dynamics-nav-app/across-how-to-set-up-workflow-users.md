---
title: "Procédure : configurer des utilisateurs de flux de travail"
description: "Avant de pouvoir créer des flux de travail, vous devez configurer des utilisateurs qui participent aux flux de travail. Cela est nécessaire, par exemple, pour spécifier qui doit recevoir une notification pour agir sur une étape du flux de travail."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reject, delegate, request
ms.date: 08/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: ed7ca6e166f7100bc19a558825e3103170fc000c
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-workflow-users"></a>Procédure : Configurer des utilisateurs de workflow
Avant de pouvoir créer des flux de travail, vous devez configurer des utilisateurs qui participent aux flux de travail. Cela est nécessaire, par exemple, pour spécifier qui doit recevoir une notification pour agir sur une étape du flux de travail.  

Dans la fenêtre **Groupe d'utilisateurs du flux de travail**, configurez des utilisateurs sous des groupes d'utilisateurs de flux de travail, et spécifiez le numéro des utilisateurs dans une séquence de processus, comme une chaîne d'approbateurs.  

Les utilisateurs de flux de travail dont la fonction est utilisateurs approbation, à la fois demandeurs d'approbation et approbateurs, doivent également être définis dans la fenêtre **Paramètres utilisateur approbation**. Pour plus d'informations, voir [Procédure : configurer des utilisateurs d'approbation](across-how-to-set-up-approval-users.md).  

> [!NOTE]  
>  Pour indiquer qu'une demande d'approbation n'est pas approuvée tant que plusieurs approbateurs dans une chaîne d'approbation ne l'ont pas approuvée, configurez les approbateurs selon une hiérarchie. Pour le type d'approbateur **Approbateur**, configurez les approbateurs dans la fenêtre **Paramètres utilisateur d'approbation**. Pour le type d'approbateur **Groupe d'utilisateurs de flux de travail**, configurez les approbateurs dans la fenêtre **Groupe d'utilisateurs du flux de travail** et définissez la hiérarchie en affectant des numéros incrémentiels à chaque approbateur dans le champ **N° séquence** . Pour plus d'informations, voir [Procédure : configurer des utilisateurs d'approbation](across-how-to-set-up-approval-users.md) ainsi que cette rubrique.  
>   
>  Pour indiquer qu'une demande d'approbation n'est pas approuvée tant que plusieurs approbateurs de même niveau ne l'ont pas approuvée, indépendamment d'une hiérarchie, configurez un groupe d'utilisateurs de flux de travail horizontal. Pour le type d'approbateur **Groupe d'utilisateurs de flux de travail**, configurez les approbateurs dans la fenêtre **Groupe d'utilisateurs du flux de travail** et affectez le même numéro à chaque approbateur dans le champ **N° séquence** . Pour plus d'informations, voir cette rubrique.  

### <a name="to-set-up-a-workflow-user"></a>Configurer un utilisateur de workflow  

1. Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Groupes d'utilisateurs du flux de travail**, puis sélectionnez le lien associé.  
2. Sélectionnez l'action **Nouveau**. La fenêtre **Groupe d'utilisateurs du flux de travail** s'ouvre.  
3. Dans le champ **Code**, entrez 20 caractères maximum pour identifier le workflow.  
4. Dans le champ **Description**, décrivez le workflow.  
5. Dans le raccourci **Membres de groupe d'utilisateurs du workflow**, renseignez la première ligne des champs comme indiqué dans le tableau ci-dessous.  

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Nom d'utilisateur**|Spécifiez l'utilisateur qui participera aux workflows.<br /><br /> L'utilisateur doit exister dans la fenêtre **Paramètres utilisateur**. Pour en savoir plus, reportez-vous à [Procédure : gérer les utilisateurs et les autorisations](ui-how-users-permissions.md).|  
    |**N° séquence**|Spécifiez l'ordre dans lequel l'utilisateur du flux de travail s'engage dans un flux par rapport à d'autres utilisateurs. Ce champ peut être utilisé, par exemple, pour indiquer à quel moment l'utilisateur approuve, par rapport à d'autres approbateurs, lorsque vous utilisez l'option **Groupe d'utilisateurs de flux de travail** dans le champ **Type approbateur** de la réponse de flux de travail lié. **CONSEIL :**  pour indiquer qu'une demande d'approbation n'est pas approuvée tant que plusieurs approbateurs de même niveau ne l'ont pas approuvée, quelle que soit la hiérarchie, configurez un groupe d'utilisateurs horizontal en affectant le même numéro de séquence aux approbateurs appropriés.|  
6. Répétez l'étape 5 pour ajouter des utilisateurs de workflow dans le groupe d'utilisateurs.  
7. Répétez l'étape 2 à 6 pour ajouter des groupes d'utilisateurs de workflow.  

## <a name="see-also"></a>Voir aussi  
[Procédure : configurer des utilisateurs d'approbation](across-how-to-set-up-approval-users.md)   
[Paramétrage des workflows](across-set-up-workflows.md)   
[Utilisation des workflows](across-use-workflows.md)   
[Procédure pas à pas : Configuration et utilisation d'un flux d'approbation achat](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md)   
[Flux de travail](across-workflow.md)   

