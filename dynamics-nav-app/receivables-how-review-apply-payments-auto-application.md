---
title: "Vérifier les paiements affectés automatiquement et appliquer à nouveau des paiements manuellement"
description: "Après l'affectation automatique des paiements, vous pouvez consulter toutes les écritures d'un paiement et appliquer à nouveau manuellement celles dont l'affectation était incorrecte."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: payment process, reconcile payment, expenses, cash receipts
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 336dd02d1f29e5f80209961eae164a6faeaf65bc
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-review-or-apply-payments-manually-after-automatic-application"></a>Procédure : réviser ou affecter les paiements manuellement après une affectation automatique
Pour chaque ligne feuille représentant un paiement dans la fenêtre **Feuille rapprochement bancaire**, vous pouvez ouvrir la fenêtre **Lettrage paiement** pour afficher toutes les écritures ouvertes candidates au paiement et les informations détaillées pour chaque écriture sur la correspondance des données sur laquelle un lettrage de paiement est basé. Ici, vous pouvez affecter les paiements manuellement ou réaffecter les paiements qui ont été automatiquement affectés à une écriture incorrecte. Pour plus d'informations sur le lettrage automatique, reportez-vous à [Procédure : rapprocher les paiements à l'aide du lettrage automatique](receivables-how-reconcile-payments-auto-application.md).

> [!IMPORTANT]  
>   Lorsque le compte bancaire pour lequel vous rapprochez des paiements est configuré pour la devise locale, la fenêtre **Lettrage paiement** affiche toutes les écritures ouvertes dans la devise locale, y compris les écritures ouvertes pour les documents qui ont été initialement facturés en devise étrangère. Les paiements appliqués aux écritures avec devises converties peuvent donc être validés avec différents montants que celui qui figure sur le document d'origine en raison des taux de change potentiellement différents utilisés respectivement par la banque et [!INCLUDE[d365fin](includes/d365fin_md.md)].

Par conséquent, nous vous recommandons de rechercher les codes devise étrangère dans le champ **Code devise** de la fenêtre **Lettrage paiement** pour vérifier si les lettrages sont basés sur des devises converties. Pour consulter le montant du document initial dans la devise étrangère et visualiser le taux de change utilisé, choisissez le champ **N° écriture affecté à**, puis, dans le menu contextuel, sélectionnez le bouton de zoom pour ouvrir la fenêtre **Écritures client** ou **Écritures fournisseur**.

Aucun ajustement profits et pertes requis en raison de conversions de devise n'est géré automatiquement par [!INCLUDE[d365fin](includes/d365fin_md.md)]..

> [!NOTE]  
>   Vous ne pouvez pas affecter des écritures avec un signe différent du signe figurant sur le paiement. Par exemple, pour fermer une note de crédit négative et sa facture positive associée, vous devez d'abord affecter la note de crédit à la facture, puis affecter le paiement à la facture avec le montant restant réduit.

> [!WARNING]  
>   Si vous utilisez des escomptes, et si la date de paiement est antérieure à la date d'échéance de paiement, le champ **Montant ouvert remise incl.** de la fenêtre **Lettrage paiement** sera utilisé pour la correspondance. Sinon, la valeur du champ **Montant ouvert** sera utilisée. Si le paiement a été effectué avec un montant avec escompte après la date d'échéance du paiement, ou si le montant total a été payé mais qu'un escompte a été accordé, le montant ne correspondra pas.

> [!NOTE]  
>   Vous ne pouvez affecter un paiement qu'à un seul compte. Si vous souhaitez diviser l'affectation sur plusieurs écritures ouvertes, par exemple pour affecter le paiement d'une somme forfaitaire, les écritures ouvertes doivent être pour le même compte. Pour plus d'informations, reportez-vous aux étapes 7 et 8 de la procédure de cette rubrique.

## <a name="to-review-or-apply-payments-after-automatic-application"></a>Pour réviser ou affecter les paiements après une affectation automatique
1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Feuille rapprochement bancaire**, puis sélectionnez le lien connexe.
2. Ouvrez le journal de rapprochement de paiement pour un compte bancaire pour lequel vous souhaitez rapprocher les paiements. Pour plus d'informations, reportez-vous à [Procédure : rapprocher les paiements à l'aide de l'application automatique](receivables-how-reconcile-payments-auto-application.md).
3. Dans la fenêtre **Feuille rapprochement bancaire**, sélectionnez un paiement que vous souhaitez réviser ou lettrer manuellement à une ou plusieurs écritures ouvertes, puis sélectionnez l'action **Lettrer manuellement**.
4. Cochez la case **Lettré** sur la ligne de l'écriture ouverte à laquelle vous voulez lettrer le paiement.
5. Le montant du paiement, qui est également indiqué dans le champ **Montant transaction** de la fenêtre **Lettrage paiement** est inséré dans le champ **Montant lettré**, mais vous pouvez modifier la valeur du champ, par exemple si vous souhaitez lettrer le montant à plusieurs écritures ouvertes.
6. Pour lettrer une partie du montant payé à une autre écriture ouverte pour le compte, par exemple pour lettrer un paiement forfaitaire, cochez la case **Lettré** pour la ligne. Le montant affecté est automatiquement déduit du montant des transactions pour refléter la répartition sur les deux écritures ouvertes.
7. Pour affecter une partie d'un paiement à une ou plusieurs écritures ouvertes qui n'existent pas dans la base de données, créez une ligne sous la ligne pour le même compte. Dans le champ **Montant lettré**, entrez le montant à lettrer sur la nouvelle ligne, puis ajustez la valeur du champ **Montant lettré** de la ligne existante.
8. Répétez les étapes 5, 6 ou 7 pour les autres écritures ouvertes auxquelles vous souhaitez affecter un paiement complet ou partiel.
9. Lorsque vous avez révisé un lettrage de paiement ou lettré manuellement une ou plusieurs écritures ouvertes, sélectionnez l'action **Accepter le lettrage**.

La fenêtre **Lettrage paiement** se ferme puis, dans la fenêtre **Feuille rapprochement bancaire**, la valeur du champ **Fiabilité correspondance** est modifiée et définie sur **Accepté** pour vous indiquer que vous avez révisé ou lettré manuellement le paiement.

## <a name="see-also"></a>Voir aussi
[Gestion des comptes client](receivables-manage-receivables.md)  
[Ventes](sales-manage-sales.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

