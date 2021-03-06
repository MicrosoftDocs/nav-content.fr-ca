---
title: "Comment utiliser les clés de ventilation dans les feuilles de comptabilité "
description: "En savoir plus sur l'utilisation des clés de ventilation dans les feuilles."
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cost accounting
ms.date: 03/29/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 3d3944d5f7e9bfe5390fd63b2ae1d05f62efab49
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-use-allocation-keys-in-general-journals"></a>Comment utiliser les clés de ventilation dans les feuilles de comptabilité
Vous pouvez ventiler une écriture dans un journal général dans différents comptes lorsque vous reportez le journal. L'affectation peut être effectuée par quantité, pourcentage ou montant.

## <a name="to-set-up-allocation-keys"></a>Pour définir des clés de ventilation
1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Feuille abonnement**, puis sélectionnez le lien connexe.
2. Sélectionnez le champ **Nom de la feuille** pour ouvrir la fenêtre **Noms feuilles comptabilité**.
3. Vous pouvez soit modifier les ventilations sur un lot existant dans la liste ou créer un lot avec des ventilations.
   * Pour créer un lot, sélectionnez l'action **Nouveau**, et passez à l'étape suivante.
   * Pour modifier les affectations à partir d'un journal existant, sélectionnez le journal et passez à l'étape 7.    
4. Dans le champ **Nom**, saisissez le nom du lot, par exemple NETTOYAGE. Dans le champ **Description**, saisissez une description, par exemple Feuille frais de nettoyage.
5. Fermez la fenêtre lorsque vous avez terminé. Un nouveau journal récurrent vide s'ouvre.
6. Renseignez les champs de la ligne.
7. Sélectionnez l'action **Ventilations**.
8. Ajoutez une ligne pour chaque affectation. Vous devez renseigner le champ **% ventilation**, **Quantité imputée** ou **Montant**. Vous devez également renseigner le champ **N° compte** et, si vous affectez la transaction à des dimensions principales, les champs de ces dimensions principales.
9. Si vous saisissez un pourcentage dans une ligne, le montant du champ **Montant** est calculé automatiquement. Ces montants sont dotés du signe opposé à celui du montant total figurant dans le champ **Montant** de la feuille récurrente.
10. Après avoir saisi les lignes de ventilation, cliquez sur **OK** pour revenir à la fenêtre **Feuille abonnement**. Le champ **Montant imputé DS** est renseigné et correspond au champ **Montant**.
11. Reportez le journal.

## <a name="to-change-an-allocation-key-that-has-already-been-set-up"></a>Pour modifier une clé d'affectation déjà configurée
1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Feuille abonnement**, puis sélectionnez le lien connexe.
2. Dans la fenêtre **Feuille récurrente**, sélectionnez la feuille contenant la ventilation.
3. Sélectionnez la ligne de la ventilation, puis sélectionnez l'action **Ventilations**.
4. Modifiez les champs appropriés, puis cliquez sur le bouton **OK**.

## <a name="see-also"></a>Voir aussi
[Utilisation de feuilles comptabilité](ui-work-general-journals.md)  
[Validation des documents et des feuilles](ui-post-documents-journals.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

