---
title: "Procédure : Facturer des projets"
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
ms.openlocfilehash: c0dcce83dfba30af38f33a6bf814b15862d5fc19
ms.contentlocale: fr-ca
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-invoice-jobs"></a>Procédure : Facturer des projets
Au cours du projet, les coûts provenant de l'utilisation de ressources, de matières, et d'achats associés au projet peuvent s'accumuler. Au fur et à mesure de la progression du projet, ces transactions sont reportées dans le journal projet. Il est important que tous les coûts soient enregistrés dans le journal projet avant de facturer le client.

Vous pouvez facturer l'ensemble du projet à partir de la fenêtre **Lignes tâche projet** ou facturer uniquement les lignes facturables sélectionnées dans la fenêtre **Lignes planning**. La facturation peut avoir lieu une fois le projet terminé ou à certains intervalles au cours du projet sur la base d'un calendrier de facturation.

**Remarque** : Si vous sélectionnez **Facturable** dans le champ **Type ligne projet** dans les documents d'achat pour les achats associés au projet, les lignes planning projet prêtes pour facturation sont créées. Pour en savoir plus, reportez-vous à [Procédure : Gérer des fournitures d'un projet](projects-how-manage-project-supplies.md).

## <a name="to-create-and-post-a-job-sales-invoice"></a>Pour créer et reporter une facture vente projet  
Vous pouvez créer une facture pour un projet ou pour une ou plusieurs tâches projet pour un client lorsque le travail à facturer est terminé ou lorsque la date de facturation basée sur un calendrier de facturation est atteinte.

Dans la fenêtre **Projets**, vous pouvez facturer un client en sélectionnant le projet, puis en cliquant sur **Créer une facture vente projet**. La procédure suivante explique comment utiliser un traitement en lot pour facturer plusieurs projets.  

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Projet Créer facture vente**, puis sélectionnez le lien connexe.  
2. Renseignez les champs selon vos besoins. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.
3. Définissez des filtres si vous souhaitez limiter le nombre de projets que le traitement en lot va traiter.
3. Pour créer les factures, cliquez sur le bouton **OK**.  

## <a name="to-create-multiple-job-sales-invoices-from-job-planning-lines"></a>Pour créer plusieurs factures vente projet à partir de lignes planification projet  
Vous pouvez créer une facture à partir des lignes planification projet et indiquer à ce moment-là la quantité de l'article, la ressource ou le compte GL sur lequel vous souhaitez facturer.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Projets**, puis sélectionnez le lien connexe.
2. Ouvrez le projet approprié.
3. Sélectionnez une tâche projet pour laquelle le champ **Type tâche projet** contient **Validation** puis, cliquez sur **Lignes planning projet**.  
4. Dans une ligne planning projet, dans le champ **Qté à transférer à facturer**, saisissez la quantité de l'article, la ressource, le type de compte général sur lequel vous souhaitez facturer.  
5. Cliquez sur **Créer facture vente**.
6. Dans la fenêtre **Projet Créer facture vente**, saisissez la date de validation et si vous souhaitez créer une facture ou ajouter cette facture à une facture existante.
7. Cliquez sur le bouton **OK**.

    Dans la ligne planning projet, dans le champ **Qté à transférer à facturer**, vous pouvez visualiser la quantité.

8. Dans la fenêtre **Lignes planning projet**, cliquez sur **Avoirs/Factures vente**.

    La fenêtre **Facture vente** s'ouvre et affiche la quantité que vous avez transférée à la facture.  
9. Apportez les modifications supplémentaires, puis cliquez sur **Valider**.

**Remarque** : La procédure ci-dessus permet également de créer, de consulter, puis de valider un avoir vente associé à un projet.

## <a name="to-calculate-and-post-job-completion-entries"></a>Pour calculer et reporter les écritures d'achèvement du projet  
À la fin des activités d'un projet (validation et facturation comprises), vous devez le mettre à jour pour définir le **Statut** du projet sur **Terminé**. Ensuite, vous devez inverser tous les TEC reportés antérieurement dans le grand livre.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Projets**, puis sélectionnez le lien connexe.  
2. Sélectionnez un projet ouvert, puis cliquez sur **Modifier**.
3. Dans le champ **Statut**, sélectionnez **Terminé**.
4. Suivez les phases d'aide pour calculer et reporter les TEC. Sinon, suivez les étapes 5 et 6 pour le faire manuellement.  
5. Cliquez sur **Calculer TEC**.
6. Dans la fenêtre **Projet Calculer TEC**, renseignez les champs comme nécessaire.  

     Les écritures TEC projet créées par le traitement par lots auront la case **Projet terminé** cochée pour indiquer qu'il s'agit d'écritures d’achèvement.  

7. Cliquez sur **Projet Valider TEC en comptabilité**.
8. Dans la fenêtre **Projet Valider TEC en comptabilité**, renseignez les champs selon vos besoins.  

     Les écritures comptabilité TEC projet créées par le traitement par lots verront la case **Projet terminé** cochée pour indiquer qu'il s'agit d'écritures d’achèvement.

## <a name="see-also"></a>Voir aussi
[Gérer des projets](projects-manage-projects.md)  
[Finance](finance-setup.md)  
[Gestion des achats](purchasing-manage-purchasing.md)         
[Gestion des ventes](sales-manage-sales.md)      
[Utiliser Dynamics NAV](ui-work-product.md)  

