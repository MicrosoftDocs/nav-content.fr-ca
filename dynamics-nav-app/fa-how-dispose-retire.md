---
title: "Procédure : céder ou annuler des immobilisations"
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
ms.openlocfilehash: 795bb23e7c0b46be095b2bbdfe7705b3d7b1e4ee
ms.contentlocale: fr-ca
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-dispose-of-or-retire-fixed-assets"></a>Procédure : céder ou annuler des immobilisations
Lorsque vous commercialisez ou cédez une immobilisation, la valeur de cession doit être reportée pour calculer et enregistrer le gain ou la perte. Une écriture cession doit être la dernière écriture reportée pour une immobilisation. Pour les immobilisations partiellement cédées, vous pouvez reporter plusieurs écritures cession. Le total de tous les montants de cession reportés doit être un montant crédit.

 **REMARQUE** : Si vous négociez une immobilisation en échange d'une autre, vous devez enregistrer à la fois la vente de l'ancienne immobilisation (cession) et l'achat de la nouvelle (acquisition). Pour en savoir plus, voir [Procédure : acquérir les immobilisations](fa-how-acquire.md).

## <a name="to-post-a-disposal-from-the-fixed-asset-gl-journal"></a>Pour reporter une cession à partir du journal GL immobilisation  
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Feuilles compta. immo.**, puis sélectionnez le lien connexe.  
2. Créez une ligne journal initiale et complétez les champs, le cas échéant. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.
3. Dans le champ **Type compta. immo**, sélectionnez **Cession**.
4. Sélectionnez l'action **Insérer contrepartie immo.**. Une seconde ligne journal est créée pour le compte de contrepartie qui est configuré pour le report de la cession.

    **Remarque** : l'étape 4 ne fonctionne que si vous avez configuré ce qui suit : la fenêtre **Fiche groupe compta. immo.** pour le groupe de validation de l'immobilisation, le champ **Cession immobilisation** contient le compte débit général et le champ **Compte contrepartie cession** contient le compte général auquel vous souhaitez valider les écritures contrepartie pour appréciation. Pour en savoir plus, voir la section « Pour configurer des groupes de validation d'immobilisation » dans [Procédure : configurer des informations d'immobilisation générales pour les immobilisations](fa-how-setup-general.md).
5. Sélectionnez l'action **Valider**.

Si vous vendez une immobilisation ou en cédez une partie, vous devez d'abord diviser l'immobilisation avant de pouvoir enregistrer la transaction cession. Pour en savoir plus, voir [Procédure : transférer, fractionner ou regrouper les immobilisations](fa-how-trans-split-combine.md).

## <a name="to-view-disposal-ledger-entries"></a>Pour visualiser des écritures cession  
Lorsque vous vendez ou cédez une immobilisation, la valeur de cession est reportée dans le grand livre où vous pouvez afficher le résultat.   

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Immobilisations**, puis sélectionnez le lien connexe.  
2. Sélectionnez l'immobilisation pour laquelle vous souhaitez afficher les écritures, puis sélectionnez l'action **Lois d'amortissement**.
3. Sélectionnez la loi d'amortissement pour laquelle vous souhaitez afficher les écritures, puis sélectionnez l'action **Écritures comptables**.
4. Sélectionnez une ligne avec **Cession** dans le champ **Catégorie compta. immo.**, puis sélectionnez l'action **Naviguer**.  
5. Dans la fenêtre **Naviguer**, sélectionnez la ligne d'écriture comptable, puis l'action **Afficher**.
La fenêtre **Écritures comptables** s'ouvre. Vous pouvez y voir les écritures résultant de la validation de la cession.

## <a name="see-also"></a>Voir aussi
[Gérer des immobilisations](fa-manage.md)  
[Configurer des immobilisations](fa-setup.md)  
[Finance](finance-setup.md)  
[Bienvenue dans Dynamics NAV](across-get-started.md)

