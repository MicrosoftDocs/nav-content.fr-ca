---
title: Affecter des paiements automatiquement et rapprocher des comptes bancaires
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 11df387c16e19421090531fd03c209103b9989d9
ms.contentlocale: fr-ca
ms.lasthandoff: 06/26/2017

---

# <a name="apply-payments-automatically-and-reconcile-bank-accounts"></a>Affecter des paiements automatiquement et rapprocher des comptes bancaires
Vous devez régulièrement rapprocher vos comptes bancaires, client et fournisseur dans Dynamics NAV en affectant les paiements enregistrés au niveau de la banque à leurs factures impayées et notes de crédit associées ou à d'autres écritures ouvertes dans Dynamics NAV.

Vous pouvez effectuer cette tâche dans la fenêtre **Feuille rapprochement bancaire** en important un fichier ou un flux de relevé bancaire pour enregistrer rapidement les paiements dans Dynamics NAV. Une fonction d'affectation automatique affecte les paiements à leurs écritures client ou fournisseur ouvertes associées en fonction des correspondances de données entre le texte de paiement et les informations d'écriture. Vous pouvez réviser et modifier les affectations automatiques avant de reporter le journal. Vous pouvez choisir de fermer les écritures de compte bancaire ouvertes associées aux écritures affectées lorsque vous reportez le journal. Cela signifie que le compte bancaire est automatiquement rapproché lorsque tous les paiements sont affectés.

Pour activer l'importation des relevés bancaires en tant que flux bancaire, vous devez d'abord configurer et activer le service de flux de la Envestnet Yodlee Bank, puis associer vos comptes bancaires aux comptes bancaires connexes en ligne. Pour plus d'informations, reportez-vous à [Procédure: configurer le service de flux de la Envestnet Yodlee Bank](bank-how-setup-bank-statement-service.md).

**Remarque** : le service Envestnet Yodlee Bank Feeds, ou tout service de flux bancaire d'un autre fournisseur, risque de ne pas être disponible dans votre système. Contactez votre partenaire Microsoft si vous souhaitez utiliser un service de flux bancaire pour importer les relevés bancaires.

Vous pouvez également utiliser le service conversion données bancaires pour disposer d'un fichier de relevé bancaire à n'importe quel format converti en flux de données que vous pouvez importer dans Dynamics NAV. Pour plus d'informations, reportez-vous à [Procédure: configurer le service de conversion de données bancaires](bank-how-setup-bank-data-conversion-service.md).

Le tableau suivant décrit une série de tâches et inclut des liens vers les rubriques qui les décrivent.

|À |Voir |
|---|----|
|Affecter des paiements aux écritures client ou fournisseur ouvertes en important un relevé bancaire, et rapprocher le compte bancaire lorsque tous les paiements sont affectés. | [Procédure : rapprocher les paiements à l'aide du lettrage automatique](receivables-how-reconcile-payments-auto-application.md) |
|Appliquer manuellement les paiements en affichant des informations détaillées sur les données de correspondance et des suggestions d'écritures ouvertes candidates auxquelles affecter des paiements. | [Procédure : réviser ou lettrer les paiements après un lettrage automatique](receivables-how-review-apply-payments-auto-application.md)
|Résoudre les paiements qui ne peuvent pas être affectés automatiquement à leurs écritures ouvertes associées, par exemple si les montants sont différents ou si une écriture associée n'existe pas. | [Procédure : rapprocher les paiements qui ne peuvent pas être lettrés automatiquement](receivables-how-reconcile-payments-cannot-apply-auto.md)
|Lier le texte des paiements à des comptes client, fournisseur ou grand livre spécifiques, pour toujours reporter les dépenses ou réceptions récurrentes en liquide sur ces comptes quand ils ne peuvent être affectés à aucun document.| [Procédure : mapper du texte sur les paiements récurrents aux comptes pour un rapprochement automatique](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md)|

## <a name="see-also"></a>Voir aussi
[Gestion des comptes client](receivables-manage-receivables.md)  
[Gestion des ventes](sales-manage-sales.md)

