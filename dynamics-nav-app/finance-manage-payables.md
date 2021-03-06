---
title: "Gestion de la comptabilité fournisseur"
description: "Aperçu de la manière dont Dynamics NAV vous aide à gérer les comptes fournisseurs, y compris les paiements fournisseur, les créditeurs, les dettes, et le solde dû."
documentationcenter: 
author: bholtorf
manager: edupont
editor: 
ms.prod: dynamics-nav-2018
ms.workload: na
ms.tgt_pltfrm: na
ms.devlang: na
ms.topic: article
ms.search.keywords: vendor payment, creditor, debt, balance due, AP
ms.date: 06/02/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 698cb92c4209f2675fda3a4b2280ab8afad0c9cc
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="managing-payables"></a>Gestion des comptes fournisseur
[!INCLUDE[d365fin_long](includes/d365fin_long_md.md)] dispose de ce dont vous avez besoin pour gérer efficacement les comptes fournisseurs.  

## <a name="payments"></a>Paiements
Il est facile de classer les paiements par ordre de priorité, de prendre en compte les pénalités pour les paiements en retard et de gérer les escomptes pour les paiements anticipés.

Vous pouvez enregistrer les paiements dans un journal général, puis imprimer des chèques avant de reporter le journal de paiements.

Vous pouvez affecter des paiements pour fermer des factures lorsque vous reportez le paiement ou après son report. Le **Mode de lettrage** spécifié pour le fournisseur (sur la **Fiche fournisseur**) détermine si vous devez effectuer ce lettrage manuellement ou s'il est effectué automatiquement. Vous pouvez toujours affecter des transactions manuellement. Toutefois, si le mode de lettrage pour le fournisseur est **Au plus ancien** et que vous ne spécifiez pas avec quel document le paiement doit être appliqué, le paiement sera appliqué avec l'écriture ouverte la plus ancienne pour ce fournisseur.

## <a name="suggest-vendor-payments"></a>Proposer paiements fournisseur
[!INCLUDE[d365fin](includes/d365fin_md.md)] peut proposer différents paiements aux fournisseurs, tels que les paiements arrivant à échéance ou les paiements donnant lieu à un escompte. La proposition de paiement peut tenir compte du montant que vous avez défini comme fonds disponibles pour le paiement, ainsi que de la possibilité d'escompte lors du paiement.

## <a name="issue-checks"></a>Émettre des chèques
[!INCLUDE[d365fin](includes/d365fin_md.md)] vous permet d'émettre des chèques aux fournisseurs manuellement et par voie électronique. Vous pouvez effectuer les deux dans la fenêtre **Feuilles paiement**, dans laquelle vous pouvez également annuler des chèques et afficher des écritures comptables chèque.

## <a name="export-payments-to-a-bank-file"></a>Exporter des paiements vers un fichier bancaire
Lorsque vous êtes prêt à régler un fournisseur, dans la fenêtre **Feuille paiement**, vous pouvez exporter un fichier contenant les informations de paiement sur les lignes feuille. Vous pouvez ensuite transférer le fichier à votre banque électronique afin qu'elle traite les transferts d'argent.

Si vous ne souhaitez pas reporter une ligne journal paiement pour un paiement exporté, par exemple parce que vous attendez la confirmation de la banque que la transaction a été traitée, vous pouvez simplement supprimer la ligne journal. Par la suite, lorsque vous créez une ligne feuille paiement pour payer le montant ouvert de la facture, le champ **Montant total exporté** affiche la quantité du montant ayant déjà été exportée. En outre, vous pouvez rechercher des informations détaillées concernant le total exporté en cliquant sur le bouton **Écritures reg. virement**.

Si vous attendez que votre banque confirme le traitement des transactions pour reporter les paiements, il existe deux méthodes d'éviter de réexporter par erreur les paiements pour les documents ouverts :  

* Dans une feuille paiement avec les lignes paiement proposées, vous pouvez trier soit la colonne **Exporté dans fichier paiement** soit la colonne **Montant total exporté**, puis supprimer les propositions de paiement pour les factures ouvertes pour lesquelles les paiements ont déjà été effectués et pour lesquelles vous ne souhaitez pas effectuer de paiements.

    **Remarque** : vous pouvez être amené à ajouter ces colonnes à la liste. Pour plus d'informations, voir [Personnalisation utilisateur](ui-user-personalization.md).  
* Sinon, dans le traitement par lots **Proposer paiements fournisseur**, où vous spécifiez les paiements à insérer dans la feuille de paiement, vous pouvez spécifier de ne pas insérer de lignes feuille pour les paiements qui ont déjà été exportés en cochant la case **Ignorer les paiements exportés**.

## <a name="see-also"></a>Voir aussi
[Modes de règlement](finance-payment-methods.md)  
[Finances](finance.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

