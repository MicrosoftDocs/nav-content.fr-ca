---
title: "Utilisation de la fonction Transférer la différence vers un compte pour rapprocher les paiements"
description: "Décrit comment traiter les paiements qui ne peuvent pas être affectés dans un document, par exemple lorsqu'un taux de change entraîne un changement de montants."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: payment process, cash receipts
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 14728fea5d8661004c23f65920ca835e1d29ac55
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-reconcile-payments-that-cannot-be-applied-automatically"></a>Procédure : rapprocher les paiements qui ne peuvent pas être affectés automatiquement
Vous serez parfois amené à gérer des paiements sur votre compte bancaire, qui ne peuvent pas être affectés à une écriture client, fournisseur ou compte bancaire ouverte associée. Les motifs peuvent être qu'il n'existe dans [!INCLUDE[d365fin](includes/d365fin_md.md)] aucun document auquel le paiement puisse être lettré, ou que le document associé dans [!INCLUDE[d365fin](includes/d365fin_md.md)] affiche un montant différent du montant de la transaction, par exemple, en raison du taux de change. Dans la fenêtre **Feuille rapprochement bancaire**, tous les montants de transaction pour les paiements qui n'ont pas encore été lettrés s'affichent dans le champ **Différence**, y compris les montants qui ne peuvent pas être lettrés pour des motifs tels que celui qui précède.

Les paiements qui ne peuvent pas être affectés peuvent apparaître sur les lignes journal rapprochement paiement pour les raisons suivantes :

* La valeur du champ **Différence** est égale à celle du champ **Montant transaction**, ce qui indique qu'aucune partie du paiement ne peut être lettrée à une écriture comptable client, fournisseur ou compte bancaire ouverte associée.
* La valeur du champ **Différence** est inférieure à celle du champ **Montant transaction**, ce qui indique qu'une partie du paiement peut être lettrée à une écriture comptable client, fournisseur ou compte bancaire ouverte associée. La partie restante du paiement ne peut pas être affectée et doit être rapprochée manuellement ou en la reportant directement sur un compte.

Pour rapprocher de tels paiements, vous pouvez cliquer sur le bouton **Transférer la différence vers un compte**, puis spécifier sur quel compte le montant du champ **Différence** sera reporté lorsque vous reportez le journal rapprochement paiement.

> [!TIP]  
>   Il existe une fonctionnalité similaire permettant de configurer le rapprochement automatique des paiements récurrents qui ne peuvent pas être affectés aux écritures ouvertes associées du grand livre client, fournisseur ou compte bancaire. Pour plus d'informations, reportez-vous à [Procédure : mapper du texte sur les paiements récurrents aux comptes pour un rapprochement automatique](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md).

## <a name="to-reconcile-payments-that-cannot-be-applied"></a>Pour rapprocher les paiements qui ne peuvent pas être affectés
1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Feuille rapprochement bancaire**, puis sélectionnez le lien connexe.
2. Ouvrez un journal rapprochement paiement. Pour plus d'informations, reportez-vous à [Procédure : rapprocher les paiements à l'aide de l'application automatique](receivables-how-reconcile-payments-auto-application.md).
3. Sélectionnez l'action **Transférer la différence vers un compte**. La fenêtre **Transférer la différence vers un compte** s'ouvre.
4. Dans le champ **Type compte**, spécifiez le type de compte sur lequel le montant du paiement sera validé.
5. Dans le champ **N° compte**, spécifiez le compte dans lequel le montant du paiement sera reporté.
6. Dans le champ **Description**, spécifiez le texte qui décrit cette validation de prélèvement. Par défaut, le texte du champ **Texte transaction** de la ligne feuille rapprochement bancaire est inséré.
7. Cliquez sur le bouton **OK**.

Si la valeur du champ **Différence** est égale à la valeur du champ **Montant transaction** lorsque vous validez la feuille rapprochement bancaire, l'intégralité du paiement sur la ligne feuille sera validé directement dans le compte contrepartie spécifié.

Si la valeur du champ **Différence** était inférieure à la valeur du champ **Montant transaction**, une ligne feuille supplémentaire est créée avec le même texte et la même date et avec la différence insérée dans le champ **Montant transaction**. Sur la ligne feuille d'origine, la différence est déduite de la valeur du champ **Montant transaction**, et le paiement demeure lettré à son écriture comptable client, fournisseur ou compte bancaire associée. Lorsque vous reportez le journal rapprochement paiement, une partie du paiement est reportée en tant que paiement affecté. L'autre partie du paiement est reportée directement dans le compte spécifié.

## <a name="see-also"></a>Voir aussi
[Gestion des comptes client](receivables-manage-receivables.md)  
[Ventes](sales-manage-sales.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

