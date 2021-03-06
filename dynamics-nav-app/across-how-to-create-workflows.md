---
title: "Procédure : créer des workflows"
description: "Vous pouvez créer des workflows qui connectent des tâches de processus entreprise exécutées par différents utilisateurs. Les tâches système, telles que le report automatique, peuvent être incluses comme étapes du flux de travail, précédées ou suivies des tâches de l'utilisateur. Demander et accorder une approbation pour créer des enregistrements sont des étapes classiques du workflow."
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
ms.openlocfilehash: fcf0a0c9ffc12de6fe21adb2a0906f241374aa2c
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-workflows"></a>Procédure : créer des workflows
Vous pouvez créer des workflows qui connectent des tâches de processus entreprise exécutées par différents utilisateurs. Les tâches système, telles que le report automatique, peuvent être incluses comme étapes du flux de travail, précédées ou suivies des tâches de l'utilisateur. Demander et accorder une approbation pour créer des enregistrements sont des étapes classiques du workflow.  

Dans la fenêtre **Workflow**, créez un workflow en répertoriant les étapes concernées sur les lignes. Chaque étape comprend un événement de workflow modéré par des conditions d'événement, et une réponse de workflow avec des options de réponse. Définissez les phases de workflow en renseignez les champs des lignes de workflow à partir de listes fixes de valeurs d'événement et de réponse qui sont les scénarios pris en charge par le code de l'application.  

Lorsque vous créez des workflows, vous pouvez copier les étapes à partir de workflows existants ou de modèles de workflow. Les modèles de workflow représentent des workflows non modifiables qui existent dans la version générique de [!INCLUDE[d365fin](includes/d365fin_md.md)]. Le code des modèles de workflow ajoutés par Microsoft a le préfixe « MS- », comme dans « MS-PIW ». Pour plus d'informations, reportez\-vous à [Procédure : créer des flux de travail à partir de modèles de flux de travail](across-how-to-create-workflows-from-workflow-templates.md).  

Si votre scénario d'entreprise requiert des événements ou réponses de flux de travail qui ne sont pas pris en charge, un partenaire Microsoft doit les implémenter en personnalisant le code de l'application.  
  
> [!NOTE]  
>  Toutes les notifications relatives aux étapes du flux de travail sont envoyées à l'aide d'une file d'attente des travaux. Assurez-vous que la file d'attente des travaux dans votre installation est configurée pour traiter les notifications du flux de travail, et que la case à cocher **Démarrer automatiquement à partir de NAS** est activée. Pour plus d'informations, voir [Utiliser des files d'attente des travaux pour planifier des tâches](admin-job-queues-schedule-tasks.md).  

## <a name="to-create-a-workflow"></a>Pour créer un workflow  
1. Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Flux de travail**, puis sélectionnez le lien associé.  
2. Sélectionnez l'action **Nouveau**. La fenêtre **Flux de travail** s'ouvre.  
3. Dans le champ **Code**, entrez 20 caractères maximum pour identifier le workflow.  
4. Pour créer le workflow à partir d'un modèle de workflow, dans la fenêtre **Flux de travail**, choisissez l'action **Créer le flux de travail à partir du modèle**. Pour plus d'informations, reportez\-vous à [Procédure : créer des flux de travail à partir de modèles de flux de travail](across-how-to-create-workflows-from-workflow-templates.md).  
5. Dans le champ **Description**, décrivez le workflow.  
6. Dans le champ **Catégorie**, spécifiez la catégorie à laquelle le workflow appartient.  
7. Dans le champ **En cas d'événement**, spécifiez l'événement qui doit se produire pour démarrer l'étape du workflow.  

    Lorsque vous choisissez le champ, la fenêtre **Événements de flux de travail** s'ouvre pour vous permettre de choisir parmi tous les événements de workflow qui existent.  
8. Dans le champ **Condition**, spécifiez une ou plusieurs conditions qui doivent être remplies pour que l'événement dans le champ **En cas d'événement** puisse se produire.  

    Lorsque vous sélectionnez le champ, la fenêtre **Conditions d'événement** s'ouvre pour vous permettre de choisir dans une liste de champs de filtre pouvant être utilisés comme conditions pour l'événement en question. Vous pouvez ajouter des champs de filtre à utiliser comme conditions d'événement. Définissez des filtres de condition d'événement comme vous définissez des filtres sur les pages de demande de rapport.  

    Si l'événement de workflow est la modification d'un champ spécifique d'un enregistrement, la fenêtre **Conditions d'événement** s'ouvre avec des options pour sélectionner le champ et le type de modification.  

    1.  Pour spécifier une modification de champ pour l'événement, dans la fenêtre **Conditions d'événement**, dans le champ **Champ**, sélectionnez le champ qui est modifié.  
    2.  Dans le champ **Opérateur**, sélectionnez **Diminué**, **Augmenté** ou **Modifié**.  
9. Dans le champ **Alors, réponse**, spécifiez la réponse qui suivra lorsque l'événement de workflow se produira.  

     Lorsque vous choisissez le champ, la fenêtre **Réponses de flux de travail** s'ouvre pour vous permettre de choisir parmi toutes les réponses de workflow qui existent et de définir des options de réponse pour la réponse sélectionnée.  
10. Dans le raccourci **Options pour la réponse sélectionnée**, spécifiez les options pour la réponse de workflow, en sélectionnant des valeurs dans les différents champs qui s'affichent, comme suit :  

    1.  Pour spécifier des options pour une réponse de workflow impliquant l'envoi d'une notification, renseignez les champs comme indiqué dans le tableau suivant.  

        |Champ|Description|  
        |----------------------------------|---------------------------------------|  
        |**Code utilisateur du destinataire**|Spécifiez l'utilisateur auquel la notification doit être envoyée. Remarque : cette option n'est disponible que pour les réponses de workflow avec un espace réservé pour un utilisateur spécifique. Pour les réponses de flux de travail sans espaces réservés pour les utilisateurs, le destinataire de la notification est généralement défini par une configuration utilisateur d'approbation.|  
        |**Page cible du lien**|Spécifiez une autre page dans [!INCLUDE[d365fin](includes/d365fin_md.md)] que le lien de la notification ouvre au lieu de la page par défaut.|  
        |**Lien personnalisé**|Spécifiez l'URL d'un lien qui est ajouté à la notification en complément du lien vers une page dans [!INCLUDE[d365fin](includes/d365fin_md.md)].|  
    2.  Pour spécifier des options pour une réponse de workflow impliquant la création d'une demande d'approbation, renseignez les champs comme indiqué dans le tableau suivant.  

        |Champ|Description|  
        |----------------------------------|---------------------------------------|  
        |**Formule de date d'échéance**|Spécifiez le nombre de jours suite auxquels la demande d'approbation doit être résolue, à compter de la date à laquelle elle a été envoyée.|  
        |**Déléguer après**|Spécifiez si et quand une demande d'approbation est automatiquement déléguée au substitut approprié. Vous pouvez choisir de déléguer automatiquement un, deux ou cinq jours après la date de demande d'approbation.|  
        |**Type approbateur**|Spécifiez l'approbateur, en fonction de la configuration des utilisateurs d'approbation et de flux de travail.<br /><br /> Les options possibles sont les suivantes :<br /><br /> -   **Représentant/acheteur** indique que l'utilisateur configuré dans le champ **Code représentant/acheteur** de la fenêtre **Configuration d'utilisateur d'approbation** détermine l'approbateur. Les écritures de demande d'approbation sont ensuite créées en fonction de la valeur du champ **Type limite approbateur**.<br />     Pour plus d'informations, voir [Procédure : configurer des utilisateurs d'approbation](across-how-to-set-up-workflow-users.md).|  
        |**Afficher le message de confirmation**|Spécifiez si un message de confirmation apparaît aux utilisateurs après leur demande d'approbation.|  
        |**Type limite approbateur**|Spécifiez les effets des limites d'approbation des approbateurs lorsque les écritures demande d'approbation sont créées pour eux. Un approbateur qualifié est un approbateur pour lequel la limite d'approbation est supérieure à la valeur de la demande.<br /><br /> Les options possibles sont les suivantes :<br /><br /> 1.  **Chaîne d'approbateurs** spécifie que les écritures demande d'approbation sont créées pour tous les approbateurs du demandeur jusqu'au et y compris le premier approbateur qualifié.<br />2.  **Approbateur direct** spécifie qu'une écriture de demandes d'approbation n'est créée que pour l'approbateur immédiat du demandeur, quelle que soit la limite d'approbation de l'approbateur.<br />3.  **Premier approbateur qualifié** spécifie qu'une écriture de demandes d'approbation n'est créée que pour le premier approbateur qualifié du demandeur.<br />|  
    3.  Pour spécifier des options pour une réponse de flux de travail impliquant la création de lignes journal, renseignez les champs comme indiqué dans le tableau suivant.  

        |Champ|Description|  
        |----------------------------------|---------------------------------------|  
        |**Nom modèle journal général**|Spécifiez le nom du modèle journal général dans lequel les lignes journal spécifiées sont créées.|  
        |**Nom lot de journal général**|Spécifiez le nom du lot journal général dans lequel les lignes journal spécifiées sont créées.|  

11. Choisissez les boutons **Augmenter le décalage** et **Réduire le décalage** pour décaler le nom de l'événement dans le champ **Si** pour définir la position de l'étape dans le flux de travail.  
    1.  Indiquez que l'étape est la suivante dans l'ordre du workflow en mettant en retrait le nom de l'événement sous le nom d'événement de l'étape précédente.  
    2.  Indiquez que l'étape est l'une des étapes alternatives qui peuvent démarrer en fonction de sa condition en plaçant le nom de l'événement à la même indentation que les autres étapes. Classez ces étapes facultatives en fonction de leur priorité en plaçant l'étape la plus importante en premier.  

    > [!NOTE]  
    >  Vous ne pouvez modifier que le décalage d'une étape qui n'a pas d'étape suivante.  

12. Répétez les étapes 7 à 11 pour ajouter d'autres étapes de workflow, avant ou après l'étape que vous venez de créer.  
13. Activez la case à cocher **Activé** pour spécifier que le workflow démarre lorsque l'événement de la première étape de type **Point d'entrée** se produit. Pour plus d'informations, voir [Utilisation des workflows](across-use-workflows.md).  

> [!NOTE]  
>  N'activez pas un workflow tant que vous n'êtes pas sûr qu'il est terminé et que les étapes de workflow concernées peuvent démarrer.  

> [!TIP]  
>  Pour visualiser les relations entre les tables qui sont utilisées dans le flux de travail, choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), et entrez **Flux de travail - Relations de table**.  

## <a name="see-also"></a>Voir aussi  
[Procédure : créer des workflows à partir de modèles de workflow](across-how-to-create-workflows-from-workflow-templates.md)   
[Procédure : configurer des utilisateurs d'approbation](across-how-to-set-up-approval-users.md)   
[Configuration de notifications de workflow](across-setting-up-workflow-notifications.md)   
[Procédure : afficher des instances d'étape de workflow archivées](across-how-to-view-archived-workflow-step-instances.md)   
[Procédure : supprimer des workflows](across-how-to-delete-workflows.md)   
[Procédure pas à pas : Configuration et utilisation d'un flux d'approbation achat](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md)   
[Paramétrage des workflows](across-set-up-workflows.md)   
[Utilisation des workflows](across-use-workflows.md)   
[Flux de travail](across-workflow.md)      


