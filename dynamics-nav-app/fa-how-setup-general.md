---
title: "Procédure : configurer des informations générales pour les immobilisations"
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
ms.openlocfilehash: 8c0e33a78d47ccfbe39a78f81e31b69f61fd4f80
ms.contentlocale: fr-ca
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-general-fixed-assets-information"></a>Procédure : configurer des informations générales pour les immobilisations
Avant de pouvoir gérer les immobilisations, vous devez configurer les comptes du grand livre par défaut, les clés d'affectation, les modèles journal et les lots pour le report et le reclassement des immobilisations. Vous pouvez classer les immobilisations par catégorie, telles que Corporelles et Incorporelles.

## <a name="to-set-up-general-default-values-for-fixed-assets"></a>Pour configurer des valeurs générales par défaut pour les immobilisations
Vous définissez le comportement général ou la fonctionnalité immobilisation et configurez les souches de numéros document dans la fenêtre **Paramètres immobilisations**.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Paramètres immobilisations**, puis sélectionnez le lien connexe.  
2. Renseignez les champs selon vos besoins. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.

## <a name="to-set-up-fixed-asset-posting-groups"></a>Pour configurer des groupes de validation immobilisation  
Les groupes comptabilisation permettent de définir des groupes d'immobilisations. Les écritures de ces groupes de report sont reportées dans les mêmes comptes du grand livre.  
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Groupes de validation immo.**, puis sélectionnez le lien connexe.  
2. Sélectionnez l'action **Nouveau**.
3. Dans la fenêtre **Fiche groupe validation immo.**, renseignez les champs, le cas échéant.

    **Remarque** : pour veiller à ce que les comptes de contrepartie pour différentes validations d'immobilisation soient automatiquement insérés lorsque vous sélectionnez l'action **Insérer contrepartie immo.** sur les lignes feuille, procédez comme suit, selon la validation de réévaluation.
4. Sur le raccourci **Compte contrepartie**, dans le champ **Contrep. réévaluation**, sélectionnez le compte général dans lequel vous souhaitez valider les écritures contrepartie pour la réévaluation.

Pour en savoir plus sur l'utilisation de l'action **Insérer contrepartie immo.** sur les lignes feuille compta. immo., voir, par exemple, [Procédure : réévaluer les immobilisations](fa-how-revalue.md).

## <a name="to-set-up-fixed-asset-allocation-keys"></a>Pour configurer les clés de ventilation d'immobilisations  
Vous pouvez affecter les transactions à plusieurs départements ou projets sur la base de clés d'affectation paramétrables. Vous pouvez, par exemple, définir une clé d'affectation pour affecter les coûts d'amortissement des véhicules entre le service administratif pour 35 % et le service commercial pour 65 %. Pour en savoir plus, voir [Procédure : utiliser les clés de ventilation dans les feuilles générales](ui-how-use-allocation-keys-general-journals.md).

Les clés d'affectation s'appliquent à des classes d'immobilisations et non à des immobilisations individuelles.  
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Groupes de validation immo.**, puis sélectionnez le lien connexe.  
2. Dans la fenêtre **Groupes compta. immo.**, sélectionnez l'action **Ventilations**, puis choisissez un type de validation.
3. Dans la fenêtre **Ventilations immo.**, renseignez les champs selon vos besoins.
4. Répétez les phases 2 et 3 pour chacun des types de report pour lesquels vous souhaitez définir des clés d'affectation.

## <a name="to-set-up-fixed-asset-journal-templates"></a>Pour configurer les modèles journal immobilisation  
Un modèle est une présentation de journal prédéfinie. Le modèle affiche des informations sur les codes suivi, les rapports et les séries de numéros. Pour plus d'informations, reportez-vous à [Utilisation des feuilles comptabilité](ui-work-general-journals.md).

Dynamics NAV crée automatiquement un modèle feuille immobilisation la première fois que vous ouvrez la fenêtre **Feuille immobilisation**. Vous pouvez cependant définir d'autres modèles feuille.  
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Modèles feuille immo.**, puis sélectionnez le lien connexe.  
2. Renseignez les champs selon vos besoins.

## <a name="to-set-up-fixed-asset-journal-batches"></a>Pour configurer des lots journal immobilisation
Vous pouvez configurer plusieurs lots journal, c'est-à-dire des journaux individuels pour chaque modèle journal. Par exemple, chaque employé peut avoir son propre lot journal dont le nom correspond à ses initiales. Pour plus d'informations, reportez-vous à [Utilisation des feuilles comptabilité](ui-work-general-journals.md).  
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Modèles feuille immo.**, puis sélectionnez le lien connexe.  
2. Sélectionnez le modèle feuille pertinent, puis l'action **Lots**.
3. Dans la fenêtre **Lots feuille immo.**, renseignez les champs selon vos besoins.

## <a name="to-set-up-fixed-asset-reclassification-journal-templates"></a>Pour configurer des modèles journal reclassement immobilisation  
Vous pouvez utiliser les feuilles reclassement dédiées lorsque vous devez transférer, fractionner ou regrouper des immobilisations. Dynamics NAV crée automatiquement un modèle feuille reclassement immobilisation la première fois que vous ouvrez la fenêtre **Feuille reclass. immo**. Vous pouvez paramétrer d'autres modèles feuille reclassement. Pour plus d'informations, reportez-vous à [Utilisation des feuilles comptabilité](ui-work-general-journals.md).  
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Modèles feuille reclass. immo.**, puis sélectionnez le lien connexe.  
2. Renseignez les champs selon vos besoins.

## <a name="to-set-up-fixed-asset-reclassification-journal-batches"></a>Pour configurer les lots journal reclassement immobilisation  
Vous pouvez configurer plusieurs lots journal, c'est-à-dire des journaux individuels pour chaque modèle journal reclassement. Par exemple, chaque employé peut avoir son propre lot journal reclassement dont le nom correspond à ses initiales. Pour plus d'informations, reportez-vous à [Utilisation des feuilles comptabilité](ui-work-general-journals.md).
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Modèles feuille reclass. immo.**, puis sélectionnez le lien connexe.  
2. Sélectionnez le modèle feuille pertinent, puis l'action **Lots**.
3. Dans la fenêtre **Lots feuille reclass. immo.**, renseignez les champs selon vos besoins.

## <a name="to-set-up-fixed-asset-class-codes"></a>Pour configurer les codes classe immobilisation  
Les codes classe immobilisation peut être utilisé pour grouper des immobilisations, par exemple les immobilisations corporelles et les immobilisations incorporelles.
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Classes immo.**, puis sélectionnez le lien connexe.
2. Saisissez les codes et les noms des classes que vous souhaitez créer.

## <a name="to-set-up-fixed-asset-subclass-codes"></a>Pour configurer les codes sous-classe immobilisation
Le code sous-classe immobilisation permet de regrouper des immobilisations en catégories, comme les bâtiments, les véhicules, le mobilier et les machines.  
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Sous-classes immo.**, puis sélectionnez le lien connexe.
2. Saisissez les codes et les noms des classes que vous souhaitez créer.

## <a name="to-set-up-fixed-asset-location-codes"></a>Pour configurer les codes emplacement immobilisation
Les codes emplacement immobilisation permettent d'enregistrer l'emplacement de l'immobilisation, tel que le service commercial, l'accueil, l'administration, la production ou un entrepôt. Ces informations sont utiles à des fins d'assurance et de suivi de l'inventaire.
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Configurations immo.**, puis sélectionnez le lien connexe.
2. Saisissez les codes et les noms des emplacements immobilisation que vous souhaitez créer.

## <a name="to-register-opening-entries"></a>Pour enregistrer des écritures d'ouverture  
Si vous utilisez les immobilisations dans Dynamics NAV pour la première fois, vous devez d'abord configurer le module Grand livre avant de configurer des immobilisations. La manière de procéder est différente si les immobilisations sont intégrées dans le grand livre.  

 La procédure suivante est utilisée si les transactions immobilisation doivent être reportées dans le grand livre.  

1. Assurez-vous que vous avez suivi les procédures de configuration de base pour les immobilisations.  
2. Créez une fiche immobilisation pour chaque immobilisation existante.  
3. Configurez les lois d'amortissement d'immobilisation.  
4. Activez l'intégration dans le grand livre en procédant comme suit.
5. Dans la zone **Rechercher**, entrez **Lois d'amortissement**, puis sélectionnez le lien associé.  
6. Sélectionnez le registre amortissement approprié. Sous l'onglet **Accueil**, dans le groupe **Gérer**, choisissez **Modifier** pour ouvrir la fenêtre **Fiche loi d'amortissement**.
7. Sur le raccourci **Intégration**, assurez-vous que tous les champs sont vides en retirant toutes les coches. Si vous disposez de plusieurs registres amortissement, activez l'intégration dans le grand livre pour chacun d'eux.  
8. Dans le journal immobilisation, entrez les lignes suivantes pour chaque immobilisation :
    - Ligne avec le coût d'acquisition.
    - Une ligne avec l'amortissement cumulé jusqu'à la fin de l'exercice financier précédent.
    - Une ligne avec l'amortissement cumulé du début de l'exercice financier en cours jusqu'à la date à laquelle Dynamics NAV est défini pour démarrer le calcul de l'amortissement.

Si vous disposez d'autres soldes ouverts, vous pouvez également les saisir maintenant\-, (amortissement, réévaluation, par exemple).  

Si les immobilisations ne sont pas intégrées dans le grand livre, omettez les étapes 4 à 7.

## <a name="see-also"></a>Voir aussi
[Configurer des immobilisations](fa-setup.md)  
[Gérer des immobilisations](fa-manage.md)  
[Finance](finance-setup.md)  
[Bienvenue dans Dynamics NAV](across-get-started.md)

