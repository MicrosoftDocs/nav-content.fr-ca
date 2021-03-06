---
title: "Aperçu des configuration des articles de service et des composantes article de service"
description: "Découvrez les éléments que vous devez configurer avant de pouvoir utiliser des articles de service, notamment les valeurs par défaut telles que le délai de réponse, le pourcentage escompte de paiement contrat et le groupe tarifs service."
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
ms.openlocfilehash: 0632bdc3b12e60c9b49893df748e8ca165c5b9d4
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-service-items-and-service-item-components"></a>Procédure : configurer les articles de service et les composantes article de service
Pour utiliser les articles de service, vous devez configurer

* les groupes articles de service suivants. 
* En option

## <a name="to-set-up-service-item-groups"></a>Pour configurer des groupes articles de service
Vous pouvez configurer des groupes d'articles associés en termes de réparation et d'entretien. Vous pouvez définir des valeurs par défaut des articles de service d'un groupe articles de service, telles que le délai de réponse, le pourcentage escompte du contrat et le groupe tarifs service. Dans le cas d'articles appartenant à un groupe articles de service, ceux-ci peuvent être, à votre demande, enregistrés automatiquement en tant qu'articles de service lorsqu'ils sont vendus.  
  
Vous pouvez affecter des groupes articles de service à des articles sur la fiche **Article** et à des articles de service sur la fiche **Article de service**.  
  
1. Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Groupes d'articles de service**, puis sélectionnez le lien associé.  
2. Créez un groupe articles de service.  
3. Renseignez les champs **Code** et **Désignation**.  
4. Dans le champ **% remise contrat par défaut**, saisissez le pourcentage remise contrat par défaut que vous souhaitez attribuer aux articles de service du groupe.  
5. Dans le champ **Code gpe tarifs serv. par déf**, saisissez le code groupe tarifs service par défaut à attribuer aux articles de service du groupe.  
6. Dans le champ **Délai de réponse par déf. (heures)**, saisissez le délai de réponse par défaut (en heures) que vous souhaitez attribuer aux articles de service du groupe.  
7. Sélectionnez le champ **Créer article de service** si vous souhaitez enregistrer les articles du groupe en tant qu'articles de service lorsqu'ils sont vendus.  

## <a name="to-set-up-service-item-components"></a>Pour configurer des composants article de service
Un article de service peut être constitué de plusieurs composants pouvant être remplacés par des pièces de rechange lors de la maintenance de l'article. Vous pouvez configurer ces composantes sur la page **Liste composantes art. service**. En outre, si vous souhaitez configurer des composantes pour des articles de service qui sont des nomenclatures, vous pouvez copier les articles de nomenclature et les créer en tant que composantes article de service. 
  
1. Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Articles de service**, puis sélectionnez le lien associé. 
2. Ouvrez l'article de service pour lequel vous voulez configurer des composants.  
3. Sélectionnez l'action **Composantes**. La fenêtre **Liste composants art. service** s'ouvre.  
4. Ajouter une nouvelle composante.  
5. Dans le champ **Type**, choisissez **Article de service** si la composante proprement dite est un article de service enregistré. Sinon, choisissez **Article**.  
6. Dans le champ **N°**, choisissez l'article ou l'article de service qui est une composante de l'article de service.  

## <a name="to-set-up-service-item-components-from-a-bom"></a>Pour configurer des composants article de service à partir de nomenclatures
1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Articles de service**, puis sélectionnez le lien associé.  
2. Ouvrez l'article de service pour lequel vous voulez configurer des composants à partir d'une nomenclature.  
3. Sélectionnez l'action **Composantes**. La fenêtre **Liste composants art. service** s'ouvre.  
4. Choisissez l'action **Copier à partir de nomenclature**.  
  
    Si l'article auquel est lié l'article de service est une nomenclature, les composants pour tous les articles de la nomenclature sont créés automatiquement.  

## <a name="to-set-up-a-service-shelf"></a>Pour configurer une tablette service
Vous pouvez configurer des tablettes de service qui identifient l'emplacement de stockage de vos articles de service. Vous pouvez affecter des tablettes de service à des articles de service dans les pages **Commande service** et **Feuille activité article de service**.  
  
1. Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Tablettes service**, puis sélectionnez le lien associé.
2. Renseignez les champs selon vos besoins.

## <a name="see-also"></a>Voir aussi
[Procédure : configurer des codes prestations standard](service-how-setup-service-coding.md)   
[Procédure : configurer le dépannage](service-how-setup-troubleshooting.md)
