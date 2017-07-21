---
title: Configuration des axes analytiques
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 18237c4b755926222a36bc97dec5d6783c11454d
ms.contentlocale: fr-ca
ms.lasthandoff: 06/26/2017

---

# <a name="set-up-dimensions"></a>Configuration des axes analytiques
Vous devez définir les dimensions et les valeurs de dimension que vous souhaitez utiliser dans votre compagnie. Vous devez également définir les axes analytiques que vous souhaitez utiliser comme axes principaux et comme raccourcis axe. Prenez soin de définir attentivement les dimensions qui seront les plus efficaces en tant que dimensions principales et raccourcis de dimension pour votre compagnie.  
Paramétrez tous les différents axes dont vous souhaitez effectuer le suivi dans la fenêtre **Axes analytiques**. La fenêtre Axes analytiques contient une ligne pour chaque axe, tel que *Projet*, *Département*, *Zone* et *Commercial*.  

Pour chaque dimension, vous devez également configurer les valeurs de dimension, par exemple, tous les départements de votre compagnie. Les sections analytiques peuvent être paramétrées sous forme de structure hiérarchique similaire au plan comptable, de manière à ce que les données puissent être réparties en plusieurs niveaux de granularité et à ce que des sous-ensembles de sections analytiques puissent être totalisés.  

Vous pouvez définir deux axes principaux qui seront automatiquement disponibles partout, par exemple dans les états et les traitements par lots. Vous pouvez également définir six raccourcis dimension supplémentaires qui seront disponibles sous forme de champ dans les lignes journal et document. Pour utiliser les axes restants, vous pouvez y accéder via une fenêtre séparée qui affiche les axes pour la ligne.  

Vous pouvez définir autant de dimensions que nécessaire pour votre compagnie et également un nombre illimité de valeurs de dimension pour chaque dimension. Vous pouvez utiliser tous les axes analytiques que vous avez définis dans les écritures des feuilles et des documents, ainsi que dans les états et les traitements par lots liés aux axes analytiques.  

## <a name="set-up-default-dimensions-for-customers-vendors-and-other-accounts"></a>Configuration des axes analytiques par défaut pour les clients, les fournisseurs, et les autres comptes
Vous pouvez configurer une dimension par défaut pour un compte spécifique. Ce code est ensuite copié dans le journal ou le document lorsque le champ du numéro du compte est renseigné sur la ligne. Toutefois, vous pouvez supprimer ou modifier le code si nécessaire. Vous pouvez également rendre une dimension obligatoire afin qu'il soit impossible de reporter une écriture avec un type de compte spécifique sauf si une valeur de dimension lui est affectée.  

En outre, vous pouvez configurer une dimension par défaut pour chaque type de compte de sorte que ce code soit copié vers le journal ou le document lorsque le type de compte est renseigné sur la ligne. Cependant, vous pouvez toujours modifier le code dans le document si nécessaire.  

Enfin, vous pouvez également rendre une dimension obligatoire afin qu'il soit impossible de reporter une écriture avec un type de compte spécifique sauf si une valeur de dimension lui est affectée.

## <a name="see-also"></a>Voir aussi
[Axes analytiques](finance-setup-dimensions.md)  
[Configurer les processus financiers de base](finance-setup-setup-finance-setup.md)

