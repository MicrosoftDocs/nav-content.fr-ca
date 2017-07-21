---
title: "Créer des séries de numéros"
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 22b3bcf71c99e106527d6bfa35478045d29b9629
ms.contentlocale: fr-ca
ms.lasthandoff: 06/26/2017

---

# <a name="create-number-series"></a>Créer des séries de numéros

Pour chaque compagnie que vous configurez, vous devez affecter des codes d'identification uniques aux éléments tels que les comptes du grand livre, les comptes client et fournisseur, les factures et les documents. La numérotation est importante, pas uniquement pour l'identification. Un système de numérotation bien conçu facilite également la gestion et l'analyse de la compagnie et permet de réduire les erreurs de saisie des données.

Vous pouvez configurer un système de numérotation complet avec un nombre illimité de séries de numéros. Vous pouvez utiliser des séries de numéros pour tous les types de documents et journaux, ainsi que pour les données de base, telles que les clients, les articles et les projets.

Vous pouvez combiner l'utilisation des séries de numéros et la numérotation manuelle.

Vous créez un système de numérotation en définissant un ou plusieurs codes pour chaque type de données de base ou de document. Par exemple, vous pouvez définir un code pour la numérotation de clients, un code pour la numérotation des factures vente et un autre code pour la numérotation des documents dans les feuilles comptabilité.

Une fois que vous avez défini un code, vous devez définir au moins une ligne série de numéros. La ligne série de numéros contient des informations telles que les premier et dernier numéros de la série et la date début. Vous pouvez définir plusieurs lignes série de numéros par code série de numéros, avec une date début différente pour chaque ligne. Les séries sont utilisées de manière consécutive, chaque série commençant à la date début respective.

Si vous voulez utiliser plusieurs codes série de numéros pour un type de données de base (par exemple, si vous voulez utiliser différentes séries de numéros pour diverses catégories d'articles), vous pouvez utiliser des liens de séries de numéros.

Outre les numéros affectés manuellement ou à l'aide du système de numérotation, toutes les transactions (écritures) se voient automatiquement affecter des numéros consécutifs. Ces numéros s'affichent dans le champ **N° écriture** de toutes les fenêtres écritures. Vous ne pouvez pas les modifier ni les supprimer.

## <a name="to-create-relationships-between-number-series"></a>Pour créer des liens entre des séries de numéros
Si vous avez défini plusieurs codes série de numéros pour un même type d'informations ou de transactions de base, vous pouvez créer des liens entre ces codes. Cette fonction peut vous aider à choisir parmi ces codes lorsque vous utilisez un numéro.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Souches de n°**, puis sélectionnez le lien connexe.
2. Sélectionnez la ligne avec la souche de numéros pour laquelle vous souhaitez créer des relations, puis cliquez sur **Relations**.
3. Dans le champ **Code souche**, entrez le code de la souche de numéros à lier à la souche sélectionnée à l'étape 2.
4. Ajoutez une ligne pour chaque code à lier à la série de numéros sélectionnée.
5. Fermez la fenêtre.

Désormais, pour créer un élément nécessitant un numéro, vous pourrez utiliser les liens ainsi créés et choisir parmi les séries de numéros liées.

## <a name="see-also"></a>Voir aussi
[Utiliser Dynamics NAV](ui-work-product.md)

