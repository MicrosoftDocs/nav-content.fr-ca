---
title: "Acheter des articles ou des services pour un projet et gérer les fournitures"
description: "Décrit comment gérer l'approvisionnement et l'achat de matériel et de services pour les projets."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, material, purchase
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 3405af0c06df0fb04c528cf114d4ef6326f7c0a9
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-manage-job-supplies"></a>Procédure : Gérer les fournitures pour un projet
La gestion des fournitures des projets relatifs à des articles, services et dépenses est l'un des aspects essentiels de l'exécution d'un projet. Vous pouvez utiliser les quantités en inventaire ou effectuer des achats spécifiques au projet en utilisant des bons de commande ou des factures achat. Par exemple, un projet de service sur un ordinateur requiert un nouveau disque. Vous devez donc créer une facture achat pour l'acheter et pour enregistrer le projet pour lequel il sera utilisé.

Si le processus d'achat ne requiert pas d'enregistrement séparé de la transaction physique, un achat peut être traité dans la fenêtre **Feuille compta. projet**. Pour plus d'informations, reportez-vous à [Procédure : Enregistrer l'utilisation pour les projets](projects-how-record-job-usage.md).

## <a name="to-purchase-items-or-services-for-a-job"></a>Pour acheter des articles ou des services pour un projet
La procédure suivante indique comment utiliser une facture achat pour acheter des produits pour un projet. Les mêmes phases s'appliquent lors de l'utilisation d'un bon de commande.  

1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Factures achat**, puis sélectionnez le lien connexe.  
2. Sélectionnez l'action **Nouveau**, puis renseignez les champs selon vos besoins. Pour plus d'informations, reportez-vous à [Procédure : enregistrer des achats](purchasing-how-record-purchases.md).
3. Dans les champs **N° projet** et **N° tâche projet**, sélectionnez les informations du projet pour lequel vous souhaitez acheter des articles ou des services. Utilisez la fonction **Choisir les colonnes** si le champ n'est pas visible. Pour plus d'informations, voir [Personnalisation utilisateur](ui-user-personalization.md).

    La valeur que vous sélectionnez dans le champ **Type ligne projet** définit si une ligne planning est créée lorsque vous validez l'activité de l'article. Si le champ indique **Facturable**, les lignes planning projet prêtes pour facturation sont créées. Pour plus d'informations, reportez-vous à [Procédure : Facturer des projets](projects-how-invoice-jobs.md).
4. Sélectionnez l'action **Valider**.

## <a name="to-view-the-value-of-purchases-for-a-job"></a>Pour afficher la valeur des achats pour un projet
1. Choisissez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Projets**, puis choisissez le lien associé.
2. Ouvrez la fiche projet appropriée.

    Dans le raccourci **Tâches**, le champ **Commandes ouvertes** affiche le montant total en commande, en devise société, des articles en stock et des services sur les documents achat pour la tâche projet ligne.  

    Le champ **Montant reçu non facturé** affiche la valeur des articles livrés sur les documents achat mais non facturés.  
3. Choisissez l'un des champs pour ouvrir la fenêtre **Lignes achat** dans laquelle vous pouvez consulter des informations sur les lignes de document achat associées, incluant les articles ou les services qui ont été réceptionnés.

## <a name="to-post-a-job-related-expense"></a>Pour reporter des frais liés à un projet
Si vous supportez les dépenses extraordinaires ou exceptionnelles du projet, vous pouvez utiliser la fenêtre **Feuille compta. projet** pour les valider directement dans le compte projet approprié.

1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Feuilles compta. projet**, puis sélectionnez le lien connexe.  
2. Créez une ligne et renseignez les informations concernant les frais, notamment les informations dans les champs **N° projet** et **N° tâche projet**.  
3. Lorsque la feuille est renseignée, cliquez sur **Valider**.

## <a name="see-also"></a>Voir aussi
[Gestion de projets](projects-manage-projects.md)  
[Finances](finance.md)  
[Achats](purchasing-manage-purchasing.md)         
[Ventes](sales-manage-sales.md)      
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

