---
title: Configurer les immobilisations grand livre
description: "Avant d'utiliser des immobilisations, vous devez paramétrer des comptes GL par défaut, des groupes de report, des clés d'affectation, des modèles et lots de journal, ainsi que des codes de classe."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: ecdb1c85526bf9c2583ed5936c2fcc55a27bcb5d
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-general-fixed-assets-information"></a>Procédure : configurer des informations générales pour les immobilisations
Avant de pouvoir gérer les immobilisations, vous devez configurer les comptes du grand livre par défaut, les clés d'affectation, les modèles journal et les lots pour le report et le reclassement des immobilisations. Vous pouvez classer les immobilisations par catégorie, telles que Corporelles et Incorporelles.

## <a name="to-set-up-general-default-values-for-fixed-assets"></a>Pour configurer des valeurs générales par défaut pour les immobilisations
Vous définissez le comportement général ou la fonctionnalité immobilisation et configurez les souches de numéros document dans la fenêtre **Paramètres immobilisations**.

1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Paramètres immobilisations**, puis sélectionnez le lien connexe.  
2. Renseignez les champs selon vos besoins. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-set-up-fixed-asset-posting-groups"></a>Pour configurer des groupes de validation immobilisation
Les groupes comptabilisation permettent de définir des groupes d'immobilisations. Les écritures de ces groupes de report sont reportées dans les mêmes comptes du grand livre.

1. Choisissez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Groupes compta. immo.**, puis choisissez le lien associé.  
2. Sélectionnez l'action **Nouveau**.
3. Dans la fenêtre **Fiche groupe validation immo.**, renseignez les champs, le cas échéant.

    > [!NOTE]  
>   Pour veiller à ce que les comptes de contrepartie pour différentes validations d'immobilisation soient automatiquement insérés lorsque vous sélectionnez l'action **Insérer contrepartie immo.** sur les lignes feuille, procédez comme suit, selon la validation de réévaluation.
4. Sur le raccourci **Compte contrepartie**, dans le champ **Contrep. réévaluation**, sélectionnez le compte général dans lequel vous souhaitez valider les écritures contrepartie pour la réévaluation.

Pour en savoir plus sur l'utilisation de l'action **Insérer contrepartie immo.** sur les lignes feuille compta. immo., voir, par exemple, [Procédure : réévaluer les immobilisations](fa-how-revalue.md).

## <a name="to-set-up-fixed-asset-allocation-keys"></a>Pour configurer les clés de ventilation d'immobilisations
Vous pouvez affecter les transactions à plusieurs départements ou projets sur la base de clés d'affectation paramétrables. Vous pouvez, par exemple, définir une clé d'affectation pour affecter les coûts d'amortissement des véhicules entre le service administratif pour 35 % et le service commercial pour 65 %. Pour plus d'informations, reportez vous à [Procédure : Répartition des coûts et du revenu](year-allocate-costs-income.md).

Les clés d'affectation s'appliquent à des classes d'immobilisations et non à des immobilisations individuelles.

1. Choisissez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Groupes compta. immo.**, puis choisissez le lien associé.  
2. Dans la fenêtre **Groupes compta. immo.**, sélectionnez l'action **Ventilations**, puis choisissez un type de validation.
3. Dans la fenêtre **Ventilations immo.**, renseignez les champs selon vos besoins.
4. Répétez les phases 2 et 3 pour chacun des types de report pour lesquels vous souhaitez définir des clés d'affectation.

## <a name="to-set-up-fixed-asset-journal-templates"></a>Pour configurer les modèles journal immobilisation
Un modèle est une présentation de journal prédéfinie. Le modèle affiche des informations sur les codes suivi, les rapports et les séries de numéros. Pour plus d'informations, voir [Utilisation des feuilles comptabilité](ui-work-general-journals.md).

[!INCLUDE[d365fin](includes/d365fin_md.md)] crée automatiquement un modèle feuille immobilisation la première fois que vous ouvrez la fenêtre **Feuille immobilisation**. Vous pouvez cependant définir d'autres modèles feuille.  

1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Modèles feuille immo.**, puis sélectionnez le lien connexe.  
2. Renseignez les champs selon vos besoins.

## <a name="to-set-up-fixed-asset-journal-batches"></a>Pour configurer des lots journal immobilisation
Vous pouvez configurer plusieurs lots journal, c'est-à-dire des journaux individuels pour chaque modèle journal. Par exemple, chaque employé peut avoir son propre journal dont le nom correspond à ses initiales. Pour plus d'informations, reportez-vous à [Utilisation des feuilles comptabilité](ui-work-general-journals.md).  

1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Modèles feuille immo.**, puis sélectionnez le lien connexe.  
2. Sélectionnez le modèle feuille pertinent, puis l'action **Lots**.
3. Dans la fenêtre **Lots feuille immo.**, renseignez les champs selon vos besoins.

## <a name="to-set-up-fixed-asset-reclassification-journal-templates"></a>Pour configurer des modèles journal reclassement immobilisation
Vous pouvez utiliser les feuilles reclassement dédiées lorsque vous devez transférer, fractionner ou regrouper des immobilisations. [!INCLUDE[d365fin](includes/d365fin_md.md)] crée automatiquement un modèle feuille reclassement immobilisation la première fois que vous ouvrez la fenêtre **Feuille reclass. immo**. Vous pouvez paramétrer d'autres modèles feuille reclassement. Pour plus d'informations, reportez-vous à [Utilisation des feuilles comptabilité](ui-work-general-journals.md).  

1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Modèles feuille reclass. immo**, puis sélectionnez le lien connexe.  
2. Renseignez les champs selon vos besoins.

## <a name="to-set-up-fixed-asset-reclassification-journal-batches"></a>Pour configurer les lots journal reclassement immobilisation
Vous pouvez configurer plusieurs lots journal, c'est-à-dire des journaux individuels pour chaque modèle journal reclassement. Par exemple, chaque employé peut avoir son propre journal reclassement dont le nom correspond à ses initiales. Pour plus d'informations, reportez-vous à [Utilisation des feuilles comptabilité](ui-work-general-journals.md).

1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Modèles feuille reclass. immo**, puis sélectionnez le lien connexe.  
2. Sélectionnez le modèle feuille pertinent, puis l'action **Lots**.
3. Dans la fenêtre **Lots feuille reclass. immo.**, renseignez les champs selon vos besoins.

## <a name="to-set-up-fixed-asset-class-codes"></a>Pour configurer les codes classe immobilisation
Les codes classe immobilisation peut être utilisé pour grouper des immobilisations, par exemple les immobilisations corporelles et les immobilisations incorporelles.

1. Choisissez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Classes immo.**, puis choisissez le lien associé.
2. Saisissez les codes et les noms des classes que vous souhaitez créer.

## <a name="to-set-up-fixed-asset-subclass-codes"></a>Pour configurer les codes sous-classe immobilisation
Le code sous-classe immobilisation permet de regrouper des immobilisations en catégories, comme les bâtiments, les véhicules, le mobilier et les machines.  

1. Choisissez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Sous-classes immo.**, puis choisissez le lien associé.
2. Saisissez les codes et les noms des classes que vous souhaitez créer.

## <a name="to-set-up-fixed-asset-location-codes"></a>Pour configurer les codes emplacement immobilisation
Les codes emplacement immobilisation permettent d'enregistrer l'emplacement de l'immobilisation, tel que le service commercial, l'accueil, l'administration, la production ou un entrepôt. Ces informations sont utiles à des fins d'assurance et de suivi de l'inventaire.

1. Choisissez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Emplacements immo.**, puis choisissez le lien associé.
2. Saisissez les codes et les noms des emplacements immobilisation que vous souhaitez créer.

## <a name="to-register-opening-entries"></a>Pour enregistrer des écritures d'ouverture
Si vous utilisez les immobilisations dans [!INCLUDE[d365fin](includes/d365fin_md.md)] pour la première fois, vous devez d'abord paramétrer le module de comptabilité avant de définir des immobilisations. La manière de procéder est différente si les immobilisations sont intégrées dans le grand livre.  

 La procédure suivante est utilisée si les transactions immobilisation doivent être reportées dans le grand livre.  

1. Assurez-vous que vous avez suivi les procédures de configuration de base pour les immobilisations.  
2. Créez une fiche immobilisation pour chaque immobilisation existante.  
3. Configurez les lois d'amortissement d'immobilisation.  
4. Activez l'intégration dans le grand livre en procédant comme suit.
5. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), saisissez **Lois d'amortissement**, puis sélectionnez le lien connexe.  
6. Sélectionnez le registre amortissement approprié. Sous l'onglet **Accueil**, dans le groupe **Gérer**, choisissez **Modifier** pour ouvrir la fenêtre **Fiche loi d'amortissement**.
7. Sur le raccourci **Intégration**, assurez-vous que tous les champs sont vides en retirant toutes les coches. Si vous disposez de plusieurs registres amortissement, activez l'intégration dans le grand livre pour chacun d'eux.  
8. Dans le journal immobilisation, entrez les lignes suivantes pour chaque immobilisation :
   * Ligne avec le coût d'acquisition.
   * Une ligne avec l'amortissement cumulé jusqu'à la fin de l'exercice financier précédent.
   * Une ligne avec l'amortissement cumulé du début de l'exercice comptable en cours jusqu'à la date à laquelle [!INCLUDE[d365fin](includes/d365fin_md.md)] est défini pour démarrer le calcul de l'amortissement.

Si vous disposez d'autres soldes ouverts, vous pouvez également les saisir maintenant (dépréciation, appréciation, par exemple).  

Si les immobilisations ne sont pas intégrées dans le grand livre, omettez les étapes 4 à 7.

## <a name="see-also"></a>Voir aussi
[Paramétrage d'immobilisations](fa-setup.md)  
[Immobilisations](fa-manage.md)  
[Finances](finance.md)  
[Bienvenue dans [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

