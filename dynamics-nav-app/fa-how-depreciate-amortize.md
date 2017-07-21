---
title: "Procédure : amortir des immobilisations"
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
ms.openlocfilehash: af71f30681d436ed5da1cd6cb3c2e13f86558631
ms.contentlocale: fr-ca
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-depreciate-or-amortize-fixed-assets"></a>Procédure : amortir des immobilisations
L'amortissement permet de ventiler le coût des immobilisations, telles que les machines et le matériel, sur leur durée d'amortissement. Vous devez définir la méthode d'amortissement de chaque immobilisation.  

 Vous pouvez reporter l'amortissement de deux manières :
- Automatiquement, via l'exécution du traitement par lots **Calculer amortissement**.
- Manuellement, à l'aide du journal GL immobilisation.  

Dynamics NAV peut calculer l'amortissement sur une base quotidienne, ce qui vous permet de calculer l'amortissement pour n'importe quelle période. Vous pouvez ainsi analyser les résultats d'exploitation en cours sur une période mensuelle, trimestrielle ou annuelle. Le calcul utilise une année standard de 360 jours et un mois standard de 30 jours. Pour en savoir plus, voir [Méthodes d'amortissement](fa-depreciation-methods.md).

Lorsqu'une immobilisation est utilisée par plusieurs départements, vous pouvez affecter automatiquement un amortissement périodique à ces départements d'après une table d'affectation paramétrable.  

Vous pouvez ignorer les écritures d'amortissement incorrectes avec le traitement par lots **Annuler écriture comptable immo**. Vous pouvez ensuite valider le montant correct de l'amortissement en exécutant de nouveau le traitement par lots **Calculer amortissement**. Lorsque vous résolvez des erreurs, celles-ci sont reportées en tant qu'écritures erreur immobilisation.  

L'actualisation permet d'ajuster des valeurs en fonction de modifications générales de niveau de prix. Le traitement par lots **Actualiser immobilisation** permet de recalculer les montants des amortissements.  

## <a name="to-calculate-a-depreciation-automatically"></a>Pour calculer automatiquement un amortissement
Une fois par mois, ou à la fréquence de votre choix, vous pouvez lancer le traitement par lots **Calculer amortissement**. Les immobilisations qui ont été vendues, celles qui ont été bloquées ou qui sont inactives, et celles qui utilisent la méthode d'amortissement manuelle ne sont pas prises en compte.    

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Calculer amortissement**, puis sélectionnez le lien connexe.  
2. Renseignez les champs selon vos besoins. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.
3. Cliquez sur le bouton **OK**.  

    Le traitement en lot calcule l'amortissement et crée des lignes dans le journal GL immobilisation.  
4. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Feuilles compta. immo.**, puis sélectionnez le lien connexe.

    Dans la fenêtre **Feuille compta. immo**, dans le champ **Nbre jours amort.**, vous pouvez voir le nombre de jours d'amortissement calculé.  
5. Sélectionnez l'action **Valider**.

## <a name="to-post-a-depreciation-manually-from-the-fixed-asset-gl-journal"></a>Pour reporter un amortissement manuellement à partir du journal GL immobilisation
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Feuille compta. immo.**, puis sélectionnez le lien connexe.  
2. Créez une ligne journal initiale et complétez les champs, le cas échéant.
3. Dans le champ **Type compta. immo**, sélectionnez **Amortissement**.
4. Sélectionnez l'action **Insérer contrepartie immo.**. Une seconde ligne journal est créée pour le compte de contrepartie qui est configuré pour le report de l'amortissement. Pour en savoir plus, voir la section « Pour configurer des groupes de validation d'immobilisation » dans [Procédure : configurer des informations d'immobilisation générales pour les immobilisations](fa-how-setup-general.md).
5. Sous l'onglet **Accueil**, sélectionnez **Valider** pour valider la feuille.

Si vous avez défini des clés d'affectation immobilisation pour affecter des montants entre plusieurs départements ou plusieurs projets, les montants seront affectés lors du report. Pour en savoir plus, voir [Procédure : configurer des informations générales sur les immobilisations](fa-how-setup-general.md).

## <a name="to-calculate-allocations-in-the-fixed-asset-gl-journal"></a>Pour calculer les affectations dans le journal GL immobilisation
Lorsqu'une immobilisation est utilisée par plusieurs départements, vous pouvez affecter automatiquement un amortissement périodique à ces départements d'après une table d'affectation paramétrable.  

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Feuille compta. immo.**, puis sélectionnez le lien connexe.   
Créez une feuille initiale et complétez les champs, le cas échéant.
3. Dans le champ **Type compta. immo**, sélectionnez **Ventilation**.
4. Sélectionnez l'action **Insérer contrepartie immo.**. Une seconde ligne journal est créée pour le compte de contrepartie qui est configuré pour le report de l'affectation.
5. Sous l'onglet **Accueil**, sélectionnez **Valider** pour valider la feuille.

## <a name="use-duplication-lists-to-prepare-to-post-to-multiple-depreciation-books"></a>Utilisez les listes de duplication pour préparer le report vers plusieurs registres amortissement  
Lorsque vous renseignez les lignes journal à reporter dans un registre amortissement, vous pouvez dupliquer les lignes dans un autre journal, après quoi elles peuvent être reportées dans un autre registre amortissement. Pour en savoir plus, voir la section « Pour reporter les écritures vers différents registres amortissement ».

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Lois d'amortissement**, puis sélectionnez le lien connexe.  
2. Ouvrez la loi d'amortissement de votre choix, puis cochez la case **Inclure dans liste duplication**.  

**Important** : si vous avez sélectionné le champ **Utiliser liste duplication**, n'utilisez pas de souches de numéros sur la feuille. En effet, les séries de numéros pour le journal GL immobilisation ne correspondent pas aux séries pour le journal immobilisation.

## <a name="to-post-entries-to-different-depreciation-books"></a>Pour reporter des écritures dans plusieurs registres amortissement  
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Feuille compta. immo.**, puis sélectionnez le lien connexe.
2. Dans la feuille avec laquelle vous souhaitez valider l'amortissement, sélectionnez la case **Utiliser liste duplication**.
3. Renseignez les champs restants selon vos besoins.
4. Sélectionnez l'action **Valider**.
5. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Feuilles immobilisation**, puis sélectionnez le lien connexe.

    La fenêtre **Feuille immobilisation** contient de nouvelles lignes pour différentes lois d'amortissement selon la liste de duplication.   

6. Examinez ou modifiez les lignes, puis sélectionnez l'action **Valider**.

**Remarque** : une autre façon de dupliquer une écriture dans une loi séparée consiste à saisir un code de loi d'amortissement dans le champ **Dupliquer dans journaux amort.** lorsque vous complétez une ligne feuille.

Vous pouvez copier des écritures d'une loi d'amortissement vers une autre à l'aide du traitement par lots **Copier lois d'amortissement**. Le traitement par lots crée des lignes feuille dans la feuille que vous avez indiquée dans la fenêtre **Param. feuille immo.** pour la loi d'amortissement vers laquelle vous souhaitez réaliser la copie. Pour plus d'informations, voir la procédure suivante.

## <a name="to-copy-fixed-asset-ledger-entries-between-depreciation-books"></a>Pour copier des écritures immobilisations entre les registres amortissement  
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Lois d'amortissement**, puis sélectionnez le lien connexe.
2. Ouvrez la fiche loi d'amortissement pertinente, puis sélectionnez l'action **Copier loi d'amortissement**.  
3. Dans la fenêtre **Copier loi d'amortissement**, renseignez les champs comme nécessaire.  
4. Cliquez sur le bouton **OK**.  

Les lignes copiées sont créées dans le journal GL immobilisation ou le journal immobilisation, selon que le registre amortissement que vous copiez a été intégrée dans le grand livre ou non.

## <a name="see-also"></a>Voir aussi
[Gérer des immobilisations](fa-manage.md)  
[Configurer des immobilisations](fa-setup.md)  
[Finance](finance-setup.md)  
[Bienvenue dans Dynamics NAV](across-get-started.md)

