---
title: "Procédure : configurer un amortissement immobilisation"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 7efc50c673514498de0caa5b3a2dc4b32d4f7f5d
ms.contentlocale: fr-ca
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-fixed-asset-depreciation"></a>Procédure : configurer un amortissement immobilisation
 Vous pouvez utiliser plusieurs méthodes d'amortissement pour préparer les états financiers et les déclarations de revenus. De nombreuses compagnies de grande taille utilisent la méthode de l'amortissement linéaire dans leurs rapports financiers car elle permet généralement la déclaration des bénéfices supérieurs. Toutefois, dans le cadre de l'impôt sur le revenu, la plupart des entreprises utilise une méthode d'amortissement accélérée. Pour en savoir plus, voir [Méthodes d'amortissement](fa-depreciation-methods.md).

 Lorsque vous avez créé les lois d'amortissement nécessaires, vous devez en attribuer au moins une à chaque immobilisation. Un registre amortissement attribué à une immobilisation est désigné comme registre amortissement immobilisation. Par conséquent, la fenêtre pour les lois d'amortissement attribuées est intitulée **Lois d'amortissement immo.**.

## <a name="to-create-a-depreciation-book"></a>Pour créer un registre amortissement  
Dans un registre amortissement immobilisation, vous spécifiez comment les immobilisations sont amorties. Pour prendre en charge plusieurs méthodes d'amortissement, vous pouvez paramétrer plusieurs lois d'amortissement.  
1.  Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Lois d'amortissement**, puis sélectionnez le lien connexe.
2. Dans la fenêtre **Liste des lois d'amortissement**, sélectionnez l'action **Nouveau**.
3. Dans la fenêtre **Fiche loi d'amortissement**, renseignez les champs comme nécessaire. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.

    **Remarque** : vous pouvez enregistrer les transactions immobilisation dans la fenêtre **Feuille compta. immo.** ou dans la fenêtre **Feuille immo.**, selon que les transactions sont destinées pour des rapports financiers ou pour la gestion interne. Procédez comme suit pour définir quel type de journal est utilisé pour les différentes activités immobilisation par défaut.
4. Sur le raccourci **Intégration**, cochez la case pour chaque activité immobilisation dont vous souhaitez valider les transactions via la fenêtre **Feuille compta. immo.**.
5. Répétez les étapes 2 à 4 pour chaque méthode d'amortissement ou méthode de report que vous souhaitez attribuer à des immobilisations en tant que registre amortissement.

## <a name="to-assign-a-depreciation-book-to-a-fixed-asset"></a>Pour attribuer un registre amortissement à une immobilisation  
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Immobilisations**, puis sélectionnez le lien connexe.
2. Sélectionnez l'immobilisation pour laquelle vous souhaitez configurer un registre amortissement immobilisation.
3. Sur le raccourci **Loi d'amortissement**, renseignez les champs, le cas échéant.
4. Si vous devez assigner plus d'une loi d'amortissement à l'immobilisation, sélectionnez l'action **Ajouter davantage de lois d'amortissement**.
5. Sinon, sélectionnez l'action **Lois d'amortissement** pour spécifier une, voire plusieurs lois d'amortissement immobilisation.

**Remarque** : lorsque vous utilisez la méthode manuelle d'amortissement, vous devez saisir l'amortissement manuellement dans la feuille comptabilisation immobilisation. La fonction **Calculer amortissement** ignore les immobilisations qui utilisent la méthode d'amortissement manuelle. Vous pouvez recourir à cette méthode pour les immobilisations qui ne font pas l'objet d'un amortissement, par exemple les terrains.

## <a name="to-assign-a-depreciation-book-to-multiple-fixed-assets-with-a-batch-job"></a>Pour attribuer un registre amortissement à plusieurs immobilisations avec un traitement en lot
Pour attribuer une loi d'amortissement à plusieurs immobilisations, vous pouvez utiliser le traitement par lots **Créer lois d'amortissement** pour que Dynamics NAV crée automatiquement les lois d'amortissement immobilisation nécessaires.  
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Immobilisations**, puis sélectionnez le lien connexe.
2. Sélectionnez l'immobilisation à laquelle vous souhaitez attribuer une loi d'amortissement, puis sélectionnez l'action **Modifier**.
3. Dans la fenêtre **Fiche livre d'amortissement**, sélectionnez l'action **Créer plans amortissement**.
4. Dans la fenêtre **Créer plans amortissement immo.**, renseignez le champ **Loi d'amortissement**.
5. Choisissez le champ **Copier immo. n°** , puis sélectionnez le numéro de l'immobilisation à utiliser comme base pour créer de nouvelles lois d'amortissement immobilisation.

    Si vous renseignez ce champ, les champs amortissement des nouveaux registres amortissement immobilisation contiennent les mêmes informations que ceux du registre amortissement immobilisation que vous copiez. N'entrez rien dans ce champ si vous souhaitez créer de nouvelles lois d'amortissement d'immobilisation avec des champs d'amortissement vides.  
6. Sur le raccourci **Immo.**, vous pouvez positionner un filtre afin de sélectionner les immobilisations pour lesquelles vous souhaitez créer des lois d'amortissement immobilisation.
7. Cliquez sur le bouton **OK**.

## <a name="to-set-up-depreciation-posting-types"></a>Pour configurer les types de report amortissement  
Pour chaque registre amortissement, vous devez configurer comment vous souhaitez que Dynamics NAV gère les différents types de report. Par exemple, vous devez indiquer s'il s'agit d'un débit ou d'un crédit et si le type de report doit être inclus dans la base d'amortissement.  
1.  Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Lois d'amortissement**, puis sélectionnez le lien connexe.  
2. Sélectionnez la loi d'amortissement que vous souhaitez configurer, puis sélectionnez l'action **Type paramètre compta. immo.**.
3. Dans la fenêtre **Type paramètre compta. immo.**, renseignez les champs, le cas échéant.

**REMARQUE** : vous ne pouvez pas insérer ni supprimer de lignes dans la fenêtre **Type paramètre compta. immo.**. Vous ne pouvez modifier que les lignes existantes.

Il est recommandé de ne pas modifier la configuration des registres amortissement pour lesquels des écritures ont déjà été reportées. Les modifications apportées n'ont pas d'incidence sur les écritures déjà reportées, ce qui rendrait les statistiques des registres amortissement inexactes.

## <a name="to-set-up-default-templates-and-batches-for-fixed-asset-depreciation"></a>Pour configurer les modèles par défaut et les lots pour l'amortissement immobilisation  
Pour chaque registre amortissement, vous définissez une configuration par défaut de modèles et de lots. Utilisez ces valeurs par défaut pour :
- Dupliquez les lignes d'un journal vers un autre.
- Créez des lignes feuille à l'aide du traitement par lots **Calculer amortissement** ou **Réévaluer immobilisations**
- Dupliquez les coûts d'acquisition dans le journal assurance.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Lois d'amortissement**, puis sélectionnez le lien connexe.
2. Sélectionnez la loi d'amortissement pour laquelle vous souhaitez définir les feuilles par défaut, puis sélectionnez l'action **Configuration feuille immo.**.
3. Pour avoir une configuration par défaut pour chaque utilisateur, choisissez le champ **Code utilisateur** à sélectionner à partir de la fenêtre **Utilisateurs**.
4. Dans les autres champs, sélectionnez le modèle journal ou le lot journal qui doit être utilisé par défaut.

## <a name="see-also"></a>Voir aussi
[Configurer des immobilisations](fa-setup.md)  
[Gérer des immobilisations](fa-manage.md)  
[Finance](finance-setup.md)  
[Bienvenue dans Dynamics NAV](across-get-started.md)

