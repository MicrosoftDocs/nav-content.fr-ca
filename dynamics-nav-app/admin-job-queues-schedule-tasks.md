---
title: "Programmer des projets à exécuter automatiquement"
description: "Les tâches programmées sont gérées par la file d'attente des travaux. Ces projets exécutent des rapports et des codeunits. Vous pouvez définir des projets à exécuter une fois, ou sur une base récurrente."
author: edupont04
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/01/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: d88b2157892a60fb74a5dcfcd83524895485689f
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="use-job-queues-to-schedule-tasks"></a>Utiliser des files d'attente des travaux pour programmer des tâches
Des files d'attente des travaux dans [!INCLUDE[d365fin](includes/d365fin_md.md)] permettent aux utilisateurs de planifier et d'exécuter des états et codeunits spécifiques. Vous pouvez définir des projets à exécuter une fois, ou sur une base récurrente. Par exemple, vous pouvez être amené à exécuter le rapport **Représentant : Statistiques ventes** chaque semaine pour suivre les ventes hebdomadaires d'un représentant, ou vous pouvez être amené à exécuter le codeunit **Traiter file d'attente courriels service** chaque jour pour vérifier si des courriels adressés aux clients concernant leurs commandes service sont envoyés en temps utile.  

## <a name="add-jobs-to-the-job-queue"></a>Ajouter des projets à la file d'attente des travaux
La fenêtre **Écritures file d'attente des travaux** répertorie tous les projets existants. Si vous ajoutez une nouvelle écriture file d'attente des travaux que vous voulez programmer, vous devez spécifier des informations sur le type d'objet à exécuter, par exemple un rapport ou un codeunit ainsi que le nom et le code de l'objet que vous voulez exécuter. Vous pouvez également ajouter des paramètres pour spécifier le comportement de la file d'attente des travaux. Par exemple, vous pouvez ajouter un paramètre pour envoyer uniquement des documents de vente reportés. Vous devez être autorisé à exécuter le rapport ou le codeunit spécifié, sans quoi une erreur est renvoyée lors de l'exécution de la file d'attente des travaux.  

Vous pouvez éventuellement définir un filtre dans le champ **Filtre catégorie de la file d'attente des travaux**. Les catégories de file d'attente des travaux peuvent être utilisées pour regrouper les projets de la liste.

[!INCLUDE[d365fin](includes/d365fin_md.md)] exécute automatiquement les projets selon le calendrier spécifié pour chaque écriture file d'attente des travaux. Vous pouvez également démarrer, arrêter et mettre en attente manuellement une écriture file d'attente des travaux.

### <a name="log-files"></a>Fichiers journaux
Les erreurs sont répertoriées dans la fenêtre **Écritures journal file d'attente des travaux** qui est accessible à partir du ruban. Vous pouvez également résoudre les erreurs de la file d'attente des travaux. Les données générées lors de l'exécution d'une file d'attente des travaux sont stockées dans la base de données.  

### <a name="background-posting-with-job-queues"></a>Report en arrière-plan avec les files d'attente des travaux
Les files d'attente des travaux sont un outil efficace pour programmer le travail des processus entreprise en arrière-plan. Par exemple, il peut y avoir une instance dans laquelle plusieurs utilisateurs essaient de reporter des documents de vente en même temps, mais uniquement une commande peut être traitée à la fois. En configurant une routine de report en arrière-plan, vous pouvez placer les reports dans une file d'attente pour les traiter en arrière-plan.  

 Sinon, vous pouvez programmer des reports à des heures pratiques pour votre organisation. Par exemple, il peut sembler raisonnable dans votre activité d'exécuter certaines routines lorsque la plupart de la saisie de données de la journée est achevée. Vous pouvez obtenir cette opération en configurant la file projets pour exécuter différents états de validation par lots, par exemple, **TPL valider commandes vente**, **TPL valider factures vente**et les états **TPL valider avoirs vente**.  

 [!INCLUDE[d365fin](includes/d365fin_md.md)] prend en charge la validation en arrière\-plan pour les types de document suivants :  

-   Ventes : document de vente, retour, note de crédit et facture  

-   Achats : bon de commande, retour, note de crédit et facture  

 Si la file d'attente des travaux ne peut pas valider la commande vente, le statut passe à **Erreur**, et la commande vente est ajoutée à la liste des commandes vente que l'utilisateur doit traiter.  

> [!NOTE]  
>  Lorsque vous programmez un document pour report et que le processus de report débute, la routine de report est automatiquement configurée pour expirer dans les deux heures si elle arrête de répondre pour une raison quelconque.  

Vous définissez cette utilisation de la file d'attente des travaux dans la fenêtre **Paramètres ventes** ou la fenêtre **Achats**, respectivement. Sur le raccourci **Report arrière-plan**, cochez la case **Reporter les documents via une file d'attente des travaux**, puis entrez les informations appropriées. Vous pouvez aussi utiliser le champ **Code catégorie de la file d'attente des travaux** pour exécuter toutes les écritures file d'attente des travaux avec ce code. Par exemple, vous pouvez utiliser une catégorie **ReportVente** qui filtre tous les documents de vente correspondant à n'importe quelle file d'attente des travaux ayant le même code catégorie.  

> [!IMPORTANT]  
>  Si vous configurez un projet qui reporte et imprime des documents et que l'imprimante affiche une boîte de dialogue, par exemple une demande d'informations d'identification ou un avertissement à propos de la quantité faible d'encre, votre document est reporté mais non imprimé. L'écriture file d'attente de travaux correspondante expire et la valeur du champ **Statut** devient **Erreur**. Par conséquent, nous vous recommandons de ne pas utiliser une configuration d'imprimante nécessitant une interaction avec les boîtes de dialogue de l'imprimante relatives au report en arrière-plan.  

## <a name="use-the-my-job-queue-part"></a>Utiliser le composant Ma file d'attente des travaux
Le composant **Ma file d'attente des travaux** répertorie les écritures files d'attente des travaux commencées par un utilisateur, mais qui ne sont pas terminées. Par défaut, le composant n'est pas visible et vous devez donc l'ajouter à votre tableau de bord. Pour plus d'informations, reportez-vous à [Procédure : modifier des tableaux de bord](change-role.md).  

Dans ce composant, vous pouvez visualiser les documents en cours de traitement ou en attente, pour lesquels votre ID est spécifié dans le champ **Code utilisateur affecté**. La composante vous permet de suivre toutes les écritures de file d'attente projet, y compris celles liées au report en arrière-plan. La composante peut vous indiquer rapidement s’il y a eu une erreur lors du report d’un document ou s’il existe des erreurs dans une écriture de file d'attente projet. Elle vous permet également d'annuler un report de document en cas de non-exécution.  

## <a name="security"></a>Sécurité  
Les écritures file d'attente des travaux s'exécutent sur la base d'autorisations. Ces autorisations doivent permettre l'exécution du rapport ou du codeunit.  

Lorsqu'une file d'attente des travaux est activée manuellement, elle s'exécute avec les informations d'identification de l'utilisateur. Lorsqu'une file d'attente des travaux est activée en tant que tâche programmée, elle s'exécute avec les informations d'identification de l'instance du serveur. Un projet s'exécute avec les informations d'identification de la file d'attente des travaux qui l'active. L'utilisateur qui a créé cette écriture file d'attente des travaux doit toutefois disposer d'autorisations. Lorsqu'un projet est exécuté dans la session utilisateur (par exemple, durant le report en arrière plan), il est exécuté avec les informations d'identification de l'utilisateur qui a créé ce projet.  

> [!IMPORTANT]  
>  Si vous utilisez l'ensemble d'autorisations SUPER qui est fourni avec [!INCLUDE[d365fin](includes/d365fin_md.md)], les utilisateurs et vous-même disposez des autorisations pour exécuter tous les objets. Dans ce cas, l'accès accordé à chaque utilisateur est uniquement limité par les autorisations relatives aux données.  

## <a name="using-job-queues-effectively"></a>Utilisation efficace des files d'attente des travaux  
L'enregistrement des écritures file d'attente des travaux possède plusieurs champs dont l'objectif est d'exécuter des paramètres dans un codeunit que vous avez indiqué comme devant être exécuté avec une file d'attente des travaux. Cela signifie également que les codeunits devant être exécutés via la file d'attente des travaux doivent être indiqués avec l'enregistrement des écritures file d'attente des travaux en tant que paramètre dans le déclencheur **OnRun**. Un niveau de sécurité supplémentaire est ainsi assuré, car les utilisateurs ne peuvent pas exécuter de codeunits aléatoires via la file d'attente des travaux. Si l'utilisateur doit transmettre des paramètres à un rapport, il n'a d'autre choix que celui d'inclure l'exécution de rapport dans un codeunit, lequel analyse ensuite les paramètres d'entrée et les intègre dans le rapport avant de l'exécuter.  

## <a name="see-also"></a>Voir aussi  
[Configuration et administration dans Dynamics NAV](admin-setup-and-administration.md)  
[Configuration de Dynamics NAV](setup.md)  

