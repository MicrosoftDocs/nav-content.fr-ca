---
title: "Procédure pas à pas - Réception et rangement dans les configurations de stockage de base"
description: "Dans [!INCLUDE[d365fin](includes/d365fin_md.md)], les processus entrants de réception et de rangement peuvent être effectués de quatre manières, à l'aide de différentes fonctionnalités en fonction du niveau de complexité de l'entrepôt."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 0a540f5813ed67ee62e43390d6d11b7c3a137f13
ms.contentlocale: fr-ca
ms.lasthandoff: 10/23/2017

---
# <a name="walkthrough-receiving-and-putting-away-in-basic-warehouse-configurations"></a>Procédure pas à pas : Réception et rangement dans les configurations de stockage de base
Dans [!INCLUDE[d365fin](includes/d365fin_md.md)], les processus entrants de réception et de rangement peuvent être effectués de quatre manières, à l'aide de différentes fonctionnalités en fonction du niveau de complexité de l'entrepôt.  

|Méthode|Processus entrant|Zones|Reçus|Rangements|Niveau de complexité (Voir [Détails de conception : configuration d'entrepôt](design-details-warehouse-setup.md))|  
|------------|---------------------|----------|--------------|----------------|--------------------------------------------------------------------------------------------------------------------|  
|A|Report de la réception et du rangement à partir de la ligne commande|X|||2|  
|B|Report de la réception et du rangement à partir d'un document de rangement inventaire|||X|3|  
|C|Report de la réception et du rangement à partir d'un document réception entrepôt||X||4/5/6|  
|J|Report de la réception d'un document réception entrepôt et report du rangement à partir d'un document de rangement entrepôt||X|X|4/5/6|  

Pour plus d'informations, reportez\-vous à [Détails de conception : flux d'enlogement](design-details-inbound-warehouse-flow.md).  

La procédure pas à pas suivante illustre la méthode B dans la table précédente.  

## <a name="about-this-walkthrough"></a>À propos de cette procédure pas à pas  
Pour les configurations entrepôt de base, lorsque votre emplacement est configuré pour exiger un traitement des rangements mais pas un traitement des réceptions, vous utilisez la fenêtre **Rangement inventaire** pour enregistrer et reporter les informations de rangement et de réception pour vos documents sources entrants. Le document source entrant peut être un bon de commande, un retour vente, un ordre de transfert entrant ou un bon de production dont la production est prête à être rangée.

> [!NOTE]
> Bien que les paramètres soient appelés **Prélèvement requis** et **Rangement requis**, vous pouvez quand même reporter les réceptions et les livraisons directement à partir des documents commerciaux sources dans les emplacements où vous cochez ces cases.  

Cette procédure pas à pas présente les tâches suivantes.  

-   Configuration de l'emplacement ARGENT pour les rangements inventaire.  
-   Configuration de l'emplacement ARGENT pour la gestion de zone.  
-   Définissez une zone par défaut pour l'article LS-81. (LS-75 est déjà défini dans CRONUS.)  
-   Créez un bon de commande pour le fournisseur 10 000 pour 40 haut-parleurs.  
-   Vérifier que les zones de rangement sont prédéfinies par la configuration.  
-   Lancement du bon de commande pour le traitement en entrepôt.  
-   Création d'un rangement inventaire sur la base d'un document source libéré.  
-   Vérifier que les zones de rangement sont héritées du bon de commande.  
-   Enregistrement d'un mouvement entrepôt dans l'entrepôt et en même temps report de la réception achat pour le bon de commande d'origine.  

## <a name="roles"></a>Rôles  
Cette procédure pas à pas présente les tâches effectuées par les rôles utilisateur suivants :  

-   Gestionnaire d'entrepôt  
-   Agent d'achats  
-   Magasinier  

## <a name="prerequisites"></a>Conditions préalables  
Pour exécuter ce processus pas à pas, vous devez :  

-   avoir CRONUS International Ltd. installé.  
-   Pour devenir magasinier dans un emplacement ARGENT, procédez comme suit :  

    1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Employés entrepôt**, puis sélectionnez le lien associé.  
    2.  Choisissez le champ **ID utilisateur** et sélectionnez votre propre compte utilisateur dans la fenêtre **Utilisateurs**.  
    3.  Dans le champ **Code magasin**, entrez ARGENT.  
    4.  Sélectionnez le champ **Par défaut**.  

## <a name="story"></a>Scénario  
Ellen, responsable d'entrepôt chez CRONUS International Ltd., crée un bon de commande de 10 unités de l'article LS-75 et 30 unités de l'article LS-81 du fournisseur 10000, qui doivent être approvisionnés à l'entrepôt ARGENT. Lorsque la livraison arrive à l'entrepôt, Jean, l'employé de l'entrepôt, range les articles dans les zones par défaut définies pour les articles. Lorsque Jean reporte le rangement, les articles sont reportés comme étant reçus dans l'inventaire et disponibles à la vente ou pour d'autres demandes.  

## <a name="setting-up-the-location"></a>Configuration de l'emplacement  
 La configuration de la fenêtre **Fiche magasin** définit les flux d'entrepôt de la société.  

### <a name="to-set-up-the-location"></a>Pour configurer l'emplacement  

1.  Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), saisissez **Magasins**, puis sélectionnez le lien connexe.  
2.  Ouvrez la fiche emplacement ARGENT.  
3.  Activez la case à cocher **Rangement requis**.  

    Configurez une zone par défaut pour les deux numéros d'article afin de contrôler l'endroit où ils sont rangés.  

4.  Choisissez l'action **Zones**.  
5.  Sélectionnez la première ligne, pour la zone S-01-0001, puis choisissez l'action **Contenu**.  

    Remarquez dans la fenêtre **Contenu de la zone** que l'article LS-75 est déjà configuré comme contenu dans la zone S-01-0001.  

6.  Sélectionnez l'action **Nouveau**.  
7.  Sélectionnez les champs **Fixe** et **Par défaut**.  
8.  Dans le champ **N° article**, saisissez LS-81.  

## <a name="creating-the-purchase-order"></a>Création du bon de commande  
Les bons de commande sont le type de document source entrant le plus répandu.  

### <a name="to-create-the-purchase-order"></a>Pour créer le bon de commande  

1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Bons de commande**, puis sélectionnez le lien associé.  
2.  Sélectionnez l'action **Nouveau**.  
3.  Créez un bon de commande pour le fournisseur 10 000 à la date de travail (23 janvier) comportant les lignes bon de commande suivantes.  

    |Article|Code d'emplacement|Code de zone|Quantité|  
    |----------|-------------------|--------------|--------------|  
    |LS_75|ARGENTE|S-01-0001|10|  
    |LS-81|ARGENTE|S-01-0001|30|  

    > [!NOTE]  
    >  Le code de zone est renseigné automatiquement en fonction de la configuration effectuée dans la section « Configuration de l'emplacement ».  

    Informez l'entrepôt que le bon de commande est prêt pour le traitement en entrepôt lorsque la livraison arrive.  

4.  Sélectionnez l'action **Lancer**.  

    La livraison des haut-parleurs provenant du fournisseur 10000 est arrivée dans l'entrepôt ARGENT. Jean procède à leur rangement.  

## <a name="receiving-and-putting-the-items-away"></a>Réception et rangement des articles  
Dans la fenêtre **Rangement inventaire**, vous pouvez gérer toutes les activités enlogement pour un document source spécifique, tel qu'un bon de commande.  

### <a name="to-receive-and-put-the-items-away"></a>Pour recevoir et ranger des articles  

1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Rangements stock**, puis sélectionnez le lien associé.  
2.  Sélectionnez l'action **Nouveau**.  
3.  Sélectionnez le champ **Document source**, puis sélectionnez **Bon de commande**.  
4.  Sélectionnez le champ **N° origine**, sélectionnez la ligne correspondant à l'achat au fournisseur 10000, puis cliquez sur le bouton **OK**.  

    Sinon, sous l'onglet **Actions**, dans le groupe **Fonctions**, choisissez **Extraire document origine**, puis sélectionnez le bon de commande.  

5.  Choisissez l'action **Remplir automatiquement la quantité à traiter**.  

    Sinon, dans le champ **Qté à traiter**, saisissez respectivement 10 et 30 sur les deux lignes rangement inventaire.  

6.  Choisissez l'action **Reporter**, sélectionnez l'action **Réceptionner**, puis choisissez le bouton **OK**.  

    Les 40 haut-parleurs sont à présent enregistrés comme rangés dans la zone S-01-0001, et une écriture article positive est créée pour refléter la réception achat reportée.  

## <a name="see-also"></a>Voir aussi  
 [Procédure : ranger des articles à l'aide des rangements inventaire](warehouse-how-to-put-items-away-with-inventory-put-aways.md)   
 [Procédure : configurer des entrepôts de base avec les zones d'opérations](warehouse-how-to-set-up-basic-warehouses-with-operations-areas.md)   
 [Procédure : déplacer les composantes vers une zone opérations dans les configurations d'entrepôt de base](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md)   
 [Procédure : Prélever pour la fabrication et l'assemblage](warehouse-how-to-pick-for-production.md)   
 [Procédure : déplacer des articles ad hoc dans les configurations de stockage de base.](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md)   
 [Détails de conception : flux d'enlogement](design-details-inbound-warehouse-flow.md)   
 [Procédures pas à pas liées au processus entreprise](walkthrough-business-process-walkthroughs.md)  
 [Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

