---
title: "Procédure pas à pas : gestion des projets"
description: "Cette procédure pas-à-pas présente les fonctionnalités de gestion de projets dans les projets. Les projets vous permettent de programmer l'utilisation des ressources de votre compagnie et de suivre les différents objet de coûts à l'utilisation des ressources sur un projet spécifique. Les projets impliquent la consommation d'heures employé, d'heures machines, d'articles dans l'inventaire et d'autres types d'utilisation pouvant faire l'objet d'un suivi au fur et à mesure de l'avancée du projet."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 75d0c1648b152717c6ceff69f37b399c8cc3ae26
ms.contentlocale: fr-ca
ms.lasthandoff: 10/23/2017

---
# <a name="walkthrough-managing-projects-with-jobs"></a>Procédure pas à pas : gestion des projets
Cette procédure pas-à-pas présente les fonctionnalités de gestion de projets dans les projets. Les projets vous permettent de programmer l'utilisation des ressources de votre compagnie et de suivre les différents objet de coûts à l'utilisation des ressources sur un projet spécifique. Les projets impliquent la consommation d'heures employé, d'heures machines, d'articles dans l'inventaire et d'autres types d'utilisation pouvant faire l'objet d'un suivi au fur et à mesure de l'avancée du projet.  

 Cette procédure pas à pas couvre la configuration d'un nouveau projet, en plus de tâches plus communes telles que la gestion des prix fixes, les paiements en plusieurs versements, le report de factures à partir de projets et la copie de projets.  

## <a name="about-this-walkthrough"></a>À propos de cette procédure pas à pas  
 Cette procédure pas à pas présente les tâches suivantes :  

### <a name="setting-up-a-job"></a>Configuration d'un projet  
 Avec la structure de budget paramétrée pour les projets, la création d'un projet est très simple. Cette procédure pas-à-pas couvre les procédures suivantes :  

-   Configuration de lignes tâche projet et de lignes planification.  
-   Création de prix spécifiques à un projet pour des articles, des ressources et des comptes du grand livre.  
-   la facturation à partir d'un projet.  

### <a name="handling-fixed-prices"></a>Gestion de prix fixes  
 Dans les projets, vous pouvez gérer des prix fixes, ainsi que les prix de biens ou de services convenus à l'avance avec les clients. Pour cette procédure pas-à-pas, vous pouvez procéder comme suit :  

-   Découvrir comment les valeurs contrat et facture sont déterminées.  
-   Autoriser le travail supplémentaire qui n'a pas été facturé dans le calendrier.  

### <a name="copying-a-job"></a>Copie d'un projet  
 Cette partie de la procédure se concentre sur la manière de copier tout ou partie d'un projet afin de réduire la saisie manuelle de données et ainsi améliorer la précision. Elle inclut les points suivants :  

-   la copie d'une partie d'un projet dans un nouveau projet ;  
-   la copie de prix spécifiques à un projet.  
-   Copie de lignes planification.  

### <a name="making-payment-by-installment"></a>Paiement en plusieurs versements  
 Lorsqu'un projet important et onéreux dure longtemps, le client conclut souvent une entente avec la compagnie pour payer en plusieurs versements. Ce scénario montre comment configurer un paiement en plusieurs versements et couvre les points suivants :  

-   Création d'un paiement en plusieurs versements pour un projet.  
-   la facturation de paiements à des clients ;  
-   Comptabilité à utiliser dans un projet configuré en vue d'un paiement en plusieurs versements.  

## <a name="roles"></a>Rôles  
 Cette procédure pas à pas inclut les tâches correspondant aux rôles suivants :  

-   Chef de projet  
-   Membre de l'équipe de projet  

## <a name="prerequisites"></a>Conditions préalables  
 Avant d'exécuter cette procédure pas à pas, veuillez suivre les instructions ci-dessous :  

-   Installez la base de données de démonstration CRONUS International Ltd.
-   Créez des exemples de données en respectant les étapes décrites dans la section suivante.  

## <a name="story"></a>Scénario  
Ce procédure pas à pas se concentre sur la société CRONUS International Ltd., entreprise de conception et de conseil, qui conçoit et équipe de nouvelles infrastructures (telles que des salles de conférence et des bureaux) avec du mobilier, des accessoires et des unités de stockage. La plus grande partie de son travail est orientée vers des projets. Prakash est chef de projet chez CRONUS. Il utilise les projets pour avoir un aperçu de chaque projet en cours entrepris par CRONUS, ainsi que les projets terminés. C'est généralement lui qui conduit les négociations avec les clients et entre les principaux éléments du projet (lignes tâche et planning, ainsi que les prix) dans [!INCLUDE[d365fin](includes/d365fin_md.md)]. Il trouve que la création, la gestion et la consultation des informations sont simples. Prakash aime également la manière dont [!INCLUDE[d365fin](includes/d365fin_md.md)] permet de copier des projets et d'effectuer un paiement en plusieurs versements.

 Tricia, membre de l'équipe de projet qui rend compte à Prakash, est responsable de la surveillance quotidienne du projet. Elle entre dans le système son propre travail, ainsi que celui accompli par les techniciens sur chaque tâche. Elle enregistre les articles qu'ils ont utilisés et les coûts exposés.  

## <a name="preparing-sample-data"></a>Préparation d'exemples de données  
 Pour préparer cette procédure pas à pas, vous devez ajouter Tricia comme nouvelle ressource.  

### <a name="to-prepare-the-sample-data"></a>Pour préparer les exemples de données  

1.  Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Ressources**, puis sélectionnez le lien connexe.  
2.  Choisissez l'action **Nouveau** pour créer une fiche ressource.  
3.  Sous le raccourci **Général**, entrez les informations suivantes :  

    - **N°.**: **Tricia**  
    - **Nom** : **Tricia**  
    - **Type** : **Personne**  

4.  Dans le champ **Unité de mesure de base**, choisissez l'action **Nouveau** pour ouvrir la fenêtre **Unité de mesure de ressource**. Dans le champ **Code**, sélectionnez **Heure**. Cliquez sur le bouton **OK**.  
5.  Sur le raccourci **Facturation**, entrez les informations suivantes :  

    -   **Coût unitaire direct** : **5**  
    -   **% coût indirect** : **4**  
    -   **Coût unitaire** : **10**  
    -   **Groupe compta. produit** : **Services**  
    -   **Groupe compta. produit TVA** : **TVA 25**  

6.  Cliquez sur le bouton **OK** pour enregistrer les modifications.  

 Dans la procédure suivante, vous créez un lot journal projet pour Tricia pour reporter son utilisation.  

### <a name="to-create-a-job-journal-batch"></a>Pour créer un lot journal projet  

1.  Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Feuilles projet**, puis sélectionnez le lien connexe.  
2.  Dans la fenêtre **Feuille projet**, choisissez le champ **Nom de la feuille**. La fenêtre **Noms feuilles projet** s’ouvre.  
3.  Choisissez l'action **Nouveau** pour créer une ligne avec les informations suivantes :  

    -   **Nom** : **Tricia**  
    -   **Description** : **Tricia**  
    -   **Souches de n°** : **JJNL-GEN**  

4.  Cliquez sur le bouton **OK** pour fermer toutes les fenêtres.  

## <a name="setting-up-a-job"></a>Configuration d'un projet  
 Dans ce cas, CRONUS a décroché un contrat avec un client, Progressive Home Furnishings, pour la conception d'une salle de conférence/repas. Le client est basé aux États-Unis et le projet nécessitera l'utilisation d'un logiciel spécial. Le chef de projet conclut une entente avec le client et crée un projet en relation avec cette entente.  

### <a name="to-set-up-a-job"></a>Pour configurer un projet  

1.  Choisissez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Projets**, puis choisissez le lien associé.  
2.  Choisissez l'action **Nouveau** pour créer une fiche.  
3.  Sous le raccourci **Général**, entrez les informations suivantes :  

    -   **Description** : **Conseil sur l'installation de la salle de conférence**  
    -   **N° client facturé** : **01445544**  

4.  Sur le raccourci **Validation**, entrez les informations suivantes :  

    -   **Statut** : **Commande**  
    -   **Groupe compta. projet** : **Configuration**  
    -   **Méthode TEC** : **Valeur de coût**  

5.  Sur le raccourci **Durée**, tapez la date du jour dans les champs **Date début** et **Date fin**. Ces dates permettront d'appliquer les conversions de devise lors de la facturation du projet.  
6.  Sur le raccourci **International**, définissez le code devise sur **USD**. Si vous sélectionnez USD dans le champ **Code devise facture**, le projet sera facturé en dollars américains et planifié dans la devise locale de CRONUS uniquement.  

 Vous pouvez personnaliser la tarification des clients projet par projet, en fonction des accords que vous avez définis. Dans la procédure suivante, le chef de projet indique un coût horaire pour Tricia, définit le prix du logiciel à utiliser et ajoute les frais de déplacement que le client a accepté de payer.  

### <a name="to-customize-pricing"></a>Pour personnaliser la tarification  

1.  Dans la fiche projet, choisissez l'action **Ressource**.  
2.  Dans la fenêtre **Prix ressource projet**, entrez les informations suivantes :  

    -   **Code** : **Tricia**  
    -   **Prix unitaire** : **20**  

3.  Cliquez sur le bouton **OK** pour fermer la fenêtre.  
4.  Sélectionnez l'action **Article**.  
5.  Dans la fenêtre **Prix article projet**, entrez les informations suivantes et le prix personnalisé :  

    1.  **N° article** : **80201 (programme graphique)**  
    2.  **Prix unitaire** : **200**  

6.  Cliquez sur le bouton **OK** pour fermer la fenêtre.  
7.  Choisissez l'action **Compte du grand livre**.  
8.  Dans la fenêtre **Prix compte GL de projet**, entrez les informations suivantes en majorant les frais de déplacement que le client a accepté de payer de 25 % :  

    1.  **Compte du grand livre** : **8430 (Déplacement)**  
    2.  **Facteur coût unitaire** : **1,25**  

9. Cliquez sur le bouton **OK** pour fermer la fenêtre.  

 Les dernières étapes de la configuration d'un projet consistent à ajouter les tâches projet et les lignes planification qui font partie de chaque tâche. Les lignes planification déterminent ce qui est facturé au client.  

### <a name="to-add-job-tasks"></a>Pour ajouter des tâches de projet  

1.  Dans la fiche **Projet** du nouveau projet, choisissez l'action **Lignes tâche projet**.  
2.  Le tableau suivant décrit les informations que vous devez entrer dans les champs.  

    |N° tâche projet|Description|Type tâche projet|  
    |------------------|---------------------------------------|-------------------|  
    |1000|Consultance sur la configuration de la salle|Début total|  
    |1010|Réunion de consultation avec le client|Report|  
    |1020|Développement|Report|  
    |1090|Total de la consultation|Fin total|  

3.  Pour indiquer que certaines tâches sont des sous-catégories d'autres tâches, sous l'onglet **Actions**, dans le groupe **Fonctions**, choisissez **Indenter tâches projet**.  

 Une ligne planification peut être de type :  

-   **Planifié** : ajouté au planning, mais non facturé.  
-   **Contrat** : facturé, mais non ajouté au planning.  
-   **Planifié et contrat** : facturé et ajouté au planning.  

 Dans cette procédure pas à pas, le chef de projet utilise le type **Planifié et contrat**. Il crée trois lignes planification pour la tâche 1010 et deux lignes planification pour la tâche 1020.  

### <a name="to-create-planning-lines"></a>Pour créer des lignes planification  

1.  Sélectionnez la ligne 1010, puis choisissez l'action **Lignes planification projet**. Entrez les informations suivantes :  

     **Ligne 1**  

    -   **Type ligne** : **Planifié et contrat**  
    -   **Date planification** : **(date du jour)**  
    -   **Type** : **Ressource**  
    -   **N°.**: **Tricia**  
    -   **Quantité** : **40**  

     **Ligne 2**  

    -   **Type ligne** : **Planifié et contrat**  
    -   **Date planification** : **(date du jour)**  
    -   **Type** : **Ressource**  
    -   **N°** : **Timothée**  
    -   **Quantité** : **40**  

     **Ligne 3**  

    -   **Type ligne** : **Planifié et contrat**  
    -   **Date planification** : **(date du jour)**  
    -   **Type**: **Compte du grand livre**  
    -   **N°** : **8430 (déplacement)**  
    -   **Quantité** : **2**  
    -   **Coût unitaire** : **400**  

2.  Cliquez sur le bouton **OK** pour fermer la fenêtre. Les totaux sont mis à jour dans la fenêtre **Lignes tâche projet**.  
3.  Sélectionnez la ligne 1020, puis choisissez l'action **Lignes planification projet**. Entrez les informations suivantes :  

     **Ligne 1**  

    -   **Type ligne** : **Planifié et contrat**  
    -   **Date planification** : **(date du jour)**  
    -   **Type** : **Ressource**  
    -   **N°.**: **Tricia**  
    -   **Quantité** : **80**  

     **Ligne 2**  

    -   **Type ligne** : **Planifié et contrat**  
    -   **Date planification** : **(date du jour)**  
    -   **Type** : **Article**  
    -   **N°** : **80201 (programme graphique)**  
    -   **Quantité** : **1**  

4.  Cliquez sur le bouton **OK** pour fermer la fenêtre. Les totaux sont mis à jour dans la fenêtre **Lignes tâche projet**.  

## <a name="calculating-remaining-usage"></a>Calcul de l'utilisation restante  
 Tricia, qui fait partie de l'équipe du projet, travaille depuis quelque temps sur le projet et souhaite enregistrer les heures et l'utilisation qu'elle y a consacrées. Elle n'a pas consacré plus de temps que ce qui avait été convenu à l'avance avec le client. Elle utilise le traitement par lots **Calc. activité restante** pour calculer l'activité restante pour le projet dans une feuille projet. Pour chaque tâche, le traitement en lot calcule la différence entre l'utilisation programmée des articles, des ressources et des dépenses générales et l'utilisation réelle reportée dans les écritures de grand livre projet. L'utilisation restante est ensuite affichée dans le journal projet à partir duquel elle peut la reporter.  

### <a name="to-calculate-remaining-usage"></a>Pour calculer l'utilisation restante  

1.  Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Feuilles projet**, puis sélectionnez le lien connexe.  
2.  Dans le champ **Nom feuille** de la fenêtre **Feuille projet**, ouvrez la liste **Noms feuilles projet**. Sélectionnez le nom de la feuille projet **Tricia**.  
3.  Choisissez l'action **Calc. utilisation restante**.  
4.  Dans la fenêtre **Projet - Calc. utilisation restante**, sous le raccourci **Tâche de projet**, dans le champ **N° projet**, sélectionnez le numéro de projet concerné (en général, J00010).  
5.  Sur le raccourci **Options**, tapez **J00001** dans le champ **N° document**. Cela facilite le suivi ultérieur du report.  
6.  Entrez la date du jour comme date de report.  
7.  Cliquez sur le bouton **OK**. Cela entraîne la génération des lignes journal projet dérivées des lignes planification créées par Prakash pour le projet.  
8.  Cliquez sur le bouton **OK** dans la fenêtre de confirmation. Les lignes générées sont ajoutées au journal projet.  
9. Assurez-vous que tous les numéros de document sont J00001, puis choisissez l'action **Reporter**. Cliquez sur **Oui** pour confirmer la validation.  
10. Les lignes sont à présent reportées. Cliquez sur le bouton **OK** pour fermer les fenêtres.  

## <a name="creating-and-posting-a-job-sales-invoice"></a>Création et report d'une facture vente projet  
 Ensuite, Tricia peut créer une facture pour l'ensemble du projet ou une partie du projet. Elle peut également joindre la facture à une autre destinée au même client pour le même projet. Dans ce cas, elle facture l'ensemble du projet, car celui-ci est à présent terminé.  

### <a name="to-create-a-job-sales-invoice"></a>Pour créer une facture vente projet  

1.  Choisissez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Projets**, puis choisissez le lien associé.  
2.  Sélectionnez le projet que vous avez créé précédemment, puis choisissez l'action **Créer une facture vente projet**.  
3.  Sous le raccourci **Tâche projet**, désactivez tout filtre associé à **N° tâche projet** pour facturer le projet. Sélectionnez le projet concerné dans le champ **N° de projet**.  
4.  Sur le raccourci **Options**, renseignez la date de validation et indiquez si vous souhaitez créer une facture par tâche ou une seule facture pour l'ensemble des tâches.  
5.  Cliquez sur le bouton **OK** pour créer la facture, puis cliquez sur le bouton **OK** dans la fenêtre de confirmation.  

 Une fois que Tricia a créé la facture, elle peut y accéder à partir de **Ventes et marketing** sous **Traitement des commandes** et en poursuivre le traitement.  

### <a name="to-post-a-new-sales-invoice"></a>Pour reporter une nouvelle facture vente  

1.  Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Factures vente**, puis sélectionnez le lien connexe.  
2.  Ouvrez la facture pour le client N°  01445544. Vous pouvez voir les informations entrées à partir des lignes planification.  
3.  Sélectionnez l'action **Valider**. Cliquez sur **Oui** pour confirmer la validation.  

### <a name="to-view-the-posted-invoice"></a>Pour afficher la facture reportée  

1.  Ouvrez le projet, puis choisissez l'action **Lignes planification projet**.  
2.  Sélectionnez l'une des lignes planification qui ont été facturées, puis choisissez l'action **Facture vente/Note de crédit**.
3. Dans la fenêtre **Factures projet**, choisissez l'action **Ouvrir la facture vente/la note de crédit**.  

 Tricia se pose une question concernant les prix, les coûts et les marges en relation avec ce projet particulier. Par conséquent, elle peut accéder à ces informations dans la fenêtre **Statistiques**.  

### <a name="to-open-the-statistics-window"></a>Pour ouvrir la fenêtre Statistiques  

1.  Choisissez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Projets**, puis choisissez le lien associé.  
2.  Sélectionnez l'action **Statistiques**. Vous pouvez consulter des informations détaillées sur les prix, les coûts et les profits d'un projet dans la devise locale et dans une devise étrangère.  
3.  Cliquez sur le bouton **Fermer** pour fermer la fenêtre **Statistiques projet**.  

## <a name="handling-fixed-prices"></a>Gestion de prix fixes  
 L'installation de salles de conférence a été confiée à CRONUS. En tant que chef de projet, Prakash souhaite disposer d'une bonne vue d'ensemble des tâches liées au projet ainsi que des coûts budgétisés et exposés associés à chacune d'elle. Il souhaite, en outre, connaître le prix total convenu pour le projet et les montants déjà facturés à ce stade. Il a conclu une entente avec le client concernant le prix fixe du projet.  

### <a name="to-manage-fixed-pricing-in-jobs"></a>Pour gérer un prix fixe dans des projets  

1.  Choisissez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Projets**, puis choisissez le lien associé.  
2.  Sélectionnez le numéro de projet **Guildford**, puis choisissez l'action **Lignes tâche projet**.  
3.  Sélectionnez la ligne 1120, puis, dans le champ **Programmé (coût total)**, cliquez avec le bouton droit sur le montant et sélectionnez **Détail**.  

     Les lignes planification projet permettent à Prakash de déterminer qu'il aura besoin de Tricia pendant 30 heures à ce stade du projet. Il convient d'un prix fixe avec le client.  

4.  Dans la fenêtre **Lignes tâche projet**, sélectionnez la ligne 1120, puis choisissez l'action **Lignes planification projet**.  
5.  Choisissez **Nouveau** pour créer une ligne avec les informations suivantes :  

    -   **Type ligne** : **Planifié et contrat**  
    -   **Type** : **Ressource**  
    -   **N°.**: **Tricia**  
    -   **Quantité** : **30**  

7.  Cliquez sur le bouton **OK** pour fermer la fenêtre.  
8.  Dans le champ **Programmé (coût total)**, cliquez avec le bouton droit sur le champ, puis choisissez de nouveau **Détail** dans la fenêtre **Lignes tâche projet**. Affichez les modifications apportées au calendrier. Vous pouvez voir que 30 heures ont été ajoutées au calendrier.  
9. Cliquez sur le bouton **OK** pour fermer les fenêtres.  

 Une fois Tricia ajoutée au calendrier pour cette ligne tâche, celle-ci va consacrer 25 heures au projet. Elle entre ces heures dans le journal projet.  

### <a name="to-enter-hours-in-the-job-journal"></a>Pour entrer des heures dans le journal projet  

1.  Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Feuilles projet**, puis sélectionnez le lien connexe.  
2.  Dans une nouvelle ligne, entrez les informations suivantes :  

    -   **Type ligne** : **(vide)**  
    -   **Date de report** : **(date du jour)**  
    -   **N° document** : **J00002**  
    -   **N° projet** : **Guildford**  
    -   **N° tâche projet** : **1120**  
    -   **Type** : **Ressource**  
    -   **N°.**: **Tricia**  
    -   **Quantité** : **25**  

3.  Sélectionnez l'action **Valider**.  

     Quelques jours plus tard, Tricia consacre 10 heures supplémentaires au projet. Elle a désormais presté un total de 35 heures. Comme l'entente porte sur 30 heures de prestation avec le client, seules 5 heures lui seront facturées. Tricia ajoutera manuellement au calendrier les cinq heures de travail supplémentaires qu'elle a effectuées.  

4.  Dans la fenêtre **Journal projet**, choisissez l'action **Calc. utilisation restante**.  
5.  Dans la fenêtre **Projet Calc. activité restante**, entrez les informations suivantes dans le raccourci **Options** :  

    -   **N° document** : **J00003**  
    -   **Date de report** : **(date du jour)**  

6.  Entrez les informations suivantes sur le raccourci **Tâche projet** :  

    -   **N° projet** : **Guildford**  
    -   **N° tâche projet** : **1120**  

     Pour exécuter le calcul, cliquez sur le bouton **OK**. Il reste cinq heures de travail à Tricia. Le champ **Type ligne** est vide, ce qui indique que seule l'activité reste à valider parce que le travail a déjà été planifié.  

7.  Dans la fenêtre **Feuille projet**, créez une ligne avec les informations suivantes. Assurez-vous que les numéros de projet suivent ceux que vous avez déjà utilisés :  

    -   **Type ligne** : **Planifié**  
    -   **N° projet** : **Guildford**  
    -   **N° tâche projet** : **1120**  
    -   **Type** : **Ressource**  
    -   **N°.**: **Tricia**  
    -   **Quantité** : **5**  

     En utilisant **Planifié** comme type de ligne, des mises à jour doivent être apportées aux coûts et aux prix prévus, mais aucune mise à jour des coûts et du prix contractuels facturés au client n'est nécessaire.  

8.  Sélectionnez l'action **Valider**. Cliquez sur le bouton **OK** pour fermer la fenêtre.  
9. Ouvrez la liste **Projets**.  
10. Sélectionnez le projet GUILDFORD, puis choisissez l'action **Lignes tâche projet**.  
11. Sélectionnez la ligne 1120, puis, dans le champ **Programmé (coût total)**, cliquez avec le bouton droit sur le montant. Choisissez **Détail** pour afficher les informations.  

     Les modifications sont automatiquement entrées dans la ligne de la tâche projet n° 1120. Dans le coût total du travail programmé, les cinq heures de travail supplémentaires effectuées par Tricia ont été ajoutées au calendrier.  

12. Sélectionnez le bouton **Fermer** pour fermer la fenêtre.  
13. Choisissez avec le bouton droit le montant indiqué dans le champ **Contrat (coût total)**, puis sélectionnez **Détail** pour afficher les informations.  

     Dans le prix total du contrat, seules les 30 heures contractuelles d'origine sont incluses car c'est ce qui a été convenu avec le client.  

## <a name="copying-jobs"></a>Copie de projets  
 Prakash a conclu une entente avec un client, Selagorian Ltd, pour l'installation de 10 salles de conférence. Cette entente est similaire à un projet antérieur. Il gagnera par conséquent du temps en copiant ce projet antérieur.  

 Dans la fenêtre **Copier projet**, vous pouvez sélectionner le projet et les lignes tâche à copier. Vous pouvez également choisir de copier les écriture de grand livre projet origine, ce qui a pour effet de créer des lignes planification basées sur une utilisation réelle, ou copier les lignes planification du projet origine, ce qui a pour effet de copier les lignes planification initiales dans le nouveau projet. Vous pouvez ensuite choisir la ligne planification ou le type de ligne écriture à inclure en ne sélectionnant que ce qui convient pour ce nouveau projet. Enfin, vous pouvez sélectionner le projet dans lequel vous voulez copier, puis définir si les prix et quantités doivent également être copiés.  

### <a name="to-copy-a-job"></a>Pour copier un projet  

1.  Choisissez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Projets**, puis choisissez le lien associé.  
2.  Choisissez l'action **Nouveau** pour créer un projet. Entrez les informations suivantes :  

    -   **Description** : **Installation de 10 salles de conférence**  
    -   **N° client facturé** : **20000**  

3.  Choisissez l'action **Copier tâches projet à partir de**.  
4.  Dans la fenêtre **Copier les tâches projet**, entrez les informations suivantes :  

    -   **N° projet** : **Guildford**  
    -   **N° tâche projet de** : **1000**  
    -   **Source** : **Lignes planning projet**  
    -   **Type lignes planification à inclure** : **Calendrier+Contrat**  
    -   **Nº projet** : **Guildford Installation de 10 salles de conférence**  
    -   Sélectionnez les champs **Copier axes** et **Copier quantité**.  

5.  Cliquez sur le bouton **OK** pour copier le projet, puis cliquez sur le bouton **OK** pour fermer la fenêtre de confirmation.  

     Si vous comparez les prix, les lignes tâche projet et les lignes planification projet des deux projets, vous pouvez constater que la copie des informations a réussi.  

## <a name="making-payments-by-installments"></a>Paiements en plusieurs versements  
 CRONUS vient de décrocher un nouveau projet dont la réalisation prendra une année. Comme ce projet mobilisera un grand nombre de ressources, le chef de projet établit le contrat de sorte que le client paie une partie du prix à la commande, une autre lorsqu'il sera à moitié accompli et le solde à la livraison.  

### <a name="to-set-up-a-new-account"></a>Pour configurer un nouveau compte  

1.  Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Plan comptable**, puis sélectionnez le lien connexe.  
2.  Dans la fenêtre **Plan comptable**, choisissez l'action **Nouveau** pour créer une fiche.  
3.  Dans la fiche **Nouveau compte du grand livre**, entrez les informations suivantes :  

    -   **N°** : **6630**  
    -   **Nom** : **Paiement du projet**  

4.  Sur le raccourci **Validation**, dans le champ **Groupe compta. produit**, sélectionnez **DIVERS**. Cliquez sur le bouton **OK** pour fermer la fenêtre.  
5.  Dans la fenêtre **Plan comptable**, sélectionnez **Paiement du projet n°6630**, puis choisissez l'action **Décaler plan comptable**. Choisissez **Oui** pour confirmer.  

 Les procédures suivantes expliquent comment créer un projet, définir un prix et configurer un paiement en plusieurs versements. Dans les lignes tâche projet, vous pouvez créer des lignes spécifiques dédiées au paiement en plusieurs versements. Tout le travail consacré au projet ajouté au calendrier sera entré dans les lignes utilisation. Pour chaque ligne tâche paiement sur les lignes planification, le type de ligne est Contrat, ce qui signifie que le client sera facturé. Entrez une nouvelle ligne pour l'acompte. Dans la ligne tâche utilisation, vous pouvez entrer les informations relatives aux articles et ressources utilisés dans ce projet, qui allongeront le calendrier, telles que les heures de travail des employés et les articles consommés pour le projet.  

### <a name="to-make-a-payment-by-installment"></a>Pour créer un paiement en plusieurs versements  

1.  Créez un projet.  
2.  Dans la nouvelle fiche **Projet**, entrez les informations suivantes :  

    -   **Description** : **Redécoration de la réception**  
    -   **N° client facturé** : **30000**  
    -   **Groupe compta. projet** : **Installation**  
    -   **Méthode TEC** : **Valeur de coût**  

3.  Sur la fiche projet, choisissez l'action **Ressource**. Entrez les informations suivantes :  

    -   **Code** : **Tricia**  
    -   **Prix unitaire** : **10**  

     Cliquez sur le bouton **OK** pour fermer la fenêtre.  

4.  Sur la fiche **Projet**, choisissez l'action **Lignes tâche projet**.  

     Le tableau suivant décrit les lignes que vous allez créer.  

    |Ligne|N° tâche projet|Description|Type tâche projet|  
    |----------|------------------|---------------------------------------|-------------------|  
    |1|1000|Paiement – Acompte|Report|  
    |2|2000|Utilisation|Report|  
    |3|3000|Paiement – À mi-parcours|Report|  
    |4|4000|Paiement – À la livraison|Report|  

5.  Dans la fenêtre **Lignes tâche projet**, sélectionnez la tâche 1000, puis choisissez l'action **Lignes planification projet**.  
6.  Créez une ligne planification avec les informations suivantes :  

    -   **Type ligne** : **Contrat**  
    -   **Date planification** : **(date du jour)**  
    -   **Type**: **Compte du grand livre**  
    -   **N°** : **6630**  
    -   **Quantité** : **1**  
    -   **Prix unitaire** : **5000**  

     Cliquez sur le bouton **OK** pour fermer la fenêtre.  

7.  Dans la fenêtre **Lignes tâche projet**, sélectionnez la **tâche 2000** et ouvrez les **Lignes planning projet** correspondantes.  

     Le tableau suivant décrit les lignes planification que vous allez créer.  

    |Ligne|Type ligne|Date planification|Type|N°|Quantité|  
    |----------|---------------|-------------------|----------|---------|--------------|  
    |1|Calendrier|(date du jour)|Ressource|Tricia|120|  
    |2|Calendrier|(date du jour)|Article|70104|10|  

     Cliquez sur le bouton **OK** pour fermer la fenêtre. Dans la fenêtre **Lignes tâche projet**, vous pouvez voir que les montants planifiés ont été mis à jour.  

8.  Dans la fenêtre **Lignes tâche projet**, sélectionnez la **tâche 3000**.  
9. Créez une ligne planification avec les informations suivantes :  

    -   **Type ligne** : **Contrat**  
    -   **Date planning** : **à une date ultérieure**  
    -   **Type**: **Compte du grand livre**  
    -   **N°** : **6630**  
    -   **Quantité** : **1**  
    -   **Prix unitaire** : **5000**  

     Cliquez sur le bouton **OK** pour fermer la fenêtre.  

10. Créez une écriture de ligne planification similaire pour la tâche projet 4000.  

 Une fois les lignes tâche et planification entrées, Prakash crée une facture pour le premier paiement. Il le fait à partir des lignes tâche projet pour être certain que la facture ne contienne que les lignes relatives au premier paiement. Vous pouvez ouvrir le document de vente à partir des lignes planification ou des lignes tâche.  

### <a name="to-create-an-invoice"></a>Pour créer une facture  

1.  Dans la fenêtre **Lignes tâche projet**, sélectionnez la ligne 1000, puis choisissez l'action **Créer facture vente**.  
2.  Dans la fenêtre **Créer facture vente**, indiquez la date du jour comme date de validation, spécifiez **Par tâche**, puis cliquez sur le bouton **OK** pour créer une facture avec les informations par défaut. Cliquez sur le bouton **OK** pour fermez la fenêtre de confirmation.  
3.  Choisissez l'action **Facture vente/note de crédit**. Sur la facture vente, vous pouvez voir que seul l'acompte est inclus dans la facture. Vous pouvez à présent envoyer cette dernière au client comme convenu.  

## <a name="next-steps"></a>Étapes suivantes  
 Cette procédure pas à pas vous a présenté l'utilisation de base des projets dans [!INCLUDE[d365fin](includes/d365fin_md.md)]. Vous avez appris à créer un projet, à copier un projet et à gérer les paiements. Vous avez également vu comment assurer le suivi des heures et créer des factures.  

## <a name="see-also"></a>Voir aussi  
 [Procédures pas à pas liées au processus entreprise](walkthrough-business-process-walkthroughs.md)   
 [Configuration de la gestion de projet](projects-setup-projects.md)   
 [Procédure : utiliser des ressources](projects-how-use-resources.md)   
 [Procédure : surveiller la progression et les performances](projects-how-monitor-progress-performance.md)   
 [Procédure : facturer des projets](projects-how-invoice-jobs.md)  
 [Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

