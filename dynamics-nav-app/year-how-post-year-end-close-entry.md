---
title: "Procédure : Reporter une écriture de fermeture de fin d'exercice"
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: a8fdb459a2b98066bb93bb47cc0bd9721b992d94
ms.contentlocale: fr-ca
ms.lasthandoff: 06/26/2017

---
# <a name="how-to-post-year-end-closing-entry"></a>Procédure : Reporter une écriture de fermeture de fin d'exercice
Dans le cadre de la fermeture des registres pour un exercice financier, vous allez exécuter le traitement en lot Fermer l'état des résultats pour transférer le résultat annuel vers un compte de bilan et fermer les comptes d'état des résultats. Après avoir utilisé le traitement en lot Fermer l'état des résultats, vous devez ouvrir le journal spécifié dans le traitement en lot, puis consulter et reporter les écritures.

## <a name="to-post-the-year-end-closing-entry"></a>Pour reporter l'écriture de fermeture de fin d'exercice
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Feuille comptabilité**, puis sélectionnez le lien connexe.
2. Dans la fenêtre **Feuille comptabilité**, dans le champ **Nom de la feuille**, sélectionnez la feuille qui contient les écritures de clôture.
3. Examinez les écritures.
4. Pour valider la feuille, sélectionnez l'action **Valider**.

**Remarque** : en cas de détection d'une erreur, un message d'erreur s'affiche. Si le report réussit, les entrées reportées sont supprimées du journal. Une fois le report terminé, une entrée est reportée sur chaque compte état des résultats, de façon à ce que son solde indique zéro et à ce que les résultats de l'exercice soient transférés dans le bilan.

## <a name="see-also"></a>Voir aussi
[Clôture des livres](year-close-books.md)  
[Clôturer exercice comptable](year-close-income-statement.md)  
[Procédure : clôture des périodes comptables](year-close-account-periods.md)  
