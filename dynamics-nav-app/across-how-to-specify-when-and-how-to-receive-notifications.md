---
title: "Procédure : spécifier quand et comment recevoir des notifications"
description: "Lorsque vous paramétrez des utilisateurs dans des workflows d'approbation, vous devez spécifier dans les fenêtres Paramètres de notification et Tableau de notification quand et comment chaque utilisateur reçoit des notifications sur les étapes du workflow d'approbation. Les utilisateurs individuels peuvent également modifier leur paramètre de notification en choisissant le bouton Changer les paramètres de notification sur toute notification."
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
ms.openlocfilehash: 7d4c09b216f64b41a1bd72507c7a09c05e19d06a
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-specify-when-and-how-to-receive-notifications"></a>Procédure : Spécifier quand et comment recevoir des notifications
Lorsque vous paramétrez des utilisateurs dans des workflows d'approbation, vous devez spécifier dans les fenêtres **Paramètres de notification** et **Tableau de notification** quand et comment chaque utilisateur reçoit des notifications sur les étapes du workflow d'approbation. Les utilisateurs individuels peuvent également modifier leur paramètre de notification en choisissant le bouton **Changer les paramètres de notification** sur toute notification.  

 Avant de pouvoir paramétrer des préférences de notification d'un utilisateur approbation, vous devez configurer l'utilisateur en tant qu'utilisateur approbation. Pour plus d'informations, voir [Procédure : configurer des utilisateurs d'approbation](across-how-to-set-up-approval-users.md).  

 Définissez la mise en forme et le contenu des notifications en configurant des modèles de notification. Pour plus d'informations, voir [Procédure : gérer les modèles de notification](across-how-to-manage-notification-templates.md).  

 Pour un grand nombre d'étapes d'approbation du workflow, il s'agit de notifier des utilisateurs qu'un événement s'est produit et qu'ils peuvent agir dessus. Par exemple, sur une étape de workflow, l'événement peut être que l'Utilisateur 1 demande l'approbation d'un nouvel enregistrement. La réponse associée est qu'une notification est envoyée à l'Utilisateur 2, l'approbateur. Sur la prochaine étape de workflow, l'événement peut être que l'Utilisateur 2 approuve l'enregistrement. La réponse associée est qu'une notification est envoyée à l'Utilisateur 3 afin de commencer un processus avec l'enregistrement approuvé. Pour les étapes de workflow concernant des approbations, chaque notification est liée à une écriture d'approbation. Pour plus d'informations, voir [Flux de travail](across-workflow.md).  

## <a name="specify-when-and-how-users-receive-notifications"></a>Spécifier quand et comment recevoir des notifications  

1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Configuration d'utilisateur d'approbation**, puis sélectionnez le lien associé.  
2.  Sélectionnez la ligne pour l'utilisateur pour lequel vous souhaitez configurer des préférences de notification, puis choisissez l'action **Configuration de la notification**.  
3.  Dans la fenêtre **Paramètres de notification**, renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Type de notification**|Spécifiez le type d'événement dont il s'agit dans la notification.<br /><br /> Sélectionnez l'une des options suivantes :<br /><br /> -   **Nouvel enregistrement** spécifie que la notification concerne un nouvel enregistrement, par exemple un document sur lequel l'utilisateur doit agir.<br />-   **Approbation** spécifie que la notification concerne une ou plusieurs demandes d'approbation.<br />-   **Échu** spécifie que l'objet de la notification est de rappeler aux utilisateurs qu'ils sont en retard pour agir sur un événement.|  
    |**Code modèle de notification**|Spécifiez le code du modèle de notification utilisé pour créer des notifications pour l'utilisateur.|  
    |**Notifications non agrégées**|Spécifiez si l'utilisateur reçoit une notification pour chaque événement notifications ou des notifications agrégées.<br /><br /> Si la case à cocher **Notifications non agrégées** n'est pas activée, l'utilisateur reçoit des notifications qui regroupent des informations sur les événements qui se produisent dans la même périodicité dans le tableau de notification.|  

     À présent, vous avez spécifié la manière dont l'utilisateur reçoit des notifications. Continuez à spécifier lorsque l'utilisateur reçoit des notifications.  

4.  Choisissez l'action **Calendrier de notification**.  
5.  Dans la fenêtre **Tableau de notification**, renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Description|  
    |---------------------------------|---------------------------------------|  
    |**Répétition**|Spécifiez la périodicité à laquelle l'utilisateur reçoit des notifications.|  
    |**Heure**|Spécifiez à quelle heure du jour l'utilisateur reçoit les notifications lorsque la valeur du champ **Répétition** est différente de la valeur **Instantané**.|  
    |**Fréquence quotidienne**|Spécifiez quel type de jours l'utilisateur reçoit des notifications lorsque la valeur dans le champ **Répétition** est **Tous les jours**.<br /><br /> Sélectionnez **Jour de la semaine** pour recevoir des notifications chaque jour travaillé de la semaine. Sélectionnez **Tous les jours** pour recevoir des notifications tous les jours, y compris le week-end.|  
    |**Lundi** à **Dimanche**|Spécifiez quel type de jours l'utilisateur reçoit des notifications lorsque la valeur dans le champ **Répétition** est **Chaque semaine**.|  
    |**Date du mois**|Spécifiez si l'utilisateur reçoit des notifications le premier ou le dernier jour du mois, ou à une date spécifique du mois.|  
    |**Date de notification mensuelle**|Spécifiez à quelle date du mois l'utilisateur reçoit des notifications lorsque la valeur dans le champ **Date du mois** est **Personnalisé**.|  

## <a name="change-when-and-how-you-receive-notifications"></a>Modifier le moment et le mode de réception des notifications  
1.  Sur l'une des notifications que vous avez reçue, par e\\\-mail ou par note, sélectionnez le bouton **Modifier les paramètres de notification**.  
2.  Dans la fenêtre **Paramètres de notification**, modifiez vos préférences de notification suivant les instructions de la procédure précédente.  

## <a name="see-also"></a>Voir aussi  
 [Procédure : configurer des utilisateurs d'approbation](across-how-to-set-up-approval-users.md)   
 [Procédure : gérer les modèles de notification](across-how-to-manage-notification-templates.md)   
 [Configuration de notifications de workflow](across-setting-up-workflow-notifications.md)   
 [Paramétrage des workflows](across-set-up-workflows.md)   
 [Utilisation des workflows](across-use-workflows.md)

