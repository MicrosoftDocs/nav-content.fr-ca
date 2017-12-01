---
title: "Procédure : reporter les coûts inventaire dans le grand livre"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 34eec596392e9316e807d3c073c3b8e59dbc12e9
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---

# <a name="how-to-post-inventory-costs-to-the-general-ledger"></a>Procédure : reporter les coûts inventaire dans le grand livre   
Lorsque vous reportez des transactions d'inventaire, telles que des livraisons vente, des factures achat ou des ajustements d'inventaire, les quantités et les coûts modifiés sont enregistrés respectivement dans les écritures article et les écritures valeur. Pour refléter ces modifications de la valeur inventaire dans vos registres financiers, vous devez reporter les coûts inventaire sur les comptes inventaire associés dans le grand livre.

Vous pouvez reporter les coûts inventaire dans le grand livre de deux manières :

- automatiquement, de sorte que les coûts inventaire soient reportés dans le grand livre chaque fois que vous reportez une transaction inventaire ;
- manuellement, de sorte que les coûts inventaire soient uniquement reportés dans le grand livre lorsque vous exécutez un traitement en lot.


## <a name="to-post-inventory-costs-automatically"></a>Pour reporter des coûts de l'inventaire automatiquement
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Paramètres stock**, puis sélectionnez le lien connexe.
2. Dans la fenêtre **Paramètres stock**, cochez la case **Compta. coûts automatique**.

Pour chaque transaction inventaire que vous reportez, les valeurs appropriées sont reportées dans le compte inventaire, le compte ajustement et le compte variation inventaire dans le grand livre.

Même si vous utilisez le report automatique des coûts, vous devez continuer à exécuter périodiquement le traitement en lot Ajuster coûts : Écr. article pour vous assurer que les coûts des produits sont transmis aux transactions sortantes appropriées, telles que les ventes ou les transferts. Cela est particulièrement important dans les situations où vous vendez des biens avant de facturer leur achat.

Si une erreur se produit dans la configuration de dimension lors du report des coûts inventaire dans le grand livre, le report se termine par une erreur.

## <a name="to-post-inventory-costs-manually"></a>Pour reporter des coûts de l'inventaire manuellement
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Valider coûts ajustés**, puis sélectionnez le lien connexe.
2. Reportez les coûts inventaire dans le grand livre manuellement en exécutant le traitement en lot. Lorsque vous exécutez ce traitement en lot, des écritures sont créées, basées sur des écritures valeur. Vous pouvez reporter les écritures de façon à ce qu'elles soient récapitulées par groupe de report.

**Remarque** : lorsque vous exécutez ce traitement par lots, il se peut que vous rencontriez des erreurs en relation avec une configuration manquante ou une configuration d'axe analytique incompatible. Si le traitement en lot détecte des erreurs dans la configuration de dimension, il les ignore et utilise les dimensions de l'écriture valeur. Pour toute autre erreur, le traitement en lot ignore le report des écritures valeur et les répertorie à la fin du rapport dans la section intitulée « Écritures ignorées ». Pour reporter ces écritures, vous devez corriger les erreurs.

Pour afficher la liste des erreurs avant d'exécuter le traitement par lot de validation, vous pouvez générer l'état **Valider coûts ajust. - Test**. Le rapport de test répertorie toutes les erreurs détectées durant le test de report. Vous pouvez ensuite corriger les erreurs et exécuter le traitement en lot de report des coûts inventaire sans ignorer aucune entrée.

Si vous voulez simplement afficher un aperçu des valeurs qui pourraient être reportées dans le grand livre sans réellement effectuer le report, vous pouvez exécuter le traitement en lot Reporter le coût de l'inventaire au grand livre sans réellement reporter les valeurs dans le grand livre. Pour ce faire, désactivez le champ Reporter sur la page de demande. De cette manière, lorsque vous exécutez le traitement en lot, le rapport est produit, indiquant les valeurs prêtes pour report dans le grand livre, mais elles ne sont pas reportées.

## <a name="see-also"></a>Voir aussi
[Gestion du stock](inventory-manage-inventory.md)    
[Procédure : ajustement des coûts article](inventory-how-adjust-item-costs.md)  
[Gestion des ventes](sales-manage-sales.md)  
[Gestion des achats](purchasing-manage-purchasing.md)

